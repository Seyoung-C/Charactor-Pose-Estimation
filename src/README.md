## 주요 소스 코드 폴더입니다.
---
### 폴더 구성
```
src/                            # 주요 소스 코드
   ├── __init__.py                 # 패키지 초기화 파일
   ├── data/                       # 데이터 로더 및 전처리 관련 코드
   │   ├── data_loader.py          # 데이터 로딩 함수 및 데이터셋 클래스
   │   └── augmentation.py         # 데이터 증강 함수
   ├── models/                     # 모델 관련 코드
   │   ├── pose_estimation_model.py # 포즈 에스티메이션 모델 정의
   │   └── utils.py                # 모델 유틸리티 함수 (가중치 로드 등)
   ├── training/                   # 모델 학습 및 평가 관련 코드
   │   ├── train.py                # 학습 스크립트
   │   └── evaluate.py             # 평가 스크립트
   └── utils/                      # 기타 유틸리티 코드
       ├── visualization.py        # 시각화 함수 (예: 포즈 추정 결과 오버레이)
       └── helpers.py              # 기타 보조 함수들
```
