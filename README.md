# bottom_up_ml

『밑바닥부터 시작하는 딥러닝』 시리즈를 따라가며 딥러닝·머신러닝의 핵심 개념을
프레임워크 없이 NumPy로 직접 구현하고 정리한 **학습용 저장소**입니다.

이론 정리(마크다운 셀)와 예제 구현(코드 셀)을 Jupyter Notebook에 함께 담아,
개념 → 수식 → 코드 순으로 밑바닥부터 쌓아 올리는 방식으로 공부했습니다.

## 작업 기간

**2024년 1월 5일 ~ 1월 22일** (약 3주간, 총 10개 커밋)

| 날짜 | 내용 |
|------|------|
| 2024-01-05 | 딥러닝1 - chapter 4(신경망 학습), chapter 5(오차역전파법) |
| 2024-01-08 | 딥러닝1 - chapter 6(학습 관련 기술), chapter 7(CNN) |
| 2024-01-10 | 딥러닝2 - chapter 2(단어의 분산 표현) |
| 2024-01-12 | 딥러닝2 - chapter 3(word2vec) |
| 2024-01-15 | 딥러닝2 - chapter 5(RNN), chapter 6(LSTM) |
| 2024-01-19 | 차분 진화(Differential Evolution) 알고리즘 |
| 2024-01-22 | SVM · SVR 기본 예제 |

## 디렉터리 구성

### `1/` — 밑바닥부터 시작하는 딥러닝 (기초편)

신경망을 구성하는 계층을 하나씩 직접 구현하며 순전파·역전파의 원리를 학습합니다.

- `chapter2` — 퍼셉트론
- `chapter3` — 신경망 (활성화 함수, 순전파)
- `chapter4` — 신경망 학습 (손실 함수, 수치 미분, 경사 하강법) · `two_layer_net.py`, `train_neuralnet.py`
- `chapter5` — 오차역전파법 (계층별 backward 구현)
- `chapter6` — 학습 관련 기술 (옵티마이저, 가중치 초기값, 배치 정규화, 오버피팅)
- `chapter7` — CNN (합성곱·풀링 계층)
- `common/` — `layers`, `optimizer`, `trainer`, `gradient`, `functions` 등 공통 구현 모듈
- `dataset/` — MNIST 데이터 및 로더

### `2/` — 밑바닥부터 시작하는 딥러닝 2 (자연어 처리편)

- `01` — 신경망 복습
- `02` — 자연어와 단어의 분산 표현 (통계 기반 기법, PTB)
- `03` — word2vec (추론 기반 기법)
- `04` — word2vec 속도 개선
- `05` — RNN (`RNNLM` 구현)
- `06` — 게이트가 추가된 RNN (LSTM)

### `ml/` — 사이킷런 기반 머신러닝 예제

- `svm/` — SVM 분류 (유방암 진단 데이터셋)
- `SVR/` — SVR 회귀 (Boston Housing Prices 데이터셋)

### `optimization/` — 최적화 알고리즘

- `differential_evolution.ipynb` — 차분 진화(Differential Evolution) 알고리즘 구현

## 사용 기술

- Python, NumPy (신경망 밑바닥 구현)
- Jupyter Notebook
- scikit-learn (SVM, SVR 예제)

## 참고 도서

- 사이토 고키, 『밑바닥부터 시작하는 딥러닝』
- 사이토 고키, 『밑바닥부터 시작하는 딥러닝 2』
