XE DÒ LINE GIẢI MÃ MÊ CUNG

Xe khả năng dò line và chạy theo line màu đen. Và đi khám phá line theo thuật toán rồi tự tìm đường ra khỏi mê cung theo thuật toán.

Mục tiêu dự án là làm nghiên cứu khoa học Tại Trường Học Viện Công Nghệ Bưu Chính Viễn Thông cơ sở TP.HCM.

Ngoài mục tiêu trên, muốn tham gia thực hiện một đồ án cùng với đội nhóm lần đầu tiên cũng như áp dụng các kiến thức mình có thể học vào trong đồ án ở năm 2 đại học.


TÍNH NĂNG CHÍNH:

  
  Do line.
  
  
  Di chuyển theo Line.
  
  
  Lưu trữ Line.
  
  
  Giải Mã Line.

PHẦN CỨNG CẦN THIẾT:
  
  
  Arduino Nano | 1 | Mạch điều khiển chính.
  
  
  Mạch Mở Rộng Arduino Nano Shield V3.0 | 1 | Mạch mở rộng.
  
  
  TCRT5000 Cảm Biến Dò Line | 3 | Dò line phân biệt line đặc biệt.
  
  
  QTR-8A CẢM BIẾN DÒ LINE 8 LED | 1 | Dò line.
  
  
  L298N Mạch Cầu H | 1 | Điều khiển động cơ.
  
  
  LM2596S Mạch Giảm Áp 3A | 1 | Cấp nguồn cho vi điều khiển và mạch điều khiển động cơ.
  
  
  Hộp Pin, Khay Pin 2x18650 Có Công Tắc | 1 | Đế pin.
  
  
  Khung Xe 3 Bánh 2 Động Cơ | 1 | Liên kết mọi thứ và là khung xe.


SƠ ĐỒ KẾT NỐI:

  <img width="1919" height="1433" alt="image" src="https://github.com/user-attachments/assets/ca32a341-0762-4179-b9ee-beff8be3f2e2" />.
  
PHẦN MỀM VÀ THƯ VIỆN:
  1. Môi trường:
    Môi trường phát triển: Arduino IDE.
    Framework: Arduino.
  
  2. Cấu hình:
    Mở file sketch_sep21a.ino.
    Thay đổi các chân đầu vào của động cơ theo code dưới:
      #define dct1 5  // động cơ bên trái tiền (1)
      #define dct2 6  // động cơ bên trai lui (1)
      #define dct 9   // tốc độ động cơ trái
      #define dcp1 7  //động cơ bên phải tiền (1)
      #define dcp2 8  //động cơ bên phải lui (1)
      #define dcp 10  //tốc độ động cơ phải

    Thay đổi tốc độ của động cơ (độ ổn định thì đúng hơn):
        const int TOCDO = 97;
        
    Thay đổi các chân đầu vào của cảm biến (lưu ý 3 số cuối là của cảm biến TCRT5000) 
      uint8_t cambien[11] = { A0, A1, A2, A3, A4, A5, A6, A7, 3, 4, 11 };
    
     

  



