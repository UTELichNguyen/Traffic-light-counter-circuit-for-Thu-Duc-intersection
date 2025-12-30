# 🚦 Hệ thống Đèn Giao Thông Ngã Tư Thủ Đức (Proteus Simulation)

> **Mô phỏng hệ thống điều khiển tín hiệu giao thông thực tế tại ngã tư Thủ Đức, TP.HCM sử dụng linh kiện Logic số (Digital Logic).**

![Status](https://img.shields.io/badge/Status-Completed-success)
![Tool](https://img.shields.io/badge/Simulation-Proteus_8.17+-blue)
![Type](https://img.shields.io/badge/Type-Digital_Logic-orange)

## 👨‍💻 Thông tin Sinh viên
* **Họ và tên:** Nguyễn Hồng Lịch
* **MSSV:** 24161298
* **Lớp/Khóa:** 2024
* **Trường:** Đại học Công nghệ Kỹ thuật TP.HCM (HCMUTE)
* **Ngành:** Công nghệ Kỹ thuật Điện tử Viễn thông

---

## 📝 Giới thiệu Dự án
Dự án này là bài tập lớn môn học, nhằm mục đích thiết kế và mô phỏng hệ thống đèn giao thông tại nút giao thông trọng điểm **Ngã tư Thủ Đức**. Hệ thống điều khiển luồng giao thông phức tạp bao gồm các hướng:
* Xa lộ Hà Nội (Song hành & Cầu vượt)
* Võ Văn Ngân
* Lê Văn Việt

Điểm đặc biệt của dự án là **không sử dụng Vi điều khiển (Microcontroller)** lập trình sẵn. Thay vào đó, toàn bộ logic điều khiển, bộ đếm thời gian và giải mã hiển thị đều được xây dựng từ các **IC số cơ bản (74xx Series)**, giúp minh họa rõ nét bản chất của mạch điện tử số.

## ⚙️ Nguyên lý hoạt động (Sơ đồ khối)
Hệ thống được thiết kế dựa trên các khối chức năng chính như sơ đồ dưới đây. Tín hiệu xung nhịp (Clock) được tạo ra và đưa vào các bộ đếm lùi, sau đó qua khối logic để điều khiển đèn và hiển thị ra LED 7 đoạn.

![So_Do_Khoi](https://github.com/user-attachments/assets/c7877037-04a2-41ad-90bf-7d923b2be542)


## 📸 Kết quả Mô phỏng
Dưới đây là giao diện mô phỏng thực tế trên Proteus. Hệ thống hiển thị đầy đủ thời gian đếm ngược và trạng thái đèn (Xanh - Vàng - Đỏ) cho tất cả các hướng của ngã tư.

![Ket_qua](https://github.com/user-attachments/assets/cd1e095d-31fc-45bd-ba33-193d76237361)


## 🛠️ Danh sách linh kiện chính
Dựa trên thiết kế, mạch sử dụng các nhóm linh kiện:

| Tên Linh Kiện | Mã IC | Chức năng |
| :--- | :--- | :--- |
| **Bộ đếm** | `74192` | Đếm lùi thời gian (BCD Counter) |
| **Bộ cộng** | `74LS83` | Tính toán giá trị nạp |
| **Giải mã LED** | `74LS247` | Hiển thị ra LED 7 đoạn |
| **Giải mã địa chỉ**| `74HCT238`| Điều khiển luồng tín hiệu |
| **Logic** | `AND/OR/XOR` | Xử lý trạng thái đèn |

## 🚀 Hướng dẫn chạy mô phỏng
Để chạy được dự án này trên máy tính của bạn:

1.  **Yêu cầu phần mềm:** Cài đặt phần mềm **Proteus 8 Professional** (Bắt buộc phiên bản **8.17 trở lên** để tránh lỗi thư viện).
2.  **Tải dự án:**
    ```bash
    https://github.com/UTELichNguyen/Traffic-light-counter-circuit-for-Thu-Duc-intersection
    ```
---
