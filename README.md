# opensw23-gitgit

## • Team Introduction

name : 손찬혁
    
ID : 201713061
   
## • Topic Introduction
### CRAFT: Character-Region Awareness For Text detection
원본 github address : https://github.com/clovaai/CRAFT-pytorch/tree/master

CRAFT text detector는 딥러닝을 이용한 텍스트 검출기 입니다. 

이미지를 input으로 설정하면 bounding box로 텍스트가 검출된 이미지와 score map, bounding box 좌표값이 적힌 text file이 output으로 출력됩니다. 

text detector에 적용된 CRAFT 모델은 Scene text detection, 즉 문자의 위치를 식별하고 지역화를 해주는 모델입니다. CRAFT 모델은 Character-level의 문자 식별을 위해 Weakly-supervised learning 과 Region & Affinity score 을 이용하여 구현되었습니다. 
    
## • Results

### • Input
![AKR20200325003700091_01_i_P4](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/f574204e-643e-43ef-afb0-35caed9c6f22)

### • Output (General Model 사용)
#### <result image, score map, bounding box coordinates>

![res_AKR20200325003700091_01_i_P4](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/111ea7c7-4b23-419e-ac87-9a7b0aad5f96)

![res_AKR20200325003700091_01_i_P4_mask](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/3045e974-cdc0-453e-a3d6-5577c4ef1768)
    
![coordinates](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/6bb4e57d-aa35-4458-96d6-4bd8a67cf1a4)

<details markdown="1">
<summary>Additional Results</summary>

<!--summary 아래 빈칸 공백 두고 내용을 적는공간-->

</details>

## • Analysis/Visualization

## • Installation

### 테스트 환경
OS : Windows 10 Home

CPU : Intel(R) Core(TM) i5-8250U CPU @ 1.60GHz   1.80 GHz

RAM : DDR4 8.00GB

GPU : Intel(R) UHD Graphics 620
    
### 1. git repository clone 하기
```
git clone https://github.com/hyeokson/opensw23-gitgit.git
```
### 2. python library 설치하기
(recommended) python 가상환경을 생성하고 library 설치

cmd에서 실행

- torch
- torchvision
- torchaudio
- opencv-python
- numpy
- scipy 
```
pip install -r requirements.txt
```
### 3. pretrained model 설치하기
*Model name* | *Used datasets* | *Languages* | *Purpose* | *Model Link* |
 | :--- | :--- | :--- | :--- | :--- |
General | SynthText, IC13, IC17 | Eng + MLT | For general purpose | [Click](https://drive.google.com/open?id=1Jk4eGD7crsqCCg9C9VjCLkMN3ze8kutZ)
IC15 | SynthText, IC15 | Eng | For IC15 only | [Click](https://drive.google.com/open?id=1i2R7UIUqmkUtF0jv_3MXTqmQ_9wuAnLf)

설치하신 pth파일은 git file 최상위 디렉토리에 저장하시면 됩니다.

### 4. pretrained model로 실행하기
```
python test.py --trained_model=[weightfile] --test_folder=[folder path to test images] --cuda=0

<General model 사용>
ex) python test.py --trained_model=craft_mlt_25k.pth --test_folder=sample_input --cuda=0

<IC15 model 사용>
ex) python test.py --trained_model=craft_ic15_20k.pth --test_folder=sample_input --cuda=0
```
result image는 default로 `result` 폴더에 저장됩니다.

sample input과 output 이미지는 각각 sample_input, sample_output 폴더에 있습니다.
### Arguments
* `--trained_model`: pretrained model
* `--text_threshold`: text confidence threshold
* `--low_text`: text low-bound score
* `--link_threshold`: link confidence threshold
* `--cuda`: use cuda for inference (default:True)
* `--canvas_size`: max image size for inference
* `--mag_ratio`: image magnification ratio
* `--poly`: enable polygon type result
* `--show_time`: show processing time
* `--test_folder`: folder path to input images
* `--refine`: use link refiner for sentense-level dataset
* `--refiner_model`: pretrained refiner model

## • Presentation
   
