# DACON_KBO-Batter-OPS-Predict-Contest

해당 공간은 [DACON 타자 OPS 예측 대회](https://dacon.io/competitions/official/62540/overview/)에 참여한 코드를 저장하기 위한 공간입니다.

해당 코드에 대한 저작권은 시로앤마로(안지민, 이인섭, 이형선, 주은혁)에게 있습니다.

주관 : [데이콘](https://dacon.io) / 주최 : KBO

## 대회 설명

역대 KBO 타자들의 정규시즌 등 게임 데이터를 활용하여 2019년 타자들의 상반기 성적 예측을 목표로 합니다.


## 데이터 설명

### 제공 데이터
* Regular_Season_Batter.csv : KBO에서 활약한 타자들의 역대 정규시즌 성적을 포함하여 몸무게, 키 ,생년월일 등의 기본정보
* Regular_Season_Batter_Day_by_Day.csv: KBO에서 활약한 타자들의 일자 별 정규시즌 성적
* Pre_Season_Batter.csv : KBO에서 활약한 타자들의 역대 시범경기(정규시즌 직전에 여는 연습경기) 성적

### 산출 데이터

* salary.csv : 타자들의 연봉 크롤링 정보(크롤링 코드가 존재 X)
* dt.csv : 구장정보에 대한 반복문을 돌린 값

### 최종 데이터
* submission.csv : 참가자들이 예측해야 할 타자의 이름과 아이디 목록

## 데이터 처리 과정

데이터 전처리 - 변수 선택(Feature Engineering) - 모델링 - 결론

### Feature Engineering
* career : 해당 시즌의 선수 연차
* g_age : 해당 시즌의 선수 나이
* s1 ~ 9 : 해당 경기 구장 정보
* salary : 해당 시즌의 선수 연봉
* transfer : 선수 이적 여부

## 모델링

* Linear Model : 선형 회귀 모형
* RandomForest : 랜덤 포레스트

## 후기

처음 출전한 공모전으로서, 상반기 야구 경기가 매일 진행되면서 점수가 업데이트되는 점이 흥미로웠음.

야구에 대한 도메인 지식을 쌓을 수 있었고, 머신러닝에 대해 공부하게 된 계기가 되었음.

## 결과

![최종결과](./image/최종 결과.PNG)

최종 4등으로서 수상을 하지 못하였지만, 이어지는 KBO 타자 OPS 시각화 대회 참가 혜택 받음.

