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

총 11개의 데이터를 실행했고 Model은 General Model을 사용했습니다.

Model을 사용했을때 출력되는 Detection Box coordinates, Score map은 생략했습니다.

### • Input(data 1)

![KakaoTalk_20230607_223520892_06](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/9818d2c2-49b7-4652-8821-c30ec59fe480)

### • Output(data 1 - original setting)

![res_KakaoTalk_20230607_223520892_06](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/1a2cb6c6-07a5-4e04-be45-c7de9e83dd84)

### • Output(data 1 - text_threshold=0.9)

![res_KakaoTalk_20230607_223520892_06](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/f4ff409c-77dd-4fa5-8df8-cc7812657a3e)

### • Output(data 1 - link_confidence=0.9)

![res_KakaoTalk_20230607_223520892_06](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/804ec884-3452-422a-b52e-886dd706372f)

<details markdown="1">
<summary>Additional Results</summary>

### • Input(data 2)

![KakaoTalk_20230608_062945799_02](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/80b62acc-1a97-40e5-8401-b6cf2910b96f)

### • Output(data 2 - original setting)

![res_KakaoTalk_20230608_062945799_02](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/323ba9a2-96f5-471b-8af0-cdb554bd6085)

### • Output(data 2 - text_threshold=0.9)

![res_KakaoTalk_20230608_062945799_02](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/bf1a4093-154e-4e21-8179-95eacfa410a3)

### • Output(data 2 - link_confidence=0.9)

![res_KakaoTalk_20230608_062945799_02](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/662cc11d-389c-486f-bdbb-15785c5f2440)

### • Input(data 3)

![KakaoTalk_20230607_223520892_02](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/545fde7e-9d5d-460c-b24e-12158fd0cdf1)

### • Output(data 3 - original setting)

![res_KakaoTalk_20230607_223520892_02](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/babc0671-97be-42b6-9b62-f81527164dce)

### • Output(data 3 - text_threshold=0.9)

![res_KakaoTalk_20230607_223520892_02](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/2562e462-3aab-4a61-8bc4-72043d3924d8)

### • Output(data 3 - link_confidence=0.9)

![res_KakaoTalk_20230607_223520892_02](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/b2242be0-86d7-41f1-afb1-2a2660fbe626)

### • Input(data 4)

![KakaoTalk_20230608_062945799](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/b03d6556-144e-4d9f-bd3c-31a0b074b1c9)

### • Output(data 4 - original setting)

![res_KakaoTalk_20230608_062945799](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/0e3b396a-c31d-4747-94a4-74b372dd595d)

### • Output(data 4 - text_threshold=0.9)

![res_KakaoTalk_20230608_062945799](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/059ed9bc-6f6c-4a1c-b736-a7241825a8e8)

### • Output(data 4 - link_confidence=0.9)

![res_KakaoTalk_20230608_062945799](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/175a4a84-9c49-4030-8f41-3519bbdfb486)

### • Input(data 5)

![KakaoTalk_20230608_062945799_01](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/f3f5ec50-5ca2-4615-964b-fb202c836d49)

### • Output(data 5 - original setting)

![res_KakaoTalk_20230608_062945799_01](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/2362af6f-4640-4055-8ec1-aaadb01b426c)

### • Output(data 5 - text_threshold=0.9)

![res_KakaoTalk_20230608_062945799_01](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/c270778f-b6c7-4618-bffe-32ab0eb6bfa4)

### • Output(data 5 - link_confidence=0.9)

![res_KakaoTalk_20230608_062945799_01](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/ecb3701d-077d-48a1-bbd0-230471d77bb5)

### • Input(data 6)

![KakaoTalk_20230608_062945799_03](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/98d24ed7-d762-4909-a8ca-98f65e0872e3)

### • Output(data 6 - original setting)

![res_KakaoTalk_20230608_062945799_03](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/5b5efa14-6140-448a-98a4-d91e1d98aca9)

### • Output(data 6 - text_threshold=0.9)

![res_KakaoTalk_20230608_062945799_03](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/c160669d-fed4-4074-bfc0-94749004d369)

### • Output(data 6 - link_confidence=0.9)

![res_KakaoTalk_20230608_062945799_03](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/e4dec316-5aee-46ae-895c-2dd01f1fad1a)

### • Input(data 7)

![KakaoTalk_20230608_062945799_04](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/37780883-375c-4881-9425-0576f8cd2c70)

### • Output(data 7 - original setting)

![res_KakaoTalk_20230608_062945799_04](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/874cf637-1c6d-4da8-ab0f-e6319e873bde)

### • Output(data 7 - text_threshold=0.9)

![res_KakaoTalk_20230608_062945799_04](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/41e43edd-2364-47a0-81c8-70183d79add9)

### • Output(data 7 - link_confidence=0.9)

![res_KakaoTalk_20230608_062945799_04](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/a14de76e-1d82-4cb2-b650-6fae7883db71)

### • Input(data 8)

![KakaoTalk_20230608_062945799_05](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/80a7be66-bc57-409f-81db-0f8bd51886aa)

### • Output(data 8 - original setting)

![res_KakaoTalk_20230608_062945799_05](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/59904e45-ed80-4a14-af87-d98d90d742c3)

### • Output(data 8 - text_threshold=0.9)

![res_KakaoTalk_20230608_062945799_05](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/b9323ac1-2580-4850-847d-8ea69c661af4)

### • Output(data 8 - link_confidence=0.9)

![res_KakaoTalk_20230608_062945799_05](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/6c32a628-7cef-4a56-bfa9-0d36f436129c)

### • Input(data 9)

![KakaoTalk_20230608_062945799_06](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/cc3b8618-6d70-4e22-ad0b-f5cca77dfac4)

### • Output(data 9 - original setting)

![res_KakaoTalk_20230608_062945799_06](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/838be92d-b66c-44b4-a0a4-593af040aa2d)

### • Output(data 9 - text_threshold=0.9)

![res_KakaoTalk_20230608_062945799_06](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/5cf0f366-611b-43e4-8e8f-82467b0e6c94)

### • Output(data 9 - link_confidence=0.9)

![res_KakaoTalk_20230608_062945799_06](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/3353aa62-63d5-45ff-8e3e-7cd0fba95dd9)

### • Input(data 10)

![KakaoTalk_20230608_062945799_07](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/cb42304d-de4d-4417-b47d-b04b23745a2d)

### • Output(data 10 - original setting)

![res_KakaoTalk_20230608_062945799_07](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/ff10df63-43bf-4945-9ca9-648fe501505a)

### • Output(data 10 - text_threshold=0.9)

![res_KakaoTalk_20230608_062945799_07](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/561553e3-5039-4cb2-9211-4e150357fa31)

### • Output(data 10 - link_confidence=0.9)

![res_KakaoTalk_20230608_062945799_07](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/ff15b894-91f1-4817-9a84-08c55c507da9)

### • Input(data 11)

![KakaoTalk_20230608_063256526](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/ef3fadc4-0638-47ef-8bdc-6529ce11794d)

### • Output(data 11 - original setting)

![res_KakaoTalk_20230608_063256526](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/06e67aca-87e3-49be-a665-6e431c7a12ff)

### • Output(data 11 - text_threshold=0.9)

![res_KakaoTalk_20230608_063256526](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/4e6d1b18-7463-4256-a157-a027ce277282)

### • Output(data 11 - link_confidence=0.9)

![res_KakaoTalk_20230608_063256526](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/138153d1-fa76-428f-8044-adf9dc29166a)

</details>

## • Analysis/Visualization

11개의 이미지 데이터를 바탕으로 5가지 항목과 결론으로 나누어서 결과를 분석했습니다.

1. Horizontal Text

![image](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/72976867-0df3-422d-ae94-d643eabdf4f8)
![image](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/15dbf48e-f48d-4d80-b9e2-42274cbe1960)

수평방향의 텍스트는 단어가 굉장히 많음에도 1개의 단어를 빼고는 Text Detection을 잘 수행하는 것을 볼 수 있다. 30도 정도 기울어진 텍스트 또한 2개 정도의 단어 빼고는 Text Detection을 잘 수행하는 것을 볼 수 있다. 보통은 텍스트들이 가로방향으로 되어 있기 때문에 Model을 학습할 때 사용된 data set도 가로방향이 많았을 것이고 이러한 이유 때문에 가로방향의 텍스트들은 Text Detection이 잘 수행되는 것이라고 추측할 수 있다.

2. Vertical Text

![image](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/fa6bd7b0-76f3-4bad-8c78-bb7162f107ec)
![image](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/c4d13d2e-b8c4-4a50-a43e-329b7261b7d0)


세로방향의 텍스트들도 곧잘 Detection 되는 것을 볼 수 있다. 하지만 가로 방향의 텍스트들은 글자가 작아도 단어별로 잘 Detection 되는 반면에, 세로방향의 텍스트는 글자가 작으면 단어별로 잘 묶지 못한다는 것을 알 수 있다. 그리고 오른쪽에 있는 이미지를 보면 한자 또한 text로 잘 인식이 된다는 것을 알 수 있다.

3. Curved Text

![image](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/31132e29-cde0-4253-b558-5ed69d754dcf)
![image](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/93d8f86f-5c29-43ad-95b4-e65f5e321a8b)


왼쪽의 이미지를 보면 커브 방향으로 배치된 text들도 잘 Detection 되는 것을 볼 수 있다. 하지만 오른쪽 이미지를 보면 정면에서 보이는 curved text들은 Detection 되지만, 곡면에 위치한 왼쪽, 오른쪽 curved text들은 Detection되지 않는다는 것을 볼 수 있다. 또한, 단어간 간격이 너무 넓으면 하나의 단어로 묶이지 않는다는 것을 알 수 있다.

4. Text With (text_threshold=0.9) 

![image](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/2239240c-b733-452e-a78d-d0ac0b5c8a40)

text_threshold 변수는 이미지의 text를 text로 인식하는 기준이 되는 threshold 값이다. Original text_threshold값은 0.7이고, 실험에서는 0.9로 설정하고 실행했다. 위의 그래프를 보면 text_threshold값을 높였을 때 original 값일 때보다 Detection Box의 수가 줄어든다는 것을 알 수 있다. 이미지에 있는 text를 text로 인식하는 기준이 높아졌기 때문에 text가 이미지에서 선명하게 보이지 않으면 Detection이 잘 되지 않는다는 것을 알 수 있다. 따라서 확실하게 text로 보이는 text만 Detection하고 싶다면 text_threshold 값을 높여서 사용하는 것이 좋고, 가능한 한 모든 text들을 Detection하고 싶다면 text_threshold 값을 낮추는 것을 추천한다. 

5. Text With (link_threshold=0.9)

![image](https://github.com/hyeokson/opensw23-gitgit/assets/127181634/733832c1-faa5-4885-ae49-e79e10796139)

link_threshold 변수는 문자들이 하나의 단어로 Detection이 될 때 기준이 되는 threshold 값이다. Original link_threshold값은 0.4이고, 실험에서는 0.9로 설정하고 실행했다. 위의 그래프를 보면 link_threshold값을 높였을 때 original 값일 때보다 Detection Box의 수가 늘어난다는 것을 알 수 있다. 하나의 단어로 Detection 되는 기준이 높아졌기 때문에 각 문자들 간의 거리가 매우 가깝지 않은 이상 개별적인 단어로 Detection 된다는 것을 알 수 있다. 따라서 문자들 간 간격이 기본적으로 넓다면 link_threshold값을 낮추는 것이 좋고, 간격이 좁지만 띄어쓰기가 잘 되어 있다면 link_threshold값을 높이는 것을 추천한다.

<결론>

Horizontal, curved text들은 Detection이 훌륭하게 수행되지만, 곡면에 위치한 text, horizontal text들은 Detection이 아예 안되거나, 같은 단어로 묶이지 않는 경우가 많으므로 이 부분에 대한 개선이 필요하다고 생각한다. 

그리고 CRAFT text detector를 사용할 때, 확실하게 text로 보이는 text들만 Detection하고 싶다면 text_threshold 값을 높여서 사용하는 것이 좋고, 가능한 한 모든 text들을 Detection하고 싶다면 text_threshold 값을 낮추는 것을 추천한다. 또한, 문자들 간 간격이 기본적으로 넓다면 link_threshold값을 낮추는 것이 좋고, 간격이 좁지만 띄어쓰기가 잘 되어 있다면 link_threshold값을 높이는 것을 추천한다.


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
   
