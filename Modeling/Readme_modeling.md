### CRNN + CTC Layer
> CNN과 RNN(LSTM)을 결합해 텍스트 이미지로부터 특성을 추출하고 글자를 학습한다.  
> CTC Layer를 추가해 중복되는 글자, 띄어쓰기 등을 줄여 True Label을 맞춰준다.  

- 모델 구조   
![그림4](https://user-images.githubusercontent.com/65157567/86538320-54c8c280-bf30-11ea-8ec0-61869ec1797b.png)  

- CTC Layer 구조  
![그림1](https://user-images.githubusercontent.com/65157567/86538350-8b9ed880-bf30-11ea-8aa6-897adcbd48ba.png)  

- CAPTCHA 텍스트 이미지 예시  
![그림2](https://user-images.githubusercontent.com/65157567/86538351-8d689c00-bf30-11ea-840f-51d82fc34a4e.png)  


[Reference: modeling](https://m.blog.naver.com/PostView.nhn?blogId=sogangori&logNo=221183469708&proxyReferer=https:%2F%2Fwww.google.com%2F)  
[Reference: CTC Layer](https://distill.pub/2017/ctc/)  
[Reference: kaggle](https://www.kaggle.com/aakashnain/building-a-captcha-ocr-in-tf2-0)  
