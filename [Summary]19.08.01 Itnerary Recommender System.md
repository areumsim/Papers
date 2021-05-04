# [RS] Itinerary recommender system with semantic trajectory pattern mining from geo-tagged photos

<br>

>**Title**: Itinerary recommender system with semantic trajectory pattern mining from geo-tagged photos <br> 
>**Authors**: Cai, G., Lee, K., & Lee, I<br>
>**Year**: 2018 <br>
>**Journal**: Expert Systems with Applications <br>
><br>
><br>
>**Read Period** : 19.08. 

<br>
<br>
    
    
## Topic
+ Recommendation System  <br>

<br>

## Probelms
+ 기존의 여행 코스 추천 시스템은 여행지 위치(인기 PoI, 이동 편리)와 여행 기간에만 기반하여 일정 추출 <br>

<br>

## Motivation
+ SNS상에 업로드 된 대량의 Geo-tagged photo를 기반으로 기존에 사용되던 지리적인 공간 정보 이외에,<br>
장소 유형, 기상 조건, 여행 기간 등 비공간적 정보를 추가로 고려하여 일정 추천
 <br>


<br>

## Proposed method
+ **(Def1) A trajectory**	: 시간정보를 가진 위치 좌표의 시퀀스 <br>
     T = < (x1, y1, t1), (x2, y2, t2), …  > <br>
+ **(Def2) Semantic Trajectory** : 장소 유형과 더불어 추가적인 의미 주석을 가진, 위치 좌표의 시퀀스  <br>
      SemT = < (SemA0, t0) , (SemA1 , t1) , … > <br>
     ( SemAi = (ei , Vi)   where  ei = set of basic sematic,  Vi = additional set of semantic annotation ) <br>
+ **(Def3) SemT-Pattern = (SemS , A)** : 의미요소를 가진 위치 좌표 시퀀스와 시간정보 <br>
     SemS = < (SemA0) , (SemA1) , …  >	: 의미 요소의 연속 <br>
      A = < α1, α2 , … >		: 두 방문 장소 사이의 시간간격 <br>
    
 <img src="https://user-images.githubusercontent.com/31869418/73640937-8227f080-46b2-11ea-9a57-e3d24342cd72.png" height="500"> <br>

<br>

## Experiments
+ Our method :  1404개의 궤적, 12개의 유형의 49개의 PoI,  <br>
      65개의 basic semantic trajectory pattern, 대부분 길이가 2-4 <br>
+ Baseline method : DBSCAN clustering으로 사용자수 기반, 17개 유형의 46개의 PoI <br>
 <br>
+ a testing dataset of 300 simulated travel routes   <br>
  • 300개 이동 경로 포함;  <br>
  • 총 22가지 고유 유형 포함  <br>
  • 거의 절반에 가까운 경로는 2개의 고유 유형을 포함  <br>
 <br>
+ Positive : 여행 일정의 후보와 사용자의 쿼리 유형 간의 일치율 <br>
Common type 의 Percentage :  perk = y/k   ( where  x : unique type , y : common type )  <br>

![image](https://user-images.githubusercontent.com/31869418/73640545-c5359400-46b1-11ea-92ba-3e6f8037b268.png)  <br>

<br>

## Conclusion
더 많은 의미론적 DB를 구축하여 통합 <br>
시스템에 대한 검증을 위하여 여행사 기반의 추천 일정과 비교 <br>
‘거부’와 같은 다양한 사용자 제약을 추가 <br>
추천 일정에 사진 이미지를 추가 <br>

Photo의 사람인식을 통해 연령 별, 여행 그룹 별 분석 및 추천 가능 <br>
SNS 업로드 된 이미지는 일부 사용자 계층에 편중될 가능성이 높음 <br>
사용자의 이전 여행 기록에 동행 및 목적 등 추가 제약 조건을 적용하는 것이 필요 <br>

<br>

## References
+ 

<br>

<br>
