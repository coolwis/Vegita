### 동빈나 유투버 강의 소스를 사용하여 Aws EC2 개발 되었습니다.
 http://ec2-3-34-69-170.ap-northeast-2.compute.amazonaws.com:2022

# 기술 스펙
```
pyhon
Flask Web Api Server
tensorflow
```

### 실행: FLASK SERVER 실행하여 접속하여 확인 가능

```
   host는 외부에서 접속 가능하도록 '0.0.0.0' 으로 지정
*  app.run(host='0.0.0.0', port='2022', debug = True) # for external connect : 0.0.0.0
*  실행: python3 server.py
```

### 배추 가격 예측 인공지능 소프트웨어
배추 가격을 예측하는 인공지능 소프트웨어입니다. <br/>


### 시스템 구성도
![image](https://user-images.githubusercontent.com/16822641/44393019-8881e580-a56e-11e8-8c08-f72eb87f1016.png)

### Demo Web Site
![image](https://user-images.githubusercontent.com/16822641/44393034-933c7a80-a56e-11e8-9678-a3a088e7d23f.png)

### 참고 문헌
* [기상청 전국 기온 및 강수량](https://data.kma.go.kr/climate/StatisticsDivision/selectStatisticsDivision.do?pgmNo=158) : 기상청 정보를 토대로 채소 가격에 영향을 미치는 요인을 분석하기 위해 참고하였습니다.
* [월별 배추 가격](https://www.kamis.or.kr/customer/price/retail/period.do?action=monthly&yyyy=2018&period=10&countycode=&itemcategorycode=200&itemcode=211&kindcode=&productrankcode=&convert_kg_yn=N) : 실질적인 국내 월별 배추 가격을 분석하기 위해 참고하였습니다.
* [시계열수치입력 수치예측 모델 레시피](https://tykimos.github.io/2017/09/09/Time-series_Numerical_Input_Numerical_Prediction_Model_Recipe/) : 시계열(Time-Series Analysis) 예측 모델 학습자료로 참고하였습니다.

* 기상청 기온과  농산물센터의 배추가격을 붙여서 날짜별 데이터를 만듦
* price data.csv

![image](https://user-images.githubusercontent.com/1407572/155975456-e41b0f85-49fa-4c29-8d36-90880b8c676d.png)



### 서버 실행 명령어
```
# 깃 허브에서 소스코드를 다운로드 받습니다.
git clone https://github.com/coolwis/Vegita.git

원본:
git clone https://github.com/ndb796/Vegita.git

# UI template 는  bootstrap을 활용
https://mdbootstrap.com/freebies/

# 받은 프로젝트 폴더로 이동합니다.
cd Vegita

# 플라스크 웹 서버 폴더로 이동합니다.
cd "Flask Web Server"

# 웹 서버를 실행합니다.
python server.py

# http://127.0.0.1:5000 에서 확인
```

### 파이썬 데이터 학습 모델 생성 명령어
```
# 프로젝트 폴더에서 파이썬 폴더로 이동합니다.
cd "Python Software"

# 엑셀(Excel) 파일로 학습을 수행합니다.
python offline.py

# (옵션) 학습된 데이터를 확인합니다.
python "predict test.py"
>> 평균 온도: -2.7
>> 최저 온도: -6.6
>> 최고 온도: 2.0
>> 강수량:  0.1
[2000.2086]

# 이후에 생성된 모델 파일을 웹 서버의 model 폴더에 붙여넣기 하면 적용됩니다.
```

#### 참고한 강의
https://www.youtube.com/watch?v=86u8TmkRN38&list=PLRx0vPvlEmdAbnmLH9yh03cw9UQU_o7PO&index=14

