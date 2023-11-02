# 미국 주별 범죄율에 따른 연관성 분석
<img src="https://github.com/addinedu-amr-4th/eda-repo-6/assets/143172717/71fa49e2-6c31-4036-a188-d8fc47ee5bc3" width="730">

#### 6조 러버덕의 EDA 프로젝트
#### 개발기간: 2023.09.07~2023.09.14 (7일)
- - -
<br/><br/>

## :us:미국의 인구는 말이죠
전 세계의 5%에 불과하지만 죄수의 인구는 25%에 달한다고 합니다.

또한 연방정부인 미국은 주마다 법이 조금씩 달라 특성이 굉장히 다양합니다.

그럼 미국의 범죄 또한 주별마다 다르게 나타나지 않을까요?
<br/><br/><br/>
## :books:처음에는 이렇게 생각했습니다.
<img src="https://github.com/addinedu-amr-4th/eda-repo-6/assets/143172717/b24645f9-794a-4002-8fad-3f17e35717e0" width="730">
<br/><br/><br/>

## :chart_with_upwards_trend:본격적인 데이터 분석
교육수준과 소득을 나타내는 지표들을 찾아 크롤링할려고 노력했습니다.
### 데이터 출처
|미국 교육부|연방 준비 은행 경제 데이터|Kaggle|
|---------|--------------------|-------|
|공립학교 학생 수|중위소득|범죄 데이터|
|공립학교 수|고졸이상 학력자 비율||
|4년제 대학교 수|학위이상 학력자 비율||

> 2015년 ~ 2019년 사이의 미국 51개 주별 데이터를 가지고 분석

###  출처 사이트
- csv 및 excel 다운로드
[범죄 데이터](https://www.kaggle.com/datasets/tunguz/us-estimated-crimes "Kaggle Link")  
[미국 교육부 자료](https://www.kaggle.com/datasets/tunguz/us-estimated-crimes "Digest of Education Statistics")  
[미국 인구조사국 자료](https://www.census.gov/en.html "Digest of Education Statistics")

- 웹 크롤링
[연방 준비 은행 경제 데이터](https://fred.stlouisfed.org/ "Federal Reserve economic data")
<br/><br/>
## 0. 데이터의 연관성을 나타내는 지표
- 지도 시각화 folium
- 산점도
- 피어슨 상관계수
<br/><br/>
## 1. 교육수준 <-> 범죄율
### 1.1 10대들의 교육수준 <-> 차량절도
- 미국 학생들의 차량 절도 유행으로 인해, 교육수준과 차량절도는 양의 상관관계를 가질 것으로 예상했습니다.

<img src="https://github.com/addinedu-ros-3rd/eda-repo-6/assets/143172717/7631a08a-827c-459a-acc1-598fbdc12921" width="300" height="300">
<img src="https://github.com/addinedu-ros-3rd/eda-repo-6/assets/143172717/0d6baf2a-d188-4912-929e-4db21eb8671a" width="300" height="300">
<img src="https://github.com/addinedu-ros-3rd/eda-repo-6/assets/143172717/87c53826-649a-4fb5-981a-26e304483b31" width="300" height="300">

- 하지만 각각의 상관계수는 약 0.255, 0.073, 0.214로 교육수준과 차량절도는 크게 상관이 있지 않았습니다.
<br/>

### 1.2 학벌 <-> 범죄율
<img src="https://github.com/addinedu-ros-3rd/eda-repo-6/assets/143172717/c6e04301-385a-4168-9683-4135dad74d08" width="300" height="300">
<img src="https://github.com/addinedu-ros-3rd/eda-repo-6/assets/143172717/4e19fdad-d775-4083-89e7-4e21bf9dc6fa" width="300" height="300">

- 학위수여자와 주별 대학교의 수 또한 범죄율과 상당히 낮은 상관관계를 보였습니다.
<br/><br/>

## 2. 소득수준 <-> 재산범죄
- 재산범죄에는 절도, 차량절도, 주거침입이 해당되어 있지만 중위소득과 0.6 이상의 상관관계를 보이는 범죄는 주거침입 뿐이었습니다.
<img src="https://github.com/addinedu-ros-3rd/eda-repo-6/assets/143172717/69c35b58-63fb-4de6-af69-032ba8542c3a" width="300" height="300">
<img src="https://github.com/addinedu-ros-3rd/eda-repo-6/assets/143172717/a85a645b-6f1b-424f-88e6-762e4c285275" width="300" height="300">
<br/><br/>
<img src="https://github.com/addinedu-ros-3rd/eda-repo-6/assets/143172717/feecaa76-aa9a-4ce4-9fbc-231b537bcba1" width="300" height="300">


- 자퇴율 또한 주거침입과 0.588의 상관관계를 보여주었습니다.
<br/><br/>

## 인구 <-> 범죄율
- 범죄의 숫자는 인구수와 거의 정비례합니다.
- 미국의 인구는 캘리포니아에 집중되어 있습니다.
- 범죄율이 제일 높은 주는 워싱턴 D.C. 특별자치구인 미국의 수도이며 도시의 동쪽 외곽지역의 범죄율이 굉장히 높다고 합니다.

<img src="https://github.com/addinedu-ros-3rd/eda-repo-6/assets/143172717/2dad999f-1a0e-46bd-bfa3-c6194ae2c51d" width="300" height="300"><img src="https://github.com/addinedu-ros-3rd/eda-repo-6/assets/143172717/ebbc130b-258c-4c66-a678-78c042b2740e" width="600" height="300">
<img src="https://github.com/addinedu-ros-3rd/eda-repo-6/assets/143172717/eb772c47-dc45-4df9-9c71-6158da387feb">
- 지도 시각화 folium




<br/><br/>
## 결론
1. 학력과 범죄율은 크게 상관이 없다.
2. 재산범죄에 포함되는 절도, 차량절도, 주거침입은 성격이 매우 다르다.
3. 소득과 빈곤율은 주거침입과 연관이 높다.
<br/><br/>
## 관련자료
[EDA 프로젝트 6조.pptx](https://docs.google.com/presentation/d/1tfwY901hPHnBKaL9KJIQmcHlLjEO1uCErJ3Oh_hnNHc/edit#slide=id.g2441b38e2e7_1_135)
