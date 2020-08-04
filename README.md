

## Qbang-text anal module part 1 : 이미지 바운딩 박스 생성

- 저는 anaconda 가상환경을 사용합니다.

#### 버전 요구사항
- PyTorch>=0.4.1
- torchvision>=0.2.1
- opencv-python>=3.4.2
- check requiremtns.txt

<requirement install 실행문>
```
pip install -r requirements.txt
```


* 학습된 모델 directory : ./qbang_model/craft_mlt_25k.pth
* 테스트할 영상은  directory : ./test
  에 넣어주시면 됩니다.
  
<이미지 테스트 실행문>  
``` (with python 3.7)
python test.py --trained_model=qbang_model/craft_mlt_25k.pth --test_folder=test
```

결과영상 저장 directory :  `./result` (by default)

### Arguments 설명 
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




## License
```
에센플랫 ESSENPLAT

Technology Development / CTO
Darin

darin@essenplat.com

```
