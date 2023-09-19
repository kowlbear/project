# NextGameIs
가지고 있는 데이터를 바탕으로 다음 분기에 어떤 게임을 설계해야 할까 라는 고민을 안고 데이터를 정리
본 데이터는 2016년 까지의 판매량을 바탕으로 2017년에 개발에 착수할 게임의 장르 및 플랫폼을 선정하는 분석 보고서를 만드는 것이 목표

# 데이터 링크
https://github.com/kowlbear/project/blob/8b3837487547812d461220030ebd82e5c609b509/nextGameIs/DA_NextGameIs.ipynb

## 분석 목표
분석에서 아래와 같은 점을 고려하면서 분석을 진행

>1. 지역에 따라서 선호하는 게임 장르가 다를까
>2. 연도별 게임의 트렌드가 있을까
>3. 출고량이 높은 게임에 대한 분석 및 시각화 프로세스가 포함

## Data Description
>Name : 게임의 이름
>
>Platform : 게임이 지원되는 플랫폼
>
>Year : 게임 출시연도
>
>Genre : 게임의 장르
>
>Publisher : 게임을 제작한 회사
>
>NA_Sales : 북미지역에서의 출고량
>
>EU_Sales : 유럽지역에서의 출고량
>
>JP_Sales : 일본지역에서의 출고량
>
>Other_Sales : 기타지역에서의 출고량
>

## 연도별 선호 장르
![image](https://user-images.githubusercontent.com/86779997/161512176-1562cdad-206a-47ae-a7c7-54c722bcf727.png)

시대별로 공통적으로 액션과 스포츠가 강세이며
최근 슈터 장르의 선호도가 증가 중이다

## 2010년대 플랫폼 선호도
![image](https://user-images.githubusercontent.com/86779997/161526246-527daf94-33d8-40c4-873b-7062b4be839f.png)

판매량은 휴대용 게임기보다 거치형 게임기의 판매량이 월등히 높고
그 중에서 PS4, PS5의 판매량의 합(35%)과 비교하면 X360, XOne의 판매량의 합(28%)에 비하여 판매량이 높은 추세이다

## 최근 최다 판매량을 세운 게임


2010년 이후 제일 많이 팔린 게임은 GTA5이다.

![image](https://github.com/kowlbear/project/assets/86779997/5dff9869-d82d-4512-8653-d9f302277eaa)


![image](https://github.com/kowlbear/project/assets/86779997/25390d6b-c7fe-49e1-8618-e9afc28f3788)



### 그러나 시리즈 판매량을 합산한다면 Call of duty 시리즈가 가장 많은 판매량을 보였다.

이는 GTA5의 판매량보다 약 3배 많은 수치를 보였다.

![image](https://github.com/kowlbear/project/assets/86779997/ff5c1ea4-8335-497b-a087-d9556188b2f6)

![image](https://github.com/kowlbear/project/assets/86779997/51edbc5b-1898-4da1-84fa-87e0d4c4b1ad)



아래는 해당 수치를 시각화한 자료이다.

![image](https://github.com/kowlbear/project/assets/86779997/aefe52ab-91e8-4312-bdba-a0306962ba2a)



## 결론

- 지역별 게임 장르 선호도는 차이가 있음

 - 공통적으로 액션 및 스포츠 장르의 점유율이 높음
 - 시대별로 트렌드의 변화는 존재하였다.

  > 80s : 플래포머, 퍼즐, 슈팅
  >
  > 90s : 플래포머, 롤플레잉, 슈팅
  >
  > 00s : 액션, 스포츠, 레이싱
  >
  > 10s : 액션, 슈팅, 스포츠
 - 근 10년간 플랫폼별 게임 판매량은 플레이스테이션 진영이 많다

 - PS4의 판매량이 XOne 판매량의 약 2배인 것을 보아 발매 플랫폼은 플레이스테이션이 유리할 것으로 판단
 - 최근 10년간 최대 판매량을 가진 게임시리즈는 콜 오브 듀티 시리즈이며, GTA5 판매량보다 약 3배가량 높다.
 - 그리고, 지역별 판매량은 북미가 제일 많이 높다
   
 ### 따라서 다음 분기에 신규 게임 제작은 북미시장 타겟의 플레이스테이션 플랫폼 슈 게임 개발에 착수하는 것이 유리하다.
