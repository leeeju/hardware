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


## putty 
![putty](https://user-images.githubusercontent.com/84003327/150062252-4db44485-580e-4d86-b1de-9e091e6d3f8b.PNG)


 data sheet
