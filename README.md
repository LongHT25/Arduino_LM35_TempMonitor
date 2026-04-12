# 🌡️ Hệ Thống Giám Sát Nhiệt Độ LM35 (Arduino)

## 📖 Mô tả dự án
Dự án này sử dụng bo mạch Arduino Uno kết hợp với cảm biến nhiệt độ tương tự LM35 để thu thập dữ liệu nhiệt độ môi trường. Dữ liệu sau khi xử lý sẽ được đóng gói theo chuẩn định dạng JSON và truyền qua cổng Serial để giao tiếp với phần mềm máy tính (C#).

## ✨ Tính năng chính
- Đọc đồng thời 3 kênh cảm biến nhiệt độ (A0, A1, A2).
- Chuyển đổi giá trị ADC 10-bit sang nhiệt độ thực tế (°C).
- Xuất dữ liệu đa kênh chuẩn JSON dễ dàng parse (Bóc tách).

## 🛠️ Phần cứng sử dụng
| STT | Tên linh kiện      | Số lượng | Ghi chú                     |
| --- | ---                | ---      | ---                         |
| 1   | Arduino Uno R3     | 1        | Bo mạch vi điều khiển chính |
| 2   | Cảm biến LM35      | 3        | Cảm biến nhiệt độ Analog    |
| 3   | Dây cắm Breadboard | N/A      | Kết nối mạch                |

## 🚀 Hướng dẫn sử dụng
1. Mở thư mục `firmware` và nạp mã nguồn `.ino` vào bo mạch Arduino.
2. Kết nối chân VCC, GND của 3 cảm biến LM35 vào nguồn 5V của Arduino.
3. Kết nối chân OUT của 3 cảm biến lần lượt vào chân A0, A1, A2.
4. Mở Serial Monitor với baudrate `9600` để xem dữ liệu JSON.

## 📂 Cấu trúc thư mục
- `firmware/`: Chứa mã nguồn C++ chạy trên Arduino.
- `pc_app/`: Chứa phần mềm giao diện máy tính (C#).
- `simulation/`: Chứa file mô phỏng sơ đồ mạch trên Proteus.
- `docs/`: Tài liệu tham khảo dự án.

## 👥 Thành viên nhóm
- **Trương Hoàng Long** (N23DCCI043) - Nhóm trưởng
- **Nguyễn Đức Lương** (N23DCCI044) - Thành viên hỗ trợ