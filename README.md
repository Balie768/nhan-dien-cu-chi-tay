<h1 align="center">🖐 Hệ thống nhận diện cử chỉ tay trong thời
gian thực để điều khiển trình chiếu PowerPoint🎤 </h1>
<div align="center">

<p align="center">
  <img src="images/logoDaiNam.png" alt="DaiNam University Logo" width="200"/>
  <img src="images/LogoAIoTLab.png" alt="AIoTLab Logo" width="170"/>
</p>

[![Made by AIoTLab](https://img.shields.io/badge/Made%20by%20AIoTLab-blue?style=for-the-badge)](https://www.facebook.com/DNUAIoTLab)
[![Fit DNU](https://img.shields.io/badge/Fit%20DNU-green?style=for-the-badge)](https://fitdnu.net/)
[![DaiNam University](https://img.shields.io/badge/DaiNam%20University-red?style=for-the-badge)](https://dainam.edu.vn)
</div>

Dự án này sử dụng **MediaPipe**, **TensorFlow**, **OpenCV** và **PyAutoGUI** để nhận diện cử chỉ tay và điều khiển PowerPoint thông qua webcam. **Mô hình GAFormer** được huấn luyện để nhận diện **8 cử chỉ tay** khác nhau nhằm thực hiện các thao tác trên **PowerPoint** như chuyển slide, bắt đầu trình chiếu, tạm dừng, v.v.

## 🎯 Tính năng chính

-Ghi lại video cử chỉ tay và lưu keypoints vào CSV.

-Huấn luyện mô hình GAFormer sử dụng Gramian Angular Field (GAF) để chuyển đổi dữ liệu.

-Nhận diện cử chỉ tay trong thời gian thực.

-Điều khiển PowerPoint bằng các cử chỉ tay đã học.

## 📥 Cài đặt

### 🛠 Điều kiện tiên quyết

- 🐍 **Python** `3.7+` - Ngôn ngữ lập trình cốt lõi
- 💾 **RAM** `8GB+` - Được đề xuất cho hiệu suất tối ưu
- 🖥 **CPU** `4+ cores` - Để xử lý song song
- 📷 **Webcam** - Để sử dụng tính năng nhận diện cử chỉ ( **Webcam** hoặc **Camera** hoạt động tốt )
- 🎯 **PyAutoGUI** (pyautogui) – Để kiểm soát PowerPoint
- 🪟 **pygetwindow** (pygetwindow) – Cho quản lý window

## 🎥 Thiết lập dự án
#### 1.📦 Clone Dự án
```bash
https://github.com/Balie768/nhan-dien-cu-chi-tay
cd hand-gesture-mediapipe
```
#### 2.📚 Tải các thư viện python cần thiết
```bash
pip install opencv-python mediapipe numpy tensorflow pandas scikit-learn matplotlib pyautogui pygetwindow
```
## 🎥 Cách sử dụng
#### 1️⃣ Chạy chương trình thu thập dữ liệu
```bash
python getdata.py
```
#### 2️⃣ Huấn luyện mô hình
```bash
python train_model.py
```
#### 3️⃣ Chạy chương trình nhận diện cử chỉ
```bash
python hand_run.py
```
## 🖐 Các cử chỉ hỗ trợ
- ✅ **Call** - Màn hình đen (tạm dừng trình chiếu)
- ✅ **Finger_Gun** - Chuyển đến slide đầu tiên
- ✅ **Left** - Quay lại slide trước
- ✅ **OK** - Tiếp tục trình chiếu
- ✅ **Open** - Mở PowerPoint và bắt đầu trình chiếu
- ✅ **Right** - Chuyển slide tiếp theo
- ✅ **Stop** - Thoát trình chiếu
- ✅ **Thumbs_Up** - Chuyển đến slide cuối cùng
## 📌 Ghi chú
- Nhấn **'q'** để thoát chương trình nhận diện.
- Đảm bảo webcam hoạt động bình thường.
## 📝 License

© 2025 **Nhóm 5 - Lớp CNTT 1603** 🎓  
🏫 **Trường Đại học Đại Nam** 

