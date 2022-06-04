# 🔍Introduction
<img src = "images/intro.png" >


#### 배경
- KNOW는 다양한 직업에 종사하고 있는 재직자에 대하여 직무관련 조사를 수행하고 있다. 
- 본 KNOW 데이터를 기반으로 직업추천 모델을 만들어보고 직업과 연관성 높은 직무능력을 탐색 발굴하고자 한다.
#### 목적
- KNOW(한국직업정보) 설문 데이터셋을 활용한 직업 추천 알고리즘 개발
- 직업과 연관이 높은 설문지 문항 분석 및 영향변수 발굴
#### 주최 / 주관
- 주최 : 한국고용정보원  /  주관 : 데이콘


#### 리더보드
- Eval Metric : Macro F1-score
- Public Score : 전체 테스트 데이터 중 33% / Private Score : 전체 테스트 데이터 중 67%

#### 최종 순위
### 🎖 3rd Prize
<br/>



# 🗂 Data Set
<img src = "images/dataset.png" >

- 전체 데이터셋 row 약 4만개, column 갯수 약 160개

### Features
- Likert 5, 7점 척도 기반의 설문
<img src = "images/5point2.png" >

- 주관식 질문
<img src = "images/text2.png"   >

### Target 
- 약 600개의 직업코드 
<img src = "images/targets.png" >



# 🧑‍💻Model

<img src = "images/result.png">

- Tabluar Data : Categorical Data가 많은 설문조사 데이터이기때문에 CatBoost 모델 사용
- Text Data : Keyword 중심의 단어들이 많아 LSTM보다 1D-CNN 모델이 더 높은 성능을 보임



