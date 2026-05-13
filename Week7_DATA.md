# 데이터분석 7주차 정규과제

📌데이터분석 정규과제는 매주 정해진 분량의 『*혼자 공부하는 데이터 분석 with 파이썬*』 을 읽고 학습하는 것입니다. 이번 주는 아래의 **DataAnalysis_7th_TIL**에 나열된 분량을 읽고 공부하시면 됩니다.

아래의 문제를 풀어보며 학습 내용을 점검하세요. 문제를 해결하는 과정에서 개념을 스스로 정리하고, 필요한 경우 제시된 강의를 참고하여 보완하는 것이 좋습니다.

<!-- 강의 링크는 아래와 같습니다.
https://www.youtube.com/watch?v=R3E4m8fqUSg&list=PLVsNizTWUw7FGzSRCkQrPEEe-ljVXgS7k&index=14
https://www.youtube.com/watch?v=W_cxRstQUk8&list=PLVsNizTWUw7FGzSRCkQrPEEe-ljVXgS7k&index=15
-->


## DataAnalysis_7th_TIL

### 7장 검증하고 예측하기
#### 01. 통계적으로 추론하기
#### 02. 머신러닝으로 예측하기


## Study Schedule

| 주차  | 공부 범위     | 완료 여부 |
| ----- | ------------- | --------- |
| 1주차 | p.24~81    | ✅         |
| 2주차 | p.84~151   | ✅         |
| 3주차 | p.154~219  | ✅         |
| 4주차 | p.222~279 | ✅         |
| 5주차 | p.282~325 | ✅         |
| 6주차 | p.328~379 | ✅         |
| 7주차 | p.382~430 | ✅         |

<br>

<!-- 여기까진 그대로 둬 주세요-->


# 1️⃣ 개념 정리 

## 01. 통계적으로 추론하기

- 모수검정: 표본을 이용해 모집단의 정보를 찾아내는 과정
- 중심극한정리: 표본 수가 많아지면 많아질 수록 샘플링 결과는 정규분포와 비슷해진다.
- 가설검정: 표본에 대한 정보를 사용해 모집단의 파라미터에 대한 가정을 검정하는 것
- 순열검정: 분포를 정규분포로 혹은 그 자체로 설정할 수 없을 때 하는 가정으로, 아래와 같은 방법으로 진행된다.
- <img width="834" height="456" alt="image" src="https://github.com/user-attachments/assets/b23c6f96-c5fc-4b15-9e7c-e713a836dcf8" />

## 02. 머신러닝으로 예측하기

- <img width="714" height="452" alt="image" src="https://github.com/user-attachments/assets/c72999a7-4ce7-4deb-a0d5-15e94883b630" />
- 이렇듯 머신러닝은 크게 지도학습과 비지도학습으로 나뉜다.
- 지도학습: 데이터에 있는 각 샘플에 대한 정답을 알고 있는 경우
- 비지도학습: 입력 데이터는 있지만 타깃이 없는 경우
- x값에 따른 y값을 구하고자 할 때 보통 선형회귀나 로지스틱회귀를 이용해 이를 도출한다.


# 2️⃣ 수행 인증

<img width="786" height="410" alt="image" src="https://github.com/user-attachments/assets/9501c32c-29dc-4bf6-9938-e06a19ccf947" />
<img width="1552" height="296" alt="image" src="https://github.com/user-attachments/assets/1159f611-d7f2-4746-b027-f2f1385f44bc" />
<img width="2686" height="1052" alt="image" src="https://github.com/user-attachments/assets/4c5b39e3-33c2-4a12-8fdf-c5ad1ed191ba" />
<img width="1314" height="634" alt="image" src="https://github.com/user-attachments/assets/ddf528d4-0c9e-49ba-a8b1-a0b18b30ce9f" />




<br>
<br>

# 3️⃣ 확인 문제

## 문제 1.

> **🧚Q. 어떤 표본의 크기가 충분히 크고(n ≥ 30), 모집단 분산을 알 수 없을 때 모평균에 대한 신뢰구간을 구하려고 한다.
이때 다음 설명 중 가장 적절한 것은 무엇인가?**

```
1️⃣ 표본의 크기가 충분히 크므로 중심극한정리에 의해 표본평균의 분포는 근사적으로 정규분포를 따른다.  
2️⃣ 모집단 분산을 모르므로 신뢰구간을 구할 수 없다.  
3️⃣ 표본이 30개 이상이면 항상 모집단도 정규분포를 따른다.  
4️⃣ 중심극한정리는 모집단이 정규분포일 때만 적용된다.
```

```
1번
```

## 문제 2.

> **🧚Q. 다음 중 순열검정(permutation test)에 대한 설명으로 가장 옳은 것은 무엇인가?**

```
1️⃣ 모집단이 정규분포를 따른다는 가정을 반드시 해야 한다.  
2️⃣ 표준점수(z-score)를 이용하여 유의확률을 계산하는 방법이다.  
3️⃣ 데이터의 라벨을 무작위로 섞어 귀무가설 하에서의 분포를 직접 구성하는 비모수적 검정 방법이다.  
4️⃣ 표본의 크기가 충분히 클 때만 사용할 수 있다.
```

```
3번
```



### 🎉 수고하셨습니다.
