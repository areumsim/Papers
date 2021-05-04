# [RS] A new user similarity model to improve the accuracy of collaborative filtering

<br>

>**Title**: A new user similarity model to improve the accuracy of collaborative filtering <br> 
>**Authors**: Liu, H., Hu, Z., Mian, A., Tian, H., & Zhu, X.<br>
>**Year**:   2014 <br>
>**Journal**: Knowledge-Based Systems <br>
><br>
><br>
>**Read Period** : - 2019.08.01 ...

<br>
<br>
   
## Topic
+ Recommender systems , Collaborative filtering  <br>

<br>

## Probelms
+ 데이터가 희소한 경우, 기존 방식은 예측 정확도가 낮다.
또한, 추천결과를 생성할 때마다 매번 많은 연산이 필요하다.

+ Jaccard : 등급을 매긴 항목 수를 고려, 두 명의 사용자가 더 일반적인 평가 항목을 가질 경우 더 유사
+ ( 평가 절대 치는 고려하지 않음 )

<br>

## Motivation
+ 두 사용자 간의 공통 등급의 비율과 사용자의 등급 선호도를 고려한 

+ 본 논문은 두 사용자 간의 공통 등급(Jaccard)과 각 사용자의 글로벌 선호도(PSS)를 결합하여 
더 정확한 Heuristic(PSS, URP) Similarity Model을 제안 

<br>

## Proposed method
1. PSS  Proximity   : rating 간의 차이만 측정
        Significance: 중앙값에서 멀 수록 더 중요/의미가 큼
        Singularity : 두 값이 다른 값들과 얼마나 다른지
2. Jaccard’   공통 항목의 비율이 적으면 punish
3. URP (User rating Preference)  사용자의 평가 선호도 고려


## TODO 
식 이미지 첨부하기 

<br>
