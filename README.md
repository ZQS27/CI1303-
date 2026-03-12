# CI1303离线语音识别模块
CI1303 是启英泰伦推出的离线语音识别模块，与天问同架构，可使用天问同款软件和驱动以及AI模型，支持本地识别命令词，无需联网，响应快、功耗低，常用于家电、智能控制等场景。
原理图：
<img width="865" height="419" alt="image" src="https://github.com/user-attachments/assets/89fb42d7-a39e-4cdf-b39b-78c097e9e4f4" />

PCB电路：

信号层1：

<img width="865" height="1078" alt="image" src="https://github.com/user-attachments/assets/ebab73da-b694-4143-9026-c0964057117a" />

地层：

<img width="865" height="1045" alt="image" src="https://github.com/user-attachments/assets/0f6e3149-cc41-42fa-a074-4aab91384ebf" />

电源层：

<img width="865" height="1043" alt="image" src="https://github.com/user-attachments/assets/4aa69dc6-7579-4dbe-97fe-7d835a123ed4" />

底层信号层：

<img width="865" height="1042" alt="image" src="https://github.com/user-attachments/assets/17c3830f-ec89-45da-8418-7163a3291a95" />

CI1303的离线语音模块，板子集成了8002D功放芯片，可以驱动一个3W的喇叭。引出全部引脚，麦克风和喇叭接口采用PH2.0。已验证成功，测试没有问题。

<img width="359" height="478" alt="image" src="https://github.com/user-attachments/assets/623a474b-f43e-4984-8480-a82571769d95" />

烧录方法是使用USB-TTL烧录器进行烧录，RXD接PB5(TX)，TXD接PB6(RX)，使用天问black烧录会遇到提示：请是否连接设备ASR-FR0?（如图），需要拔掉连接核心板的GND引脚，按住核心板上按键（长按不松手），再重新插上GND进行升级烧录。

<img width="865" height="463" alt="image" src="https://github.com/user-attachments/assets/971d4128-7721-40d0-993d-415e98250e2c" />

若遇到提示设备连接成功后又连接失败的情况图3，建议在天问block提示：请是否连接设备 ASR-FR0?前不要连接GND，当提示请是否连接设备 ASR-FR0?再连接GND，可以保证不会因为断开时间不足5s而重新连接失败的情况。

<img width="922" height="198" alt="image" src="https://github.com/user-attachments/assets/906b8ac2-a983-4da5-b312-e870617f2ef9" />
<img width="786" height="260" alt="image" src="https://github.com/user-attachments/assets/ee441974-38cf-4a13-98f1-f9771108ad50" />











