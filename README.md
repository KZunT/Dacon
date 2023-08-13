<div align=center>
    <h1>데이콘 경진대회 코드 저장소</h1>
    <br>
</div>

## 유방암의 임파선 전이 예측 AI 경진대회
![image](https://github.com/KZunT/Dacon/assets/94132370/05d9a6f0-82c9-4f09-b41a-b367e415c037)

### [주제]
유방암 병리 슬라이드 영상과 임상 항목을 통한 유방암의 임파선 전이 여부 예측

### [목표]
유방암 병리 슬라이드 영상과 임상 항목을 조합하여 유방암의 임파선 전이 여부 이진 분류


### [주최 / 주관]
- 주최 : 연세대학교 의과대학, JLK, MTS 
- 후원 : 보건산업진흥원  
- 주관 : 데이콘
--- 

## Solution

### Image data
- H&E normalization 적용
- Multi instance learning을 위한 224x224 크기 패치 분할

### Tabular data
- REFCV 기반의 feature selection


### Model structure
![제스텍프로젝트의 복사본 drawio (1)](https://github.com/KZunT/Dacon/assets/94132370/319e3445-4710-4ec9-8a04-fe5814e2ffbb)

- Image feature extractor (Resnet50) - Multi instance learning
- Tabular feature extractor (DNN) 
- Classifier (DNN)

## Reference
- [Tumor Classification](https://www.nature.com/articles/s41598-020-58467-9)
- [Multi Instance Learning](https://arxiv.org/abs/1802.04712)
- [Multi Instance Learning이란?](https://www.edwith.org/medical-20200327/lecture/63148/)
- [whole-slide training approach](https://www.nature.com/articles/s41467-021-21467-y)
