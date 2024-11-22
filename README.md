# Mạch Mtiny Uno ATmega328P (Arduino Compatible)

![](/image/mtiny_328p_1.jpg)

## Giới thiệu

Mạch Mtiny Uno ATmega328P (Arduino Compatible) được nghiên cứu và và sản xuất bởi MakerLab.vn dựa trên nguyên mẫu là mạch Arduino Uno, mạch có thiết kế nhỏ gọn tiện lắp đặt, dễ dàng kết nối và lập trình với phần mềm Arduino qua mạch nạp Mtiny Programmer với chuẩn nạp Mtiny Socket.

> Mtiny là viết tắt của Maker Tiny là dự án tạo ra các mạch vi điều khiển với thiết kế nhỏ gọn sử dụng chuẩn chân cắm DIP 2.54mm, các mạch Mtiny cùng sử dụng chung mạch nạp chương trình và giao tiếp máy tính Mtiny Programmer với chuẩn nạp Mtiny Socket.

## Thông số kỹ thuật

<table><thead>
  <tr>
    <th>Model</th>
    <th>Mtiny Uno ATmega328P (Arduino Compatible)</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MCU</td>
    <td>ATmega328P</td>
  </tr>
  <tr>
    <td>Power Supply</td>
    <td>5V Pin: 4.5 ~ 5.5VDC, Typical 5VDC</td>
  </tr>
  <tr>
    <td>Interface</td>
    <td>UART/SPI/I2C/PWM</td>
  </tr>
  <tr>
    <td>Digital I/O Pins</td>
    <td>14 (of which 6 provide PWM output)</td>
  </tr>
  <tr>
    <td>PWM Digital I/O Pins</td>
    <td>6</td>
  </tr>
  <tr>
    <td>Analog Input Pins</td>
    <td>6</td>
  </tr>
  <tr>
    <td>DC Current per I/O Pin</td>
    <td>20 mA</td>
  </tr>
  <tr>
    <td>Flash Memory</td>
    <td>32 KB (ATmega328P) of which 0.5 KB used by bootloader</td>
  </tr>
  <tr>
    <td>SRAM</td>
    <td>2 KB (ATmega328P)</td>
  </tr>
  <tr>
    <td>EEPROM</td>
    <td>1 KB (ATmega328P)</td>
  </tr>
  <tr>
    <td>Clock Speed</td>
    <td>16 MHz</td>
  </tr>
  <tr>
    <td>LED_BUILTIN</td>
    <td>13</td>
  </tr>
  <tr>
    <td>Packet</td>
    <td>DIP26 (13x2) 2.54mm</td>
  </tr>
  <tr>
    <td>Programmer</td>
    <td><a href="https://wiki.makerlab.vn/index.php/M%E1%BA%A1ch_Mtiny_Programmer_(Arduino_Compatible)" target="_blank" rel="noopener noreferrer">Mạch Mtiny Programmer (Arduino Compatible)</a></td>
  </tr>
  <tr>
    <td>Programmer Connector</td>
    <td>Mtiny Socket - IDC 8-Pin (2x4)</td>
  </tr>
</tbody></table>

## Kích thước

![](/image/mtiny_328p_2.jpg)

## Các tính năng vượt trội

1) Thiết kế nhỏ gọn với chuẩn chân cắm DIP 2.54mm, tương thích với hầu hết các loại BreadBoard thông dụng.

2) Thuộc Series Mtiny nên cùng sử dụng chung mạch nạp chương trình và giao tiếp máy tính Mtiny Programmer với chuẩn nạp Mtiny Socket.

3) Bổ sung thêm các linh kiện giúp ổn định, chống nhiễu.

4) Sau khi đã nạp chương trình, có thể cấp nguồn linh hoạt cho mạch bằng mạch Mtiny Power (6~24VDC) hoặc cấp nguồn trực tiếp qua chân 3V3 (3~3.3VDC).

## Hình ảnh

![](/image/mtiny_328p_3.jpg)

## Hướng dẫn sử dụng

### Hướng dẫn hàn Mtiny Socket và kết nối với Mạch Mtiny Programmer cho Mạch Mtiny Uno

- Mạch Mtiny Uno sử dụng mạch nạp Mtiny Programer với chuẩn nạp Mtiny Socket để nạp chương trình và cấp nguồn bằng máy tính, hàn Mtiny Socket sử dụng rào đực đôi Header 2x4pins theo chiều hướng lên và kết nối như sau:
![](/image/mtiny_328p_4.jpg)

### Hướng dẫn nạp chương trình với Arduino sử dụng mạch Mtiny Programmer

#### Hướng dẫn sử dụng phần mềm Arduino cơ bản

1) Giới thiệu về Arduino

2) Ngôn ngữ lập trình Arduino

3) Cách cài đặt phần mềm Arduino IDE

4) Cách cài đặt Driver và nạp chương trình cho mạch Arduino / Arduino Compatible

5) Cách cài đặt các thư viện phần cứng Arduino Library

6) Cách sử dụng Serial Monitor & Serial Plotter trên phần mềm Arduino

#### Hướng dẫn kết nối và nạp chương trình cho Mạch Vietduino Uno trên phần mềm Arduino

1) Kết nối máy tính: Kết nối Mạch Mtiny Uno với Mạch Mtiny Programmer bằng cáp IDC 2x4pins, kết nối Mạch Mtiny Programmer với máy tính bằng cáp USB-C sẽ thấy Led nguồn PWR trên mạch Mtiny Programmer và Mtiny Uno phát sáng:

![](/image/mtiny_328p_5.jpg)

2) Cài đặt Driver: Mạch Mtiny Programmer sử dụng IC nạp chương trình và giao tiếp máy tính CH340, các bạn có thể tham khảo hướng dẫn cài đặt Driver tại đây cho hệ điều hành Windows, lưu ý hệ điều hành MacOS hoặc Linux sẽ tự nhận Driver mà không cần cài đặt.

3) Cấu hình mạch trên phần mềm Arduino: Để cấu hình mạch trên phần mềm Arduino chúng ta cần làm các bước sau:

- Thiết lập Board tại Tools > Board > Arduino AVR Boards > Arduino Uno và Port (cổng kết nối) cho mạch, nếu không xác định được cổng kết nối có thể ngắt kết nối Mạch Mtiny Programmer và kết nối lại đồng thời kiểm tra phần Port để thấy cổng kết nối mới của mạch xuất hiện:

![](/image/mtiny_328p_6.jpg)

- Sau khi đã hoàn thành các thiết lập cơ bản bạn có thể nạp chương trình Blink sau vào mạch để test bằng cách nhấn vào nút Upload hoặc chọn Sketch > Upload sẽ thấy Led được kết nối với chân D13 trên mạch chớp tắt 1 giây 1 lần:

```ino
/*
  Blink
  Turns an LED_BUILTIN on D13 of Vietduino Uno for one second, then off for one second, repeatedly.
*/
// the setup function runs once when you press reset or power the board
void setup() {
  // initialize digital pin LED_BUILTIN on D13 as an output.
  pinMode(13, OUTPUT);
}

// the loop function runs over and over again forever
void loop() {
  digitalWrite(13, HIGH);  // turn the LED on (HIGH is the voltage level)
  delay(1000);                      // wait for a second
  digitalWrite(13, LOW);   // turn the LED off by making the voltage LOW
  delay(1000);                      // wait for a second
}
```

![](/image/mtiny_328p_7.jpg)

### Hướng dẫn cấp nguồn sử dụng mạch Mtiny Power sau khi đã nạp chương trình

Trong các trường hợp đã nạp chương trình (không cần sử dụng đến mạch nạp), muốn cấp nguồn riêng cho các mạch Mtiny và các mạch khác trong hệ thống, các bạn có thể sử dụng mạch Mtiny Power kết nối với các chân 3V3-5V-GND trên Mtiny Socket như sau:

<table><thead>
  <tr>
    <th>Power Input</th>
    <th>USB-C: 5VDC (Support USB Power Bank)<br>Domino (VIN): 6~24VDC</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Power Output</td>
    <td>5VDC - Max 500mA (USB-C Input)<br>5VDC - Max 1500mA (Domino Input)<br>3.3VDC - Max 700mA</td>
  </tr>
</tbody>
</table>

![](/image/mtiny_328p_8.jpg)
## Nhà phân phối
Có thể mua Mạch Mtiny Uno ATmega328P (Arduino Compatible) tại các nhà phân phối sau:

- [Hshop.vn - Điện tử & Robot.](hshop.vn)
