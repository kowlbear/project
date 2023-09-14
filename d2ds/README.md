# Dart2dataStudio
Dart 에서 제공하는 api를 통하여 데이터를 수집 후 google Datastudio를 통해 누구나 쉽게 볼 수 있는 Dashboard로 시각화하였습니다.
데이터 링크 : https://github.com/kowlbear/project/blob/c6c5020b603db32b2ada760ce12be51b7a729171/d2ds/dart_api.ipynb

## 1. 데이터 흐름
  해당 데이터의 흐름은 다음과 같습니다.
  
  전자공시시스템(DART) -> opendart api를 통한 데이터 호출 -> python의 pandas 및 gspread 라이브러리를 통하여 데이터 전처리 및 저장 -> google looker studio(data studio)를 통한 Dashboard 구현
![image](https://github.com/kowlbear/project/assets/86779997/7979b792-0c73-46b0-b9c1-105f9f04ce83)



## 2. dashboard 구현과정
### 데이터 수집
opendart api를 발급받아 기업의 재무재표 데이터를 가져옵니다. 사용한 api 데이터는 단일회사 주요계정을 바탕으로 제작하였습니다.
호출한 데이터는 삼성전자의 2022년 사업보고서입니다.

### 데이터 전처리
요청한 데이터는 pandas 라이브러리를 통하여 Dataframe으로 처리하였고, 결측치와 원본데이터의 쉼표(,)를 전처리하였습니다.

### 데이터 저장
전처리한 Dataframe을 서비스 google cloud 내 google sheet에 저장하였습니다.
gspread 라이브러리를 사용을 위한 권한 인증 먼저 진행하였습니다.
google sheet api의 권한 인증을 위하여 서비스할 계정을 발급받은 후 인증정보가 있는 json 파일을 읽습니다. 권한인증 후 저장할 google sheet를 오픈한 후에  dataframe을 해당 sheet에 저장하였습니다.

### 데이터 시각화
cloud에 저장된 google sheet를 looker studio로 보고서를 만들었습니다.
저장한 sheet를 데이터 연결하였고, 측정기준과 측정항목을 매핑하여 표로 구현하였습니다.
그 후, 계정별 당기/전기/전전기 순으로 계정값을 차트로 표현하였습니다.

   아래 링크를 통하여 Dashboard를 확인할 수 있습니다.[
   https://lookerstudio.google.com/reporting/7b488fb6-c7d5-431d-bdf5-5d00b05bb75d](https://lookerstudio.google.com/reporting/7b488fb6-c7d5-431d-bdf5-5d00b05bb75d)
![image](https://github.com/kowlbear/project/assets/86779997/5d184bce-50de-44d7-813f-3b22392cc1b9)

### 
   
## 3. 개선사항
### SQL 통한 데이터 저장 및 활용
  해당 방법은 sql없이 간단한 데이터 구축을 위하여 google sheet로 구현한 버전입니다.
  sql을 통한 방법은 추후 업데이트 할 예정입니다.
### 
