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

- 데이터는 Dacon 홈페이지 다운로드 받을 수 있습니다.