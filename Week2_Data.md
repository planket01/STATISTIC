# 데이터분석 2주차 정규과제

📌데이터분석 정규과제는 매주 정해진 분량의 『*혼자 공부하는 데이터 분석 with 파이썬*』 을 읽고 학습하는 것입니다. 이번 주는 아래의 **DataAnalysis_2nd_TIL**에 나열된 분량을 읽고 공부하시면 됩니다.

아래의 문제를 풀어보며 학습 내용을 점검하세요. 문제를 해결하는 과정에서 개념을 스스로 정리하고, 필요한 경우 제시된 강의를 참고하여 보완하는 것이 좋습니다.

<!-- 강의 링크는 아래와 같습니다.
https://www.youtube.com/watch?v=s_-VvTLb3gs&list=PLVsNizTWUw7FGzSRCkQrPEEe-ljVXgS7k&index=4
https://www.youtube.com/watch?v=Il6L8OtNFpc&list=PLVsNizTWUw7FGzSRCkQrPEEe-ljVXgS7k&index=5
-->


## DataAnalysis_2nd_TIL

### 2장 데이터 수집하기
#### 01. API 사용하기
#### 02. 웹 스크래핑 사용하기


## Study Schedule

| 주차  | 공부 범위     | 완료 여부 |
| ----- | ------------- | --------- |
| 1주차 | p.24~81    | ✅         |
| 2주차 | p.84~151   | ✅         |
| 3주차 | p.154~219  | 🍽️         |
| 4주차 | p.222~279 | 🍽️         |
| 5주차 | p.282~325 | 🍽️         |
| 6주차 | p.328~379 | 🍽️         |
| 7주차 | p.382~430 | 🍽️         |

<br>

<!-- 여기까진 그대로 둬 주세요-->


# 1️⃣ 개념 정리 

## 01. API 사용하기

- 통신규약인 HTTP: 웹브라우저(내 컴퓨터)에서 HTTP을 통해 데이터를 요청하면, 웹서버(네이버,구글 등)는 HTML을 웹브라우저에게 전달한다.
- 이때 받는 데이터는 CSV, JSON, XML에 등 HTML이 아닌 형식으로 온다.
- JSON(JavaScript Object Notation): {"~~": "~"} 형식이다.
- JSON을 데이터프레임 형식으로도 바꿀 수 있다. 이외 다양한 것들은 실습 참고
- XML(extensible Markup Language): 시작과 종결 태그를 통해 이해하기 쉬운 구조로 이루어져있다.
- 부모.자식 처럼 계층적인 구조라는 특징이 있다.
- 다만 자식 엘리먼트 순서는 고정된 것이 아니기 때문에 book 객체의 findtextO 메서드를 사용해야 한다.
- 여러 자신 엘리먼트에서 동일 이름인 것을 찾을 때는 findall,for문을 사용한다.

## 02.웹 스크래핑 사용하기

- API로 제공하지 않는 데이터를 수집할 때 유용하다.
- gdown 패키지를 사용해 코랩으로 다운할 수 있다. -> 이후에는 데이터프레임을 다루는 것과 동일하다.
- loc함수를 사용해 데이터를 추출 할 때, :을 이용할 수 있지만, 끝지점도 포함된다는 것에 유의하자.
- 뷰티플수프: HTML 안에 있는 내용을 찾아주는 기능을 한다. 이때 원하는 데이터가 HTML 어디에 위치해 있는지 알아야한다.


# 2️⃣ 수행 인증

<img width="528" height="328" alt="image" src="https://github.com/user-attachments/assets/02f37bb7-1ee9-4251-99d6-9c470a8c2f7f" />
<img width="2010" height="1186" alt="image" src="https://github.com/user-attachments/assets/f5aa483b-0776-4ed0-b0c8-1c8839f6caa1" />
<img width="2488" height="1176" alt="image" src="https://github.com/user-attachments/assets/c415e924-dbdd-424c-bba6-fd04b7558741" />
<img width="1774" height="1132" alt="image" src="https://github.com/user-attachments/assets/cfdb4228-a1a7-4736-bef1-440b627a2592" />
<img width="1600" height="1164" alt="image" src="https://github.com/user-attachments/assets/c34117bb-65ac-4769-b2b8-1c1277828b2c" />
<img width="1570" height="984" alt="image" src="https://github.com/user-attachments/assets/a228ca21-a04b-40bd-b509-13783146dcde" />


<br>
<br>

# 3️⃣ 확인 문제

## 문제 1.

> **🧚Q. 다음 중 BeautifulSoup 외에 웹 스크래핑에 사용할 수 있는 파이썬 패키지로 가장 적절한 것은 무엇인가요?**

```
1️⃣ NumPy  
2️⃣ Scrapy  
3️⃣ Matplotlib  
4️⃣ Scikit-learn  
```

```
2️⃣ Scrapy
나머지 선택지들은 머신러닝, EDA 등에 사용되는 패키지고, Scrapy는 requests와 뷰티플스프를 합친것과 같다고 책에서 소개했다.(125p)
```



### 🎉 수고하셨습니다.
