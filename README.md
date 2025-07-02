# 📊 Numpy 기초 및 활용 레포트

---

## 📚 목차

1. [Numpy 소개 및 설치](#1-numpy-소개-및-설치)
2. [배열 생성 및 속성](#2-배열-생성-및-속성)
3. [배열 연산](#3-배열-연산)
4. [인덱싱 및 조건 필터링](#4-인덱싱-및-조건-필터링)
5. [배열 구조 변경 및 병합](#5-배열-구조-변경-및-병합)
6. [통계 및 수학 함수](#6-통계-및-수학-함수)
7. [실전 예제](#7-실전-예제)
8. [실행 방법](#8-실행-방법)
9. [참고자료](#9-참고자료)

---

## 1. Numpy 소개 및 설치

- **Numpy란?**  
  Numpy는 Python에서 고성능 수치 계산을 위한 핵심 라이브러리입니다.  
  다차원 배열 객체와 배열 기반의 수학 함수 등을 제공합니다.

- **설치 방법**  
  ```bash
  pip install numpy

2. 배열 생성 및 속성
배열 생성 함수

python
복사
편집
import numpy as np

np.array([1, 2, 3])
np.zeros((2, 3))
np.ones((3, 3))
np.arange(0, 10, 2)
np.linspace(0, 1, 5)
배열 속성 확인

python
복사
편집
a = np.array([[1, 2, 3], [4, 5, 6]])
a.shape       # 배열 형태
a.ndim        # 차원 수
a.size        # 전체 요소 수
a.dtype       # 자료형
3. 배열 연산
기본 연산 (브로드캐스팅 지원)

python
복사
편집
a + b
a - b
a * b
a / b
수학 함수

python
복사
편집
np.sqrt(a)
np.exp(a)
np.log(a)
np.sin(a)
4. 인덱싱 및 조건 필터링
인덱싱과 슬라이싱

python
복사
편집
a[0, 1]
a[:, 0]
a[1:3, :]
조건 필터링

python
복사
편집
a[a > 5]
a[(a % 2) == 0]
5. 배열 구조 변경 및 병합
배열 구조 변경

python
복사
편집
a.reshape(3, 2)
a.ravel()
a.T  # 전치
병합과 분할

python
복사
편집
np.hstack((a, b))
np.vstack((a, b))
np.split(a, 2)
6. 통계 및 수학 함수
통계 함수

python
복사
편집
np.mean(a)
np.median(a)
np.std(a)
np.var(a)
np.sum(a)
np.max(a)
np.min(a)
np.argmax(a)
np.argmin(a)
7. 실전 예제
이미지 처리

python
복사
편집
from matplotlib import image
img = image.imread('sample.png')
print(img.shape)  # (높이, 너비, 채널)
선형대수

python
복사
편집
A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])
np.dot(A, B)
np.linalg.inv(A)
np.linalg.eig(A)
8. 실행 방법
bash
복사
편집
pip install -r requirements.txt
jupyter notebook
9. 참고자료
📘 Numpy 공식 문서

📙 Python 데이터 사이언스 핸드북 - Jake VanderPlas

📗 Kaggle Python Numpy 튜토리얼
