# 미국 주별 범죄율에 따른 연관성 분석
<img src="https://github.com/addinedu-amr-4th/eda-repo-6/assets/143172717/71fa49e2-6c31-4036-a188-d8fc47ee5bc3" width="730">

> 6조 러버덕의 EDA 프로젝트
- - -
<br/><br/><br/>

## :us:미국의 인구는 말이죠
전 세계의 5%에 불과하지만 죄수의 인구는 25%에 달한다고 합니다.

또한 연방정부인 미국은 주마다 법이 조금씩 달라 특성이 굉장히 다양합니다.

그럼 미국의 범죄 또한 주별마다 다르게 나타나지 않을까요?
<br/><br/><br/>
## :books:처음에는 이렇게 생각했습니다.
<img src="https://github.com/addinedu-amr-4th/eda-repo-6/assets/143172717/b24645f9-794a-4002-8fad-3f17e35717e0" width="730">
<br/><br/><br/>

## 미국 학생들의 차량 절도 유행

교육수준과 차량절도는 양의 상관관계를 가질 것이다.

<img src="https://github.com/addinedu-amr-4th/eda-repo-6/assets/143172717/e3078807-940b-4291-812a-485fa789d6bd" width="730">
<img src="https://github.com/addinedu-amr-4th/eda-repo-6/assets/143172717/17ba461c-54b1-4b74-bcc0-a02a70ca018e" width="730">
<br/><br/><br/>

## :chart_with_upwards_trend:데이터의 연관성을 나타내는 지표
- 지도 시각화 folium
- 산점도
- 피어슨 상관계수


## 데이터 출처
* Kaggle
  * 범죄 데이터
* 미국 교육부
  * 공립학교 학생 수
  * 공립학교 수
  * 4년제 대학교 수
* 연방 준비 은행 경제 데이터
  * 중위소득
  * 고졸이상 학력자 비율
  * 학위이상 학력자 비율 
* 미국 인구조사국
  * 빈곤율

2015년 ~ 2019년 사이의 미국 51개 주별 데이터를 가지고 분석.

## 데이터베이스 구축
### 1. 데이터 수집
#### 1-1. csv 및 excel 다운로드
[범죄 데이터](https://www.kaggle.com/datasets/tunguz/us-estimated-crimes "Kaggle Link")

[미국 교육부 자료](https://www.kaggle.com/datasets/tunguz/us-estimated-crimes "Digest of Education Statistics")
[미국 인구조사국 자료](https://www.census.gov/en.html "Digest of Education Statistics")

#### 1-2. 웹 크롤링
[연방 준비 은행 경제 데이터](https://fred.stlouisfed.org/ "Federal Reserve economic data")

### 2. 데이터 전처리
### 3. 데이터베이스 구축

## 데이터분석: 시각화 & 상관계수

## 관련자료
[EDA 프로젝트 6조.pptx](https://docs.google.com/presentation/d/1tfwY901hPHnBKaL9KJIQmcHlLjEO1uCErJ3Oh_hnNHc/edit#slide=id.g2441b38e2e7_1_135)
