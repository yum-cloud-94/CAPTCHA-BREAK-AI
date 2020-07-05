## DATA 설명
> Python으로 CAPTCHA 이미지 데이터를 생성함  
> Windows 운영체제의 Jupyter Notebook에서 작성   

#### 데이터 생성 기준  
1) 영어 소문자, 숫자로만 구성(a-z, 0-9, 총 36개)  
2) Width, Height = 150, 50  
3) 6자리의 CAPTHCHA 텍스트 이미지  

#### 데이터 생성을 위해 설치해야하는 패키지
1) CAPTCHA  
```python  
!pip install captcha  
from captcha.image import ImageCaptcha  
```
2) CLAPTCHA  
```python  
!pip install claptcha  
from claptcha import Claptcha  
```
#### 이미지 샘플
1) CAPTCHA  
![8p41m8](https://user-images.githubusercontent.com/65157567/86043769-1e98c800-ba84-11ea-91db-a17070d24180.png) ![b3v0mh](https://user-images.githubusercontent.com/65157567/86043828-2f493e00-ba84-11ea-92c3-752f85af88ea.png) ![osowdu](https://user-images.githubusercontent.com/65157567/86043910-4ee06680-ba84-11ea-81e9-76eadf698bae.png)  

2) CLAPTCHA  
![4yfj4j](https://user-images.githubusercontent.com/65157567/86043986-6c153500-ba84-11ea-87fc-6c0976440b05.png) ![7fhh5l](https://user-images.githubusercontent.com/65157567/86044010-76373380-ba84-11ea-8ea5-7672b7cc8fd2.png) ![hpd9xc](https://user-images.githubusercontent.com/65157567/86044065-89e29a00-ba84-11ea-82c0-8b3025db6906.png)


---------
* 참고  
CLAPTCHA의 경우, 이미지 사이즈를 조정하는 것, 폰트 하나만 지정할 수 있다는 점 등의 이유로  
CAPTCHA 이미지 10,000개만 사용해서 프로젝트를 진행함.

