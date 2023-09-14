# Dart2dataStudio
Dart 에서 제공하는 api를 통하여 데이터를 수집 후 google Datastudio를 통해 누구나 쉽게 볼 수 있는 Dashboard로 시각화하였습니다.

## 1. 데이터 흐름
  해당 데이터의 흐름은 다음과 같습니다.
  전자공시시스템(DART) -> opendart api를 통한 데이터 호출 -> python의 pands 및 gspread 라이브러리를 통하여 데이터 변환 및 저장 -> google looker studio(data studio)를 통한 Dashboard 구현

## 2. dashboard 구현
   아래 링크를 통하여 Dashboard를 구현하였습니다.
   https://lookerstudio.google.com/reporting/7b488fb6-c7d5-431d-bdf5-5d00b05bb75d
## 3. 개선사항
