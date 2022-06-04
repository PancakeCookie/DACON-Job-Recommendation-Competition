# Intro
<img src = "images/intro.png" >


#### 배경
- KNOW는 다양한 직업에 종사하고 있는 재직자에 대하여 직무관련 조사를 수행하고 있다. 
- (2017년 : 일반업무활동, 2018년 : 업무환경 및 흥미, 2019년 : 지식 및 성격, 2020년 : 업무수행능력 및 가치관)
- 본 KNOW 데이터를 기반으로 직업추천 모델을 만들어보고 직업과 연관성 높은 직무능력을 탐색 발굴하고자 한다.
#### 목적
- KNOW(한국직업정보) 설문 데이터셋을 활용한 직업 추천 알고리즘 개발
- 직업과 연관이 높은 설문지 문항 분석 및 영향변수 발굴
#### 주최 / 주관
- 주최 : 한국고용정보원  /  주관 : 데이콘


#### 리더보드
- Eval Metric : Macro F1-score
- Public Score : 전체 테스트 데이터 중 33%
- Private Score : 전체 테스트 데이터 중 67%

#### 최종 순위
- 🎖 **3rd**

# Data Set
<img src = "images/data set.png">

- 2017년 : 응답자수 9486 row, 질문 개수 156 column 
- 2018년 : 응답자수 9072 row, 질문 개수 141 column
- 2019년 : 응답자수 8555 row, 질문 개수 153 column
- 2020년 : 응답자수 8122 row, 질문 개수 185 column


**Features: Likert 5점 척도 기반의 설문 + 주관식 답변** 

**Target: 약 600개의 직업 class**


# Model

<img src = "images/exp results.png">

- Tabluar Data : Categorical Data가 많은 설문조사 데이터이기때문에 CatBoost 모델 사용
- Text Data : Keyword 중심의 단어들이 많아 LSTM보다 1D-CNN 모델이 더 높은 성능을 보임



