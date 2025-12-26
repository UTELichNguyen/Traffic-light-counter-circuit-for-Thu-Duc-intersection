# Traffic Light Control System - Circuit Details

## 1. Schematic Diagram - Block 1 (Sơ đồ nguyên lý - Khối 1)
Dưới đây là sơ đồ nguyên lý của khối mạch xử lý chính (Main Processing Block). Khối này đảm nhiệm chức năng đếm và xử lý logic cho hệ thống đèn.

<img width="1219" height="791" alt="Screenshot 2025-12-26 225220" src="https://github.com/user-attachments/assets/3bcad8f5-2908-4170-8dd1-0a929ebb59d7" />


**Mô tả hoạt động:** Mạch sử dụng kết hợp các IC đếm (74192, 7493) và IC cộng/giải mã (74LS83, 74HCT238) để điều khiển trạng thái logic.

---

## 2. Bill of Materials (Danh sách linh kiện)
Dưới đây là bảng thống kê linh kiện được sử dụng trong Block 1:

| Loại Linh Kiện (Category) | Tên Linh Kiện (Name) | Chức năng chính (Description) |
| :--- | :--- | :--- |
| **Counters (IC Đếm)** | `74192` | Synchronous Up/Down Decade Counter (Đếm lên/xuống) |
| | `7493` | 4-bit Binary Counter (Bộ đếm nhị phân 4-bit) |
| **Logic & Math ICs** | `74LS83` | 4-bit Binary Full Adder (Bộ cộng toàn phần 4-bit) |
| | `74HCT238` | 3-to-8 Line Decoder/Demultiplexer (Giải mã 3 sang 8) |
| | `74LS247` | BCD to 7-Segment Decoder (Giải mã LED 7 đoạn) |
| | `74LS386` | Quad 2-Input XOR Gates |
| **Logic Gates** | `AND`, `OR`, `OR_3` | Các cổng logic cơ bản |
| | `NOT`, `XOR` | Cổng đảo và cổng XOR |
| **Display & I/O** | `7SEG-BCD-GRN` | LED 7 đoạn (Màu xanh) |
| | `TRAFFIC LIGHTS` | Mô hình đèn giao thông |
| | `BUTTON` | Nút nhấn điều khiển |
| **Passive/Others** | `RES` (Resistor) | Điện trở |
| | `CAPACITOR` | Tụ điện |
| | `LOGICSTATE` | Đầu vào trạng thái Logic (0/1) |

---
