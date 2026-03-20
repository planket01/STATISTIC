# 데이터분석 3주차 정규과제

📌데이터분석 정규과제는 매주 정해진 분량의 『*혼자 공부하는 데이터 분석 with 파이썬*』 을 읽고 학습하는 것입니다. 이번 주는 아래의 **DataAnalysis_3rd_TIL**에 나열된 분량을 읽고 공부하시면 됩니다.

아래의 문제를 풀어보며 학습 내용을 점검하세요. 문제를 해결하는 과정에서 개념을 스스로 정리하고, 필요한 경우 제시된 강의를 참고하여 보완하는 것이 좋습니다.

<!-- 강의 링크는 아래와 같습니다.
https://www.youtube.com/watch?v=CE3_InvbmLY&list=PLVsNizTWUw7FGzSRCkQrPEEe-ljVXgS7k&index=6
https://www.youtube.com/watch?v=hhbzUEQWdTg&list=PLVsNizTWUw7FGzSRCkQrPEEe-ljVXgS7k&index=7
-->


## DataAnalysis_3rd_TIL

### 3장 데이터 정제하기
#### 01. 불필요한 데이터 삭제하기
#### 02. 잘못된 데이터 수정하기


## Study Schedule

| 주차  | 공부 범위     | 완료 여부 |
| ----- | ------------- | --------- |
| 1주차 | p.24~81    | ✅         |
| 2주차 | p.84~151   | ✅         |
| 3주차 | p.154~219  | ✅         |
| 4주차 | p.222~279 | 🍽️         |
| 5주차 | p.282~325 | 🍽️         |
| 6주차 | p.328~379 | 🍽️         |
| 7주차 | p.382~430 | 🍽️         |

<br>

<!-- 여기까진 그대로 둬 주세요-->


# 1️⃣ 개념 정리 

## 01. 불필요한 데이터 삭제하기

- loc: 필요한 행/렬을 지정해서 그것들로만 이루어진 데이터프레임을 만들 수 있다.
- 원소별 비교를 통해 리스트와 비슷한 형식인 넘파이 불리언 형식을 출력할 수 있다.
- df.drop('제거 원하는 열', axis=l) axis=0(행)/l(열):을 제거
- drop에서 제거 원하는 열이 여러 개일 경우: df.drop([~,~,~~~~], axis=l)
- df.drop('제거 원하는 열', axis=l, inplace=True)를 하면, 해당 변수가 원하는 열이 없어진 꼴로 수정 후 저장된다.
- 결측치가 있는 열을 제거하고 싶으면 .dropna()를 하면 된다.
- 중복된 열을 제거: duplicated(subset=[~])이용
- 이를 이용해서 중복을 stack 쌓이는 것으로 인식해 groupby 함수를 통해 몇 개가 중복됐는지 알 수 있다.

## 02. 잘못된 데이터 수정하기

- 누락된 값의 개수를 확인하고, NaN이 아닌, string 타입으로 결측치임을 채워넣는다.(코딩 오류 방지)
- replace를 통해 한 번에 결측치를 원하는 것으로 바꿀 수 있다.
- 값을 수정하는 것은 일이 많기 때문에 정규식을 이용해 간단하게 진행하는 것을 배운다.
- 아래와 같은 매서드를 통해 정규식을 통해 다양한 상황을 처리 가능하다.
- <img width="1022" height="316" alt="image" src="https://github.com/user-attachments/assets/9191827f-07c9-4c72-86c0-b8ed7868e338" />
-



# 2️⃣ 수행 인증

<img width="1324" height="926" alt="image" src="https://github.com/user-attachments/assets/d1e8b2a3-23b7-4788-803b-9eec45ffdaa7" />
<img width="1724" height="836" alt="image" src="https://github.com/user-attachments/assets/cd891664-2134-48c6-af90-477726114ced" />
<img width="1330" height="856" alt="image" src="https://github.com/user-attachments/assets/bb629095-d8b9-46da-8e39-edaa77412317" />
<img width="1074" height="1044" alt="image" src="https://github.com/user-attachments/assets/aa29f030-4f6c-4fa3-8367-54cc868e3d0a" />
<img width="1214" height="952" alt="image" src="https://github.com/user-attachments/assets/c735039d-a79a-4419-baed-3fbee56fdf98" />
<img width="1742" height="846" alt="image" src="https://github.com/user-attachments/assets/f8806a2b-1f1b-43dc-b79d-cb2b9edb260c" />
<img width="1072" height="606" alt="image" src="https://github.com/user-attachments/assets/cc5e601d-4bb0-4193-9951-f671cb62ec93" />


<!-- 이번 주차에는 API를 발급받는 과정도 포함하여 첨부해주세요.-->


<br>
<br>

# 3️⃣ 확인 문제

## 문제 1.

> **🧚Q. 다음 두 데이터프레임 df1, df2를 합쳐서 데이터프레임 df3를 만들려고 합니다.**  
> 적절한 판다스 명령을 선택해주세요.

<table>
<tr>

<td>

### df1

| index | col1 | col2 |
|-------|------|------|
| 0     | x    | 5    |
| 1     | y    | 6    |
| 2     | z    | 7    |

</td>

<td>

### df2

| index | col3 | col4 |
|-------|------|------|
| 0     | x    | 50   |
| 1     | y    | 60   |
| 2     | w    | 70   |

</td>

<td align="center" valign="middle">

<h2> ➜ </h2>

</td>

<td>

### df3 (결과)

| index | col1 | col2 | col3 | col4 |
|-------|------|------|------|------|
| 0     | x    | 5.0  | x    | 50.0 |
| 1     | y    | 6.0  | y    | 60.0 |
| 2     | z    | 7.0  | NaN  | NaN  |
| 3     | NaN  | NaN  | w    | 70.0 |

</td>

</tr>
</table>

```
1️⃣ pd.merge(df1, df2)
2️⃣ pd.merge(df1, df2, how='left')
3️⃣ pd.merge(df1, df2, left_on='col1', right_on='col3', how='outer')
4️⃣ pd.merge(df1, df2, left_on='col1', right_on='col3', how='inner')
```

```
- 정답은 3번이다.
- 1,2번의 x,y는 다 채워져 있고 그 결과 3의 x,y도 다 채워져있다.
- 반변 1,2번에 각각 서로다른 z와 w가 있는데, 이들은 서로에게 서로 없는 데이터가 존재한다.
- 따라서 모두 다 표시하되, 없는 데이터를 NaN값으로 return하도록 how='outer';아마 합집합 how='inner'하면 겹치는 것만 나옴;교집합
- 그리고 이 모든게 1번은 col1, 2번은 col3을 기준으로 이루어졌으니 이를 명시해야 한다.
```



### 🎉 수고하셨습니다.
