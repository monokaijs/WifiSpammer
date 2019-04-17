# WifiSpammer
## Requirements / Yêu cầu
Yêu cầu cần có:
- Một board mạch IoT có Module Wifi ESP8266 (Như Wemos, NodeMCU, blah blah, thậm chí có thể là Arduino + ESP8266).
- Arduino IDE, link cài bên dưới.
- Một tí hiểu biết về code. (Không cần cũng được nhưng hơi khó).

You must have these things:
- An IoT Development Board that has Wifi Module ESP8266 (Such as Wemos, NodeMCU, ... or an Arduino board with ESP8266 connected).
- Arduino IDE, download link below.
- Basic knowledge about coding. (Not compulsory requirement but it's better to know what're you doing.).

## Setup / Cài đặt
> Phần này sẽ hướng dẫn bạn cách cài đặt Arduino IDE và thiết lập nó để dùng với board mạch kia.
> This section will let you know how to install Arduino IDE to your computer and the way to configure to work with our IoT Board.
### Arduino IDE Installation / Cài đặt Arduino IDE
Download Arduino IDE: [![Download Arduino IDE](https://img.shields.io/badge/downloads-1k-brightgreen.svg)](https://www.arduino.cc/download_handler.php)

The installation is quite easy, I won't mention more about it to save our time :D.
Quá trình cài đặt không có gì khó khăn nên để tiết kiệm thời gian mình sẽ không đề cập đến nó :D.

### Arduino IDE Configuration / Thiết lập Arduino IDE
> To work with ESP8266 based circuit, we must have suitable plugin for Arduino IDE to transmit data between your computer and your development board. Remember to care about the PORT you use to connect the board to your computer. I will explain about it in the next section.

> Để làm việc với mạch có ESP8266, chúng ta phải có plugin thích hợp cho Arduino IDE để trao đổi dwxl iệu giữa máy tính và mạch phát triển. Nhớ để ý xem dùng PORT nào để kết nối mạch với máy tính. Mình sẽ đề cập tới cái này trông phần tiếp.

**Step 1:** Open Arduino IDE, choose `File` -> `Preferences` (`Ctrl` + `,`)

**Bước 1:** Mở Arduino IDE lên, chọn `File` -> `Preferences` (`Ctrl` + `,`)
***
**Step 2:** Look for `Additional Boards Manager URLs`, copy paste this line to it:
```
http://arduino.esp8266.com/stable/package_esp8266com_index.json
```

**Bước 2:** Tìm ô `Additional Boards Manager URLs`, copy paste dòng này vào đó:
```
http://arduino.esp8266.com/stable/package_esp8266com_index.json
```
Then click `OK` button. / Sau đó nhấn nút `OK`.
***
**Step 3:** Open `Tools` -> `Boards` -> `Boards Manager` and Wait for the IDE to load required packets.

**Bước 3:** Mở `Tools` -> `Boards` -> `Boards Manager` và đợi một tí để IDE load xong mấy thứ cần thiết.
***
**Step 4:** Search for `esp8266`, then install the result. Finally, click Close.

**Bước 4:** Tìm `esp8266`, sau đó cài cái hiện ra trong kết quả. Cuối cùng nhấn Close.
***
**Step 5:** Open `Tools` -> `Boards` -> Choose your board in the list. Choose the suitable PORT in `Tools` -> `Ports` too.

**Bước 5:** Mở `Tools` -> `Boards` -> Chọn bảng mạch của bạn trong danh sách. Chọn luôn cả PORT trong `Tools` -> `Ports` nữa.
***
**Step 6:** Change the upload speed to 115200 at `Tools` -> `Boards` -> `Upload Speed`.

**Bước 6:** Thay đổi tốc độ Upload thành 115200 ở `Tools` -> `Boards` -> `Upload Speed`.

Then Upload my code to the board. We're done.

Sau đó Upload code lên mạch là xong.










