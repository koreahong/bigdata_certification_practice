# 빅분기 실기 예제풀이

## 모델링 과정

1. 데이터수집
2. 데이터전처리
    - 환불금액 null -> 0으로 처리
    - 환불은 0에 해당하는 성별이 압도적으로 많음. -> 0,1로 전환방법 고려
    - 정규화
    - 원핫인코딩
3. 모델링
    - 랜덤포레스트
    - xgboost
    - lightgbm
    - 로지스틱회귀
    - 스태킹모델(랜덤포레스트,xgboost,lightgbm -> 로지스틱 회귀)
3. 결과
    - 데이터전처리 기본 + 랜던포레스트가 AUC값이 0.67로 가장 높음
