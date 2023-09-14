# Dart2dataStudio
Dart 에서 제공하는 api를 통하여 데이터를 수집 후 google Datastudio를 통해 누구나 쉽게 볼 수 있는 Dashboard로 시각화하였습니다.
데이터 링크 : https://github.com/kowlbear/project/blob/c6c5020b603db32b2ada760ce12be51b7a729171/d2ds/dart_api.ipynb

## 1. 데이터 흐름
  해당 데이터의 흐름은 다음과 같습니다.
  전자공시시스템(DART) -> opendart api를 통한 데이터 호출 -> python의 pands 및 gspread 라이브러리를 통하여 데이터 변환 및 저장 -> google looker studio(data studio)를 통한 Dashboard 구현
  

## 2. dashboard 구현
   아래 링크를 통하여 Dashboard를 구현하였습니다.[
   https://lookerstudio.google.com/reporting/7b488fb6-c7d5-431d-bdf5-5d00b05bb75d](https://lookerstudio.google.com/reporting/7b488fb6-c7d5-431d-bdf5-5d00b05bb75d)
![image](https://github.com/kowlbear/project/assets/86779997/5d184bce-50de-44d7-813f-3b22392cc1b9)

   
## 3. 개선사항
  해당 방법은 sql없이 간단한 데이터 구축을 위하여 google sheet로 구현한 버전입니다.
  sql을 통한 방법은 추후 업데이트 할 예정입니다.
