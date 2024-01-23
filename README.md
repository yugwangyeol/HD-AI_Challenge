# HD-AI-CHALLENGE

<br/>

## 1. 배경 & 목적
 
- 예선 : 항만 內 선박 대기 시간 예측을 위한 선박 항차 데이터 분석 AI 알고리즘 개발
- 본선 : 센서 데이터를 활용하여 건설 현장 운용 효율화를 위한 작업자의 운전 성향과 숙련도에 영향을 받지 않고 정확한 작업 중량을 예측할 수 있는 모델을 개발

<br/>

## 2. 주최/주관 & 팀원 & 성과

- 주최/주관: HD한국조선해양 AI Center/DACON
- 참가인원 : 1,439명
- 성과 : 에선(10등) 본선(1등,대상 수상)
<br/>
![170000790063290](https://github.com/yugwangyeol/HD-AI_Challenge/assets/72298825/6e58aaa6-6a8a-4ede-8dde-a1828ef08482)

<br/>

## 3. 프로젝트 기간

- 예선 : 2023년 9월 25일 ~ 10월 30일
- 본선 문제 모델링 진행 : 2023년 11월 06일 ~ 11월 09일
- 오프라인 본선 진행 : 2023년 11월 10일
- 최종 결과 발표 : 2023년 11월 15일
- 시상식 : 2023년 11월 30일 (HD 현대 포럼)

<br/>

## 4. 프로젝트 소개

**[예선]**  
<br/>
&nbsp;&nbsp;&nbsp;&nbsp; HD-AI-CHALLENGE 예선에서는 선박 데이터를 가지고 항만 내 선박 대기시간 에측을 휘안 AI 알고리즘 개발을 진행하였다. 데이터는 약 39만개의 train data와 약 22만개의 test data가 주어졌다. 예선 대회 도중 특이한 점은 대회 마감 13일 전에 대회 데이터가 수정되었다. 1차적으로 주어진 데이터에서는 유가 정보인 ['DUBAI', 'BRENT', 'WTI', 'BDI_ADJ']와 날짜 정보만으로 항만 대기 시간을 구할 수 있었다. 이는 유가 정보가 target의 정보를 포함하고 있어서 Data Leakage로 데이터 수정되었다.  

&nbsp;&nbsp;&nbsp;&nbsp; 유가 정보를 제외한 데이터로 13일 동안 대회를 진행하였다. 남은 데이터로 target과 관련된 EDA를 진행하였고, 날씨 데이터가 target과 유사한 패턴을 보임을 확인하였다. 이후 항만 데이터, 날짜 데이터, 날씨 데이터를 바탕으로 Feature 생성을 진행하였고, 짤읍 시간 내에 성능을 대기 위해 AutoML모델인 Autogluon을 사용하여 기본적인 target값을 구헀다. 이후 EDA에서 파악한 패턴을 바탕으로 후처리 알고리즘을 생성하여 target을 새롭게 생성하였다. 알고리즘 적용 여부에 따라 성능이 크게 차이남을 보였다. 해당 후처리 방법론을 통해 예선을 Public score 9th(0.6%) 32.05994 | Private score 10th(0.6%) 32.45594으로 통과하였다.  

**[본선]**
<br/>
![스크린샷 2024-01-23 203817](https://github.com/yugwangyeol/HD-AI_Challenge/assets/72298825/f8ae4b47-d6c4-46ac-9c74-5961eda52f3c)

&nbsp;&nbsp;&nbsp;&nbsp; 본선에서는 4개의 sensor 데이터와 3개의 sinal 데이터를 가지고, 사용자의 숙련도에 상관없이 작업 중량을 예측하는 AI 알고리즘을 개발하였다. 
 
 


<br/>

## 5. Process



<br/>

## 6. 프로젝트 팀원 및 담당 역할

**[팀원]**

- 학부생 3명

**[담당 역할]**

- 데이터 전처리 및 EDA
- 인사이트 도출
- 모델링&알고리즘 개발
- 발표 자료 제작

<br/>

## 6. 발표 자료

[HD-AI-CHALLENGE 본선 발표 자료](https://drive.google.com/file/d/1LucNwGaHszsWa-NIxNpl8cFeIRABim0f/view)  
