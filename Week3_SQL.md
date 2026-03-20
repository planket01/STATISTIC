# SQL_BASIC 3주차 정규 과제 

📌SQL_BASIC 정규과제는 매주 정해진 분량의 `초보자를 위한 BigQuery(SQL) 입문` 강의를 듣고 간단한 문제를 풀면서 학습하는 것입니다. 이번주는 아래의 **SQL_Basic_3rd_TIL**에 나열된 분량을 수강하고 `학습 목표`에 맞게 공부하시면 됩니다.

**3주차 과제는 문제 풀이를 중심으로**, 강의에서 제시된 예제 문제 중 **7 문제 이상을 선택하여 직접 풀어본 뒤**, 강의 영상의 풀이와 비교해 **틀린 부분, 맞은 부분, 새롭게 배운 개념**을 구체적으로 정리해주세요. (적어도 3문제는 정리해야 합니다.) 완성된 과제는 Gihub에 업로드하고, 링크를 스프레드시트 'SQL' 시트에 입력해 제출해주세요.

**👀(수행 인증샷은 필수입니다.)** 

## SQL_BASIC_3rd

### 섹션 3. 데이터 탐색 - 조건, 추출, 요약

### 2-6. 연습문제 1~3번

### 2-6. 연습문제 7~9번

### 2-6. 연습문제 10~12번

### 2-6. 연습문제 13~17번

### 2-7. 정리 

### 2-8. 새로운 집계함수



## 섹션 4. 쿼리 잘 작성하기, 쿼리 작성 템플릿 및 오류를 잘 디버깅하기

### 3-1. INTRO

### 3-2. SQL 쿼리 작성하는 흐름

### 3-3. 쿼리 작성 템플릿과 생산성 도구 



## 🏁 강의 수강 (Study Schedule)

| 주차  | 공부 범위              | 완료 여부 |
| ----- | ---------------------- | --------- |
| 1주차 | 섹션 **1-1** ~ **2-2** | ✅         |
| 2주차 | 섹션 **2-3** ~ **2-5** | ✅         |
| 3주차 | 섹션 **2-6** ~ **3-3** | ✅         |
| 4주차 | 섹션 **3-4** ~ **4-4** | 🍽️         |
| 5주차 | 섹션 **4-4** ~ **4-9** | 🍽️         |
| 6주차 | 섹션 **5-1** ~ **5-7** | 🍽️         |
| 7주차 | 섹션 **6-1** ~ **6-6** | 🍽️         |

<br>

<!-- 여기까진 그대로 둬 주세요-->

---

# 1️⃣ 개념정리

## 2-6. 연습문제

~~~
✅ 학습 목표 :
* 연습문제(7문제 이상) 푼 것들 정리하기
~~~
- 1번 문제
- <img width="656" height="850" alt="image" src="https://github.com/user-attachments/assets/ecc99103-4744-403b-b4e3-c4501d1c8f3f" />
- IS NULL이라는 것을 새로 배웠다.
- 2번 문제
- <img width="888" height="1018" alt="image" src="https://github.com/user-attachments/assets/575c6375-ec42-4f21-ad25-f128a839819b" />
- 여기서 계속 오류가 났었는데, 집계하는 기준이 있다면 그 기준을 GROUP BY 해줘야 한다는 것을 알 수 있었다.
- 이전에 배웠지만 까먹었던 내림차순도 기억할 수 있어 좋았다.
- 3번 문제
- <img width="876" height="784" alt="image" src="https://github.com/user-attachments/assets/9b6e09f4-156c-4709-94a8-1fd9cf31d778" />
- 2번 문제에서 type2가 없어야 한다는 조건만 빼면 되기에 쉽게 맞췄다.
- DISTINCT 라는 것을 알려줬는데, 이 자료는 다 중복이 없었기 때문에 결과가 같았지만, 만약 같은 자료가 섞여있다면 이를 써봐야 할 것이다.
- 4번 문제
- <img width="664" height="780" alt="image" src="https://github.com/user-attachments/assets/8afa7f26-a3ff-4c6d-bd35-e7b189ed228d" />
- 다른점: is_legendary를 썼느냐 차이가 있는데 이것이 있는 것이 뭐가 어떤건지 보기에 좋은 것 같다.
- 5번 문제
- <img width="672" height="298" alt="image" src="https://github.com/user-attachments/assets/0bf458ed-dea9-4544-9bc2-b3c5916e92ab" />
- 집계 후 조건인 HAVING을 앞에 정리한 것을 토대로 기억해냈고, 덕분에 한 번에 맞출 수 있었다.
- 6번 문제
- <img width="576" height="228" alt="image" src="https://github.com/user-attachments/assets/00c27907-5f73-4218-b292-aaaf8f45fe3a" />
- 쉬운 문제였다.
- 7번 문제
- <img width="712" height="224" alt="image" src="https://github.com/user-attachments/assets/658f45e2-f7fc-4cf7-9940-8da46e032c92" />
- WHERE name IN ('Iris', 'Whitney', 'Cynthia')이라는 IN 조건을 통해 OR등 반복하는 작업을 줄인다는 것을 배웠다.
- 9번 문제
- <img width="574" height="224" alt="image" src="https://github.com/user-attachments/assets/f00974fa-7936-4005-815c-1e95e23e6dbe" />
- 쉬운 문제다.
- 11번 문제
- <img width="614" height="318" alt="image" src="https://github.com/user-attachments/assets/040a349c-1164-4c38-8bcf-25a86191c9de" />
- 처음에는 MAX를 쓰는줄 알고 계속 오류 떠서 풀이를 보니 ORDERED BY와 LIMIT을 써야한다는 것을 알게됐다.
- 12번 문제
- <img width="644" height="332" alt="image" src="https://github.com/user-attachments/assets/2180d6db-f159-40a0-aab4-210ce799aa9a" />
- 11번 문제의 NOT NULL을 NULL로만 바꾸면 된다.
- 13번 문제
- <img width="626" height="238" alt="image" src="https://github.com/user-attachments/assets/1074b3b4-6c52-4700-8a9c-6d4118c1f59e" />
- LIKE라는 것을 처음 봤고, 단어를 찾는데 유용한 기능을 가진다.
- 14번 문제
- <img width="652" height="222" alt="image" src="https://github.com/user-attachments/assets/a3239b01-9b04-4ea1-b7b7-e82f602ced33" />
- 쉽다.
- 17번 문제
- <img width="724" height="226" alt="image" src="https://github.com/user-attachments/assets/c689e8b5-16af-43cf-9991-84e4766d801e" />
- 매우 어렵다.
- <img width="1858" height="916" alt="image" src="https://github.com/user-attachments/assets/867513ff-1c61-45fc-bfad-93db44354923" />
- 정리하면 위와 같은 사진과 같다.


## 2-8. 새로운 집계함수

~~~
✅ 학습 목표 :
* SQL 쿼리 구조를 이해할 수 있다. 
* SELECT, FROM, WHERE을 활용하는 방법을 설명할 수 있다. 
~~~

- GROUP BY ALL이라는 것이 추가됐는데, 이는 기존에 GROUP BY에서 일일이 손으로 썼다면, 이는 자동 판단되어 정리되는 장점이 있다.



## 3-2. 쿼리를 작성하는 흐름

~~~
✅ 학습 목표 :
* 쿼리를 작성하는 흐름을 설명할 수 있다.
~~~

- 데이터가 어떤 것을 해결하기 위해 쓰일 것인지를 생각하는 지표 정의를 하고
- 원하는 결과를 명확하게 표현할 수 있게 확실하게 변수 이름을 지어야 한다.
- 지표 탐색: 비슷한 문제를 풀었던 사례를 찾아본다.
- 만약 유사한 사례가 없다면 직접 쿼리를 생성하고, 있다면 그것을 이용하는 것이 좋다.
- 만약 테이블이 여러 개라면 연결방법을 고민해야 한다.
- 이후 깔끔하게 정리해 결과가 맞는지 확인하고 문서로 저장한다.



## 3-3. 쿼리 작성 템플릿과 생산성 도구

~~~
✅ 학습 목표 :
* 생산성 도구를 만들 수 있다.
~~~

<!-- 이어질 주차에서 생산성 도구를 활용한 실습이 있습니다.강의에 맞게 제작하여 화면을 캡쳐하여 이 주석을 지우고 올려주세요. -->
- 보통 탬플릿을 활용하기 불편하기에 사용하지 않는 경우가 많다. -> 습관이 형성되지 않음
- 이를 해결할 수 있는 것이 생산형 AI를 사용하는 것이다.
<img width="1396" height="606" alt="image" src="https://github.com/user-attachments/assets/798eb76c-8e60-42df-83dd-ecbd609996a4" />
<img width="1050" height="376" alt="image" src="https://github.com/user-attachments/assets/b8f43d5b-f5e5-4a92-88f5-f14c7fca2ec1" />




<br>
<br>

---

# 2️⃣ 학습 인증란

<img width="854" height="742" alt="image" src="https://github.com/user-attachments/assets/9181029f-0101-4a16-b734-4c41fb9bbb5f" />
<img width="1946" height="1458" alt="image" src="https://github.com/user-attachments/assets/10f8c00d-9071-4fcf-a2cf-da319b92d3e4" />





<br><br>



---

# 3️⃣ 확인문제

## 문제 1

> **🧚Q. Q. 포켓몬 연구에 흥미를 느낀 혜인은 각 타입(type1)별 평균 공격력(attack)을 비교해보고 싶었습니다.**
>
> 그래서 다음과 같은 필요한 정보를 미리 정리해보았습니다. 

~~~
조건 : attack이 50 이상인 포켓몬만 포함
보고 싶은 컬럼 : type1
집계 내용 : 각 type1 별 평균 공격력
정렬 기준 : 평균 공격력을 기준으로 내림차순 정렬
~~~

> **이 목표를 바탕으로 혜인은 아래와 같은 쿼리를 작성했지만, 일부 SQL 문법 요소를 빼먹었습니다. 비어 있는 부분인 ㄱ, ㄴ, ㄷ, ㄹ 에 들어갈 알맞은 SQL 구문을 채워보세요:**

~~~sql
SELECT type1, (ㄱ)
FROM pokemon
(ㄴ) attack >= 50
(ㄷ) type1
ORDER BY (ㄱ) (ㄹ);
~~~



~~~
SELECT type1, SUM(attack)/COUNT(id) as avg_at
FROM pokemon
WHERE attack >= 50
GROUP BY type1
ORDER BY avg_at DESC;
~~~



### 🎉 수고하셨습니다.
