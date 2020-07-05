## CAPTCHA-BREAK-AI
Breaking CAPTCHA for Intelligence RPA

### 프로젝트 개요
CAPTCHA를 무력화해서 Intelligence RPA를 구현하도록 하는 프로젝트이다.

### 폴더 설명
1) __DATA__  
CAPTCHA 이미지를 Python Library로 생성  
  
  

2) __Image_preprocessing__   
Dillation, Close연산으로 선, 점의 노이즈를 제거해준다.  
  
- 원본 이미지  
![그림1](https://user-images.githubusercontent.com/65157567/86440773-08ba2a00-bd46-11ea-85f8-aad625f846bc.png)  
- 선 제거 이미지(Dillation 연산)  
![그림2](https://user-images.githubusercontent.com/65157567/86440809-1a9bcd00-bd46-11ea-89c1-4802135b7396.png)  
- 점 제거 이미지(Close 연산)  
![그림3](https://user-images.githubusercontent.com/65157567/86440898-43bc5d80-bd46-11ea-9ec4-3d211cd9b710.png)   

3) __Modeling__  
CRNN + CTC Layer 모델 사용  
Vanilla CAPTCHA Image와 Preprocessed CAPTCHA Image 두 가지 데이터를 모델에 적용  
  
  
4) __Model_Test__  
2,000개의 CAPTCHA 이미지를 추가로 생성   
Tesseract-OCR, CRNN+CTC Layer 모델로 결과를 비교   
  
### 설치 패키지
1. Tesseract-OCR
```python
!pip install pytesseract
import pytesseract

# pytesseract 환경변수 설정 필요
pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files (x86)\Tesseract-OCR\tesseract'

# 사용법 
pytesseract.image_to_string(image,config='--psm 6 oem 3, lang=eng)
```

2. Generate CAPTCHA Image
```python
!pip install captcha
from captcha.image import ImageCaptcha
```

