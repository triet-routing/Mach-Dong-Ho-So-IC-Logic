# Mô hình Mạch Đồng hồ số sử dụng IC Logic | 04-2025

> Đồ án Kỹ thuật - Chuyên ngành Điện tử Công nghiệp.
> Hệ thống hiển thị thời gian thực (Ngày : Giờ : Phút : Giây) xây dựng hoàn toàn từ các linh kiện số rời rạc.

## Giới thiệu Tổng quan
Dự án tập trung vào việc thiết kế và thi công mạch đồng hồ số không sử dụng vi điều khiển. Toàn bộ hệ thống được vận hành dựa trên các IC logic chức năng, từ khâu tạo xung chuẩn đến các tầng đếm và giải mã hiển thị trên LED 7 đoạn. Đây là giải pháp giúp tối ưu hóa việc hiểu sâu về nguyên lý kỹ thuật số và cấu trúc các bộ đếm.
<img width="983" height="493" alt="PCB_hinhanh" src="https://github.com/user-attachments/assets/3b5bc93c-f7c0-4d23-9ffb-12c76ea7131b" />
<img width="980" height="499" alt="machhoanchinh" src="https://github.com/user-attachments/assets/80bb9c63-bd36-44b4-89fe-36ba76963c2a" />

## Các tính năng chính
* **Hiển thị đầy đủ thông số:** Theo dõi Ngày, Giờ, Phút, Giây trực quan qua hệ thống 8 LED 7 đoạn.
* **Xung nhịp thạch anh chính xác:** Sử dụng thạch anh 32.768kHz kết hợp IC chia tần để tạo xung nhịp 1Hz ổn định tuyệt đối.
* **Hiệu chỉnh thủ công:** Tích hợp hệ thống nút nhấn cho phép cài đặt lại thời gian theo ý muốn người dùng.
* **Nguồn ổn áp an toàn:** Mạch nguồn thiết kế riêng biệt chuyển đổi từ 220VAC sang 5VDC, có tản nhiệt cho IC ổn áp 7805.

## Ngân xếp Công nghệ (Linh kiện chủ đạo)
* **Bộ đếm (Counter):** IC 74LS90 (Bộ đếm thập phân).
* **Bộ giải mã (Decoder):** IC 74247 (BCD to 7-segment).
* **Tạo xung & Chia tần:** IC 4060, IC 4013 kết hợp thạch anh 32.768kHz.
* **Cổng logic điều kiện:** IC 74HC08 (AND), IC 74LS86 (XOR).
* **Hiển thị:** LED 7 đoạn Anode chung.
* **Công cụ thiết kế:** Proteus, Altium Designer.



## Cấu trúc Thư mục
├── schematic/         # Bản vẽ sơ đồ nguyên lý (Proteus/PDF)
├── pcb_layout/        # Bản vẽ mạch in PCB
├── docs/              # Tài liệu báo cáo (.doc) và slide thuyết trình (.ppt)
└── images/            # Hình ảnh thực tế của mạch sau thi công
