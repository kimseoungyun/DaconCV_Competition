# 'SW중심대학 공동 AI 경진대회 2023' 대회

## 코드 소개
- Dacon에서 주최한 'SW중심대학 공동 AI 경진대회 2023'에 나갔을 때, 사용한 코드입니다.

## 대회 소개
- 위성 이미지로부터 정밀한 건물의 영역을 분할해내는 대회입니다.
- https://dacon.io/competitions/official/236092/overview/description

## 대회 기간
-  2023.07.03 ~ 2023.07.28

## 대회 성적
- 35/277으로 상위 16%으로 마무리했습니다. (22위까지 순위권이었습니다.)

## 사용한 기법
- UNet 모델
- ResNet 모델
- Cutmix 증강기법

## 파일 설명
- train.py 파일을 통해서 가중치 파일을 저장합니다.
- inference.py 파일을 통해서 가중치 파일을 활용한 모델로부터 submit 파일을 얻어냅니다.
- test_result.py 파일을 통해서 submit 파일을 시각화해서 확인할 수 있습니다.
- model.py 파일에서 학습에 사용할 모델을 만듭니다.
- model_loader.py 파일에서 학습에 사용할 모델을 로드합니다.
- dataloader.py 파일을 통해서 불러온 데이터에 적용할 dataloader를 만듭니다.
- cutmix.py 파일은 당시에 가장 핫했던 cutmix 기법을 구현하려 했던 코드입니다.
- custom_dataset.py 파일은 데이터셋에 추가 조치를 해서 로드하는 코드입니다.
- custom_csv.py 파일은 csv파일에 적힌 img path 정보를 수정하는 코드입니다.
- utils.py 파일은 RLE 인코딩과 디코딩하는 코드입니다.

## 기술적 역할
- 학습 파이프라인 작성
- 다양한 모델 코드 작성 및 실험
- 결과 확인 코드 작성
- 학습 성능 지표 코드 작성
- 다양한 기법(최적화 함수, 활성화 함수, loss 함수, 증강기법 등등) 및  가설검증 및 하이퍼파라미터 튜닝
- inference.py 코드 작성

## 배운 점
- 첫 imagesegmentation 프로젝트이자 두 번째 CV 프로젝트여서 CV 모델에 대한 깊은 이해와 여러 증강기법에 대한 공부를 할 수 있었습니다.
- 딥러닝 학습 파이프라인에 대해서 확실히 감을 익힐 수 있게 되었습니다.
- 실제로 대회에서의 점수 차이가 정말 사소한 것에서 나뉜다는 것을 알게 되었습니다.
- 반복되는 가설과 검증에 익숙해질 수 있었고 생각 이상으로 뜻대로 성능이 오르지 않는다는 것을 알게 되었습니다.
- 최신 논문을 찾아내는 능력과 이를 코드로 구현하는 능력이 상당히 요구되는 것을 알게 되었고 학습의 필요성을 느끼게 됐습니다.

ps: 데이터는 Dacon 홈페이지 다운로드 받을 수 있습니다.
