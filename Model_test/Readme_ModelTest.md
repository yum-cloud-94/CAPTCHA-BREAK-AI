### Model Test
> CAPTCHA 이미지를 전처리 전, 후 데이터로 학습한 뒤  
> 추가로 생성한 Test 데이터 2,000개로 모델을 평가했음.

1) 결과  
> - Vanilla CAPTCHA Image로 학습한 후 Test Data의 정확도 : 88.47%  
> - Preprocessed CAPTCHA Image로 학습한 후 Test Data의 정확도 : 82.75%  

2) 결과 해석  
> - 사람이 봐도 알아보기 힘든 CAPTCHA 이미지 데이터가 다량으로 존재함.  
> - API를 받거나 Crawling을 통해 실제로 사용되는 데이터를 사용하는 것이  
> 좋은 성능을 보일 것으로 예상.  
  
  
![그림3](https://user-images.githubusercontent.com/65157567/86538672-47acd300-bf32-11ea-94de-393265e6ccd6.png)
