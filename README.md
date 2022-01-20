## hardware & 전장설계 & 시리얼(Serial)

H/W 설계로는 기초적으로 시작할 때 Fritzing 또는 심화로 시직할 때는 STM32CubeIDE or STM32CubeMX 전장도를 구성할때는 Wondershare EdrawMax를 추천한다 전부 오픈소스로 사용이 가능하고 다양한 보드툴 및 기능을 제공하며 사용을 할 수 있다.

전장 도식을 할떄 사용한 프로그램은  ```Wondershare EdrawMax``` 를 사용함 무료판도 양호 하게 사용 할 수 있는 장점이 있다

## EdrawMax

![aaaa](https://user-images.githubusercontent.com/84003327/149474386-380fd59c-045c-4315-8855-f7e6b284d5f2.PNG)


## Fritzing

보이는 것과 같이 다양한 툴을 사용 할 수 있으며 ```Fritzing```에서 코드를 작성 후 시뮬레이션 까지 할 수 있는 장점이 있다, 툴의 시각화 또한 잘되있어 ```Fritzing```으로 먼저 실험해보고 직접 만드는 절차를 추천한다.   Fritzing을 모르는 사람이 많아서 사용한다면 더욱 편리한 전장 설계를 할 수 있다

![asa](https://user-images.githubusercontent.com/84003327/149685147-ac0fb817-3092-4b74-83d0-b5737d39e4d1.PNG)


## STM32CubeIDE 

심화 단계로 넘어 왔다면  ```STM32CubeIDE``` 를 추천한다, 점더 세밀하게 pin의 대한 정보 및 설정을 할 수 있으며 실무에서 자주 사용되는 툴이다, ```STM32CubeMX``` 툴을 함깨 사용하면 더욱 편리한 하드웨어 코딩을 할 수 있으며 실전 컴파일 및 업로드를 지원한다.

![캡처](https://user-images.githubusercontent.com/84003327/149685425-308ed1d2-1917-46e8-af41-64a781cc841b.PNG)


## 시리얼(Serial) 포트 사용해보기 

시리얼 포트란? 시리얼(Serial), 유아트(UART), 컴포트(COM) 등등 다양한 이름으로 불리는데 주로 ```디버깅용```이나 ```바이너리 전송용```으로 활용된다

시리얼을 사용하기 전에 먼저 컴퓨터의 usb 포트에 잘 연결되 있는지 확인을 해야 한다, 이 과정이 시리얼 포트를 사용하기 위한 가장 첫 단계이다.

![장치 관리자](https://user-images.githubusercontent.com/84003327/150054460-7bec7145-8f74-4bb2-8f5e-ca2986ec8cac.PNG)

보이는것 처럼 ```포트(COM & LPT)```를 보면 하나는 ```뉴클레오```, 하나는 ```시리얼이```(초음파 센서) 연결되 있는것을 확인 할 수 있다

연결을 확인 했다면 ```시리얼 모니터``` 프로그램를 사용해서 직동상태를 확인 할 수 있다 시리얼 모니터 프로그램에는 다양하게 있지만 대중적으로  ```Arduino```, ```PUTTY```, ```J1C```등을 사용하고 

## Arduino

가장 대중적으로 하드웨어 및 코딩을 입문하는데 사용하는 툴이다 아두이노 보드를 사용하여 led와 각종 센서를 제저 하는데 활용 할 수 있다

![아두이노 시리얼 모니터](https://user-images.githubusercontent.com/84003327/150062792-a968e3a5-39a8-4167-a0ab-a6b7762701d4.PNG)![ar](https://user-images.githubusercontent.com/84003327/150062939-86eee6a8-3221-4a3c-9073-8e3b08ef6fb8.PNG)


## putty 

PuTTY는 SSH, 텔넷, rlogin, raw TCP를 위한 클라이언트로 동작하는 자유 및 오픈 소스 단말 에뮬레이터 응용 프로그램이다. PuTTY라는 이름에는 특별한 뜻이 없으나 tty는
유닉스 전통의 터미널의 이름을 가리키며 teletype를 짧게 줄인 것이다

![putty](https://user-images.githubusercontent.com/84003327/150062252-4db44485-580e-4d86-b1de-9e091e6d3f8b.PNG)![pu](https://user-images.githubusercontent.com/84003327/150062854-e6f5b24b-c262-4bf3-ac87-98fad9c39db2.PNG)


시리얼 라인에 연결된 포트 번호를 넣어주고 Speed에서 통신속도를 지정해주면 된다, 통신속도는 사용하는 기기의  ```data sheet ```를 보면 알 수 있는데 뒤에 설명 하겠다

## J1C

[J1C_User_Manual.pdf](https://github.com/leeeju/hardware/files/7894035/J1C_User_Manual.pdf)  <- 설명서 다운!!


![j1c](https://user-images.githubusercontent.com/84003327/150063216-6655994a-3a70-4e4f-97b6-3847a3a71c51.PNG)![j1](https://user-images.githubusercontent.com/84003327/150063574-291c55f5-e2a9-4cde-9c6c-3a0a6d4cb463.PNG)

위와 같이 시리얼 모니터를 사용하여 추가 장비를 시리얼통신 연결을 할 수 있다

## data sheet 사용법

데이터 시트는 하드웨어를 하는 사람이라면 반드시 읽을 수 있어야 하는 것이다, 추가로 장착할 장비의 기본 제원 및 연결방법이 나와있는 문서로 통신 속도, RX TX와 같은 데이터 라인의 대한 설명이 적혀 있는 것을 확인 할 수 있다   

https://www.alldatasheet.com/ 를 참조하여 데이터 시트를 검색해 보자


## 통신속도의 중요성

데이터 통신 속도는 통상적으로 bps 또는 BAUD로 나타낸다, BPS란? 1초당 몇개의 비트(bit)가 송/수신 되는가를 말하며 대부분의 신호전달은 하나의 신호의 하나의 비트로 대응된다
데이터를 주고 받는 PC와 기기 사이의 사로간의 통신 속도가 맞지 않으면 잘못된 정보 및 오류가 수신된다

Baud rates 값은 어떻게든 설정할 수 있지만 통신 속도에 크게 영향을 받지 않는 경우 일반적으로 9600 bps를 사용한다. 다른 표준 baud are 값으로 1200, 2400, 4800, 19200, 38400, 57600, 115200 을 사용할 수도 있다
