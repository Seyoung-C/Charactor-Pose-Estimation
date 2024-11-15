# Charactor-Pose-Estimation
Pose estimation for animated characters through augmentation of human pose datasets
---
## Repository
```
Charactor-Pose-Estimation/
│
├── README.md                       # 프로젝트 개요, 설치 방법, 사용법 등의 설명
├── requirements.txt                # 필요한 패키지 목록
├── setup.py                        # 패키지 설치 및 초기화 관련 스크립트 (필요할 경우)
├── .gitignore                      # Git에 포함하지 않을 파일 목록
│
├── data/                           # 원본 데이터 및 전처리한 데이터 저장 폴더
│   ├── raw/                        # 원본 데이터 (MPII Human Pose, augmented images 등)
│   ├── processed/                  # 전처리된 데이터 저장 (JSON, .mat 파일 등)
│   └── augmentation/               # 증강된 데이터셋 저장 폴더
│
├── notebooks/                      # Jupyter Notebook 파일들
│   ├── data_augmentation/          # 데이터 증강 관련
│   ├── model_training/             # 모델 학습 관련
│   └── experiments/                # 다양한 실험 관련
│
├── src/                            # 주요 소스 코드
│   ├── __init__.py                 # 패키지 초기화 파일
│   ├── data/                       # 데이터 로더 및 전처리 관련 코드
│   │   ├── data_loader.py          # 데이터 로딩 함수 및 데이터셋 클래스
│   │   └── augmentation.py         # 데이터 증강 함수
│   ├── models/                     # 모델 관련 코드
│   │   ├── pose_estimation_model.py # 포즈 에스티메이션 모델 정의
│   │   └── utils.py                # 모델 유틸리티 함수 (가중치 로드 등)
│   ├── training/                   # 모델 학습 및 평가 관련 코드
│   │   ├── train.py                # 학습 스크립트
│   │   └── evaluate.py             # 평가 스크립트
│   └── utils/                      # 기타 유틸리티 코드
│       ├── visualization.py        # 시각화 함수 (예: 포즈 추정 결과 오버레이)
│       └── helpers.py              # 기타 보조 함수들
│
├── experiments/                    # 실험 및 결과 저장 폴더
│   ├── logs/                       # 학습 및 평가 로그
│   ├── checkpoints/                # 모델 체크포인트
│   └── results/                    # 평가 결과 및 메트릭 (그래프, 수치 등)
│
└── scripts/                        # 실행 가능한 스크립트 모음
    ├── download_data.sh            # 데이터셋 다운로드 스크립트
    ├── preprocess_data.py          # 전처리 스크립트
    └── run_training.sh             # 학습 실행 스크립트
```
