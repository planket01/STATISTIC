# SQL_BASIC 6주차 정규 과제 

📌SQL_BASIC 정규과제는 매주 정해진 분량의 `초보자를 위한 BigQuery(SQL) 입문` 강의를 듣고 간단한 문제를 풀면서 학습하는 것입니다. 이번주는 아래의 **SQL_Basic_6th_TIL**에 나열된 분량을 수강하고 `학습 목표`에 맞게 공부하시면 됩니다.

**6주차 과제는 강의 내용을 정리하는 것과 함께, 프로그래머스에서 제공하는 SQL 문제를 직접 풀어보는 실습도 병행합니다.** 강의에서는 **배운 내용을 정리하고 주요 쿼리 예제를 정리**하며, 프로그래머스 문제는 **직접 풀어본 뒤 풀이 과정과 결과, 배운 점을 함께 기록**해주세요. 완성된 과제는 Github에 업로드하고, 링크를 스프레드시트 'SQL' 시트에 입력해 제출해주세요.

**👀(수행 인증샷은 필수입니다.)** 

## SQL_BASIC_6th

### 섹션 6. 다량의 자료를 연결 : JOIN 

### 5-1. Intro

### 5-2. JOIN 이해하기

### 5-3. 다양한 JOIN 방법

### 5-4. JOIN 쿼리 작성하기 

### 5-5. JOIN을 처음 공부할 때 헷갈렸던 부분

### 5-6. JOIN 연습문제 1~2번

### 5-6. JOIN 연습문제 3~5번

### 5-7. 정리



## 🏁 강의 수강 (Study Schedule)

| 주차  | 공부 범위              | 완료 여부 |
| ----- | ---------------------- | --------- |
| 1주차 | 섹션 **1-1** ~ **2-2** | ✅         |
| 2주차 | 섹션 **2-3** ~ **2-5** | ✅         |
| 3주차 | 섹션 **2-6** ~ **3-3** | ✅         |
| 4주차 | 섹션 **3-4** ~ **4-4** | ✅         |
| 5주차 | 섹션 **4-4** ~ **4-9** | ✅         |
| 6주차 | 섹션 **5-1** ~ **5-7** | ✅         |
| 7주차 | 섹션 **6-1** ~ **6-6** | 🍽️         |

<!-- 여기까진 그대로 둬 주세요-->

<br>

---

# 1️⃣ 개념정리

## 5-2. JOIN 이해하기

~~~
✅ 학습 목표 :
* JOIN에 대한 정의와 필요성에 대해 설명할 수 있다.
~~~

두 데이터의 공통값이 있을 수도 있고, 아닐 때도 있는데 보통 ~~id를 확인하면 된다.(key)
-> 트레이너가 포획한 포켓몬을 기준으로 연결할 예정이고, 그러면 오른쪽에 새로운 컬럼이 추가된다.
join해서 그대로 쓰기 보다는 필요한 것만 분석할 수 있게 조작해 다룬다.

## 5-3. 다양한 JOIN 방법

~~~
✅ 학습 목표 :
* JOIN 방법들의 종류를 설명할 수 있다. 
* 각 JOIN 방법들의 차이점에 대해서 설명할 수 있다. 
~~~

inner: 공통 요소만 연결
left/right outer: 왼/오른쪽으로 테이블 기준으로 연결
full outer: 양쪽 기준으로 연결
cross : 두 테이블의 요소들을 곱함
<img width="1856" height="928" alt="image" src="https://github.com/user-attachments/assets/4324530e-4be9-41c9-9541-b1bd6c24b19d" />


## 5-4. JOIN 쿼리 작성하기 

~~~
✅ 학습 목표 :
* JOIN을 사용한 문법에 대해 이해하여 적용할 수 있다.
* JOIN 을 활용한 쿼리를 작성할 수 있다. 
~~~

<img width="1212" height="708" alt="image" src="https://github.com/user-attachments/assets/c1ace38c-855b-4136-bd4b-53a5f3c71d56" />
- 한 결과
- <img width="808" height="530" alt="image" src="https://github.com/user-attachments/assets/7dfa0b02-7f97-4c77-a08b-1f546653d096" />
-  .*exept(~): joint 할 때 제외할 컬럼 지



## 5-6. JOIN 연습문제 1~5번 

~~~
✅ 학습 목표 :
* 연습문제(3문제 이상) 푼 것들 정리하기
~~~

<img width="778" height="474" alt="image" src="https://github.com/user-attachments/assets/564321de-c573-4b7c-b92b-0ead835ba73c" />
<img width="804" height="334" alt="image" src="https://github.com/user-attachments/assets/9e9fb893-98b4-4490-9516-c0f2e1f5fe37" />
<img width="920" height="290" alt="image" src="https://github.com/user-attachments/assets/1f459f15-0573-4277-bb16-4b5cbd7d402f" />


<br>

<br>

---

# 2️⃣ 확인문제 & 문제 인증

## 프로그래머스 문제 

https://school.programmers.co.kr/learn/courses/30/lessons/131533

> 상품 별 오프라인 매출 구하기

https://school.programmers.co.kr/learn/courses/30/lessons/133027

> 주문량이 많은 아이스크림들 조회하기

- 문제1
<img width="1174" height="982" alt="image" src="https://github.com/user-attachments/assets/eab2a3a6-0b15-4fa5-8582-7a2dadfa61a8" />
- 매출액은 SUM(P.PRICE * S.SALES_AMOUNT)이니 두 데이터에서 각각 가격과 수량을 곱해야 하는 문제이다.
- GROUP BY, ORDER BY를 사용해 매출액을 기준으로 내림차순 정렬해주시고 매출액이 같다면 상품코드를 기준으로 오름차순 정렬하는 것꺼지
- 모든 조건을 맞추는 것이 복잡했다.
- 복잡한 문제 상황도 차근차근 한다면 표현 가능함을 알 수 있다.

- ㅇ
- 문제2
<img width="1488" height="1100" alt="image" src="https://github.com/user-attachments/assets/b4c419c1-ec6c-4040-b893-82caaba57df5" />
- 문제가 매우 복잡하여 어떻게 풀어야할지 잘 몰랐다.
- 제일 많은 것을 순서대로 3개만 필요로 하니 limit도 이용해야 한다.
- 가장 어려운 부분은 join 안을 어떻게 채우는지를 결정하는 과정이었다.


---

# 3️⃣ 참고자료

JOIN 에 대해서 그림으로 쉽게 이해할 수 있는 자료들도 있어서 첨부합니다. 아래의 블로그도 학습할 때 같이 참고해주세요.

1. https://data-marketing-bk.tistory.com/entry/SQL-JOIN-%ED%95%9C-%EB%B0%A9%EC%97%90-%EC%A0%95%EB%A6%AC-%EA%B0%9C%EB%85%90%EB%B6%80%ED%84%B0-%EC%BD%94%EB%93%9C%EA%B9%8C%EC%A7%80-%EC%9D%B4%EA%B2%83%EB%A7%8C-%EB%B3%B4%EC%9E%90



2. https://velog.io/@wijoonwu/JOIN

<br>

### 🎉 수고하셨습니다.
