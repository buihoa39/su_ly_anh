# 🦆 Duck Hunt - Hand Control Game

Một trò chơi **Bắn Vịt** cổ điển được điều khiển bằng **cử chỉ tay** thông qua webcam, sử dụng **MediaPipe** và **OpenCV** kết hợp với **Pygame**. Người chơi dùng **ngón trỏ** làm tâm ngắm và **cử chỉ bàn tay** để bắn hoặc nạp đạn.

---

## 🎮 Tính năng chính

- 🎯 Điều khiển tâm ngắm bằng **ngón trỏ** qua webcam.
- 🤏 Bắn khi **ngón cái và ngón trỏ chạm nhau**.
- ✋ Nạp đạn khi **ngón cái và ngón trỏ cách xa nhau**.
- 🔫 Hai chế độ chơi:
  - **Classic Mode**: Bắn không giới hạn, tăng độ khó theo thời gian.
  - **Time Mode**: Giới hạn thời gian, qua từng level với mục tiêu cụ thể.
- 📈 Lưu điểm cao nhất vào file `highscore.txt`.
- 💥 Hiệu ứng trúng/miss, âm thanh sống động.
- 🧠 Giao diện menu linh hoạt điều khiển bằng chuột hoặc tay.

🎯 Giao diện chính
![giao diện chính]()
---

## 📦 Cài đặt

### 1. Cài Python

Yêu cầu Python 3.12 hoặc mới hơn.

### 2. Cài thư viện cần thiết

```bash
pip install pygame opencv-python mediapipe numpy
```

---

## 📁 Cấu trúc thư mục

```
DuckHunt/
│
├── main.py                # Mã nguồn chính
├── highscore.txt          # File lưu điểm cao
├── bg2.png                # Hình nền game
├── d1.png, d2.png         # Vịt bay bên phải
├── d3.png, d4.png         # Vịt bay bên trái
├── ot.png                 # Tâm ngắm
├── hit.png                # Hiệu ứng trúng
├── hit_sound.wav          # Âm thanh trúng
└── miss_sound.wav         # Âm thanh trượt
```

---

## 🕹️ Cách chơi

| Hành động        | Cách thực hiện                                       |
|------------------|------------------------------------------------------|
| Điều khiển tâm ngắm | Di chuyển **ngón trỏ** trước webcam                 |
| Bắn              | **Chạm ngón cái và ngón trỏ**                        |
| Nạp đạn          | **Tách ngón cái và ngón trỏ xa nhau**               |
| Chọn menu        | Di chuyển tay/chuột đến nút và **nhấp (giữ)**        |
| Khởi động lại    | Nhấn phím **R** khi đang chơi                       |

---

## 🧠 Một số lưu ý

- Chơi trong môi trường sáng tốt để **MediaPipe nhận diện tay chính xác**.
- Chỉ hỗ trợ **1 tay duy nhất** (tay phải được khuyến khích).
- Tâm ngắm được **làm mượt** để tránh rung lắc.

---

## 📸 Công nghệ sử dụng

- **Python**
- **Pygame** – Đồ họa và âm thanh
- **OpenCV** – Xử lý hình ảnh từ webcam
- **MediaPipe** – Nhận diện tay & cử chỉ
- **Multithreading** – Luồng riêng cho camera
