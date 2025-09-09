# XE DÒ LINE GIẢI MÃ MÊ CUNG


Xe khả năng dò line và chạy theo line màu đen. Và đi khám phá line theo thuật toán Left Hand rồi tự rút ngắn lại theo thuật toán.  
Mục tiêu dự án là làm nghiên cứu khoa học Tại Trường Học Viện Công Nghệ Bưu Chính Viễn Thông cơ sở TP.HCM.  
Ngoài mục tiêu trên, muốn tham gia thực hiện một đồ án cùng với đội nhóm lần đầu tiên cũng như áp dụng các kiến thức mình có thể học vào trong đồ án ở năm 2 đại học.  

## TÍNH NĂNG CHÍNH: 
- Do line.
- Di chuyển theo Line.  
- Lưu trữ line.
- Giải mã line tìm đường ra khỏi line.
  
## PHẦN CỨNG CẦN THIẾT:  
| Tên Linh Kiện | Ghi Chú | Số Lượng |
| :--- | :--- | :---: |
| Arduino Nano | Mạch điều khiển chính | 1 |
| Mạch Mở Rộng Arduino Nano Shield V3.0 | Mạch mở rộng | 1 |  
| TCRT5000 Cảm Biến Dò Line | Dò line phân biệt line đặc biệt | 3 |
| QTR-8A CẢM BIẾN DÒ LINE 8 LED | Dò line | 1 |
| L298N Mạch Cầu H | Điều khiển động cơ | 1 |
| LM2596S Mạch Giảm Áp 3A | Cấp nguồn cho vi điều khiển và mạch điều khiển động cơ | 1 | 
| Hộp Pin, Khay Pin 2x18650 Có Công Tắc | Đế pin | 1 |
| Khung Xe 3 Bánh 2 Động Cơ | Liên kết mọi thứ và là khung xe | 1 |

## SƠ ĐỒ KẾT NỐI:

  <img width="1919" height="1433" alt="image" src="https://github.com/user-attachments/assets/ca32a341-0762-4179-b9ee-beff8be3f2e2" />
  
## PHẦN MỀM VÀ THƯ VIỆN:
### 1. Môi trường:  
Môi trường phát triển: Arduino IDE.  
Framework: Arduino.   
  
### 2. Cấu hình:  
Mở file sketch_sep21a.ino.  
Thay đổi các chân đầu vào của động cơ theo code dưới:
``` c++
      #define dct1 5  // động cơ bên trái tiền (1)
      #define dct2 6  // động cơ bên trai lui (1)
      #define dct 9   // tốc độ động cơ trái
      #define dcp1 7  //động cơ bên phải tiền (1)
      #define dcp2 8  //động cơ bên phải lui (1)
      #define dcp 10  //tốc độ động cơ phải
```
Thay đổi tốc độ của động cơ (độ ổn định thì đúng hơn):  
```c++
const int TOCDO = 97;
```
Thay đổi các chân đầu vào của cảm biến (lưu ý 3 số cuối là của cảm biến TCRT5000) 
```c++
uint8_t cambien[11] = { A0, A1, A2, A3, A4, A5, A6, A7, 3, 4, 11 };
```
### 3. Biên dịch và Nạp code:
Chọn đúng 'Board' và cổng 'COM'.  
Nhấn nút 'Upload' để biên dịch và nạp chương trình vào vi điều khiển.  

## Cách sử dụng:  
-  Lắp hai pin 18650 vào đế pin.
-  Bật công tắc.
-  Cho xe vào line.
-  Đợi xe giải mã.
-  Xe quay đầu về vạch xuất phát.
-  Xe đi ra khỏi mê cung theo đường đã rút gọn.
-  Link video: https://youtu.be/IJJcZgNXqVM
  
## Cấu trúc thư mục:
|-- sketch_sep21a.ino

## Các thành viên trong nhóm:
Trần Quốc Cường  
Nguyễn Việt Thành

## Liên hệ:
Tên: Trần Quốc Cường  
Email: tranquoccuong103111@gmail.com  
GitHub: github.com/TranQuoc-Cuong
  



