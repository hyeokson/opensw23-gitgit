# Assignment Day 1

## • Team Introduction

name : 손찬혁
    
ID : 201713061
   
## • Topic Introduction

CRAFT text detector는 딥러닝을 이용한 텍스트 검출기 입니다. text detector를 사용하게 되면 bounding box로 이미지에 있는 텍스트를 검출할 수 있습니다. text detector에 적용된 CRAFT 모델은 Scene text detection, 즉 문자의 위치를 식별하고 지역화를 해주는 모델입니다. CRAFT 모델은 Character-level의 문자 식별을 위해 Weakly-supervised learning 과 Region & Affinity score 을 이용하여 구현되었습니다. 
    
## • Results
<원본 이미지>

![AKR20200325003700091_01_i_P4](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/f574204e-643e-43ef-afb0-35caed9c6f22)

<CRAFT text detector 적용 후 이미지>

![res_AKR20200325003700091_01_i_P4](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/111ea7c7-4b23-419e-ac87-9a7b0aad5f96)
    
## • Analysis/Visualization

## • Installation
    
1. git repository clone 하기
```
git clone https://github.com/hyeokson/opensw23-gitgit.git
```
2. python library 설치하기
- torch
- torchvision
- torchaudio
- opencv-python
- numpy
- scipy 
```
pip install torch torchvision torchaudio opencv-python numpy scipy
```
3. pretrained model로 실행하기
```
python test.py --trained_model=[weightfile] --test_folder=[folder path to test images]
```
result image는 default로 `result` 파일에 저장됩니다.

## • Presentation
   
