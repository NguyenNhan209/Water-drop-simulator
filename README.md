# 💧 Water Pouring Simulator

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Canvas_API-FF6B6B?style=for-the-badge&logo=html5&logoColor=white" alt="Canvas" />
</p>

<h3 align="center">🌊 Mô phỏng rót nước tương tác – Dự án Khoa học kỹ thuật 2025</h3>

<p align="center">
  <img width="1557" alt="Water Pouring Simulator Demo" src="https://github.com/user-attachments/assets/4fdd65c5-2960-4352-a07a-21e03ff7e63f" />
</p>

---

## 📋 Mục lục

- [🌊 Giới thiệu](#-giới-thiệu)
- [✨ Tính năng nổi bật](#-tính-năng-nổi-bật)
- [🎯 Mục tiêu dự án](#-mục-tiêu-dự-án)
- [⚙️ Công nghệ sử dụng](#️-công-nghệ-sử-dụng)
- [🚀 Cách chạy dự án](#-cách-chạy-dự-án)
- [🎮 Hướng dẫn sử dụng](#-hướng-dẫn-sử-dụng)
- [🖼️ Ảnh minh họa](#️-ảnh-minh-họa)
- [🔧 Cấu trúc dự án](#-cấu-trúc-dự-án)
- [👥 Thành viên nhóm](#-thành-viên-nhóm)
- [📝 Changelog](#-changelog)
- [🧾 License](#-license)
- [🌟 Ghi công](#-ghi-công)

---

## 🌊 Giới thiệu

**Water Pouring Simulator** là một ứng dụng mô phỏng tương tác quá trình **rót nước từ bình vào cốc**, được xây dựng hoàn toàn bằng **HTML5 Canvas, CSS3 và Vanilla JavaScript** mà không sử dụng thư viện bên ngoài.

Dự án tập trung vào việc mô phỏng vật lý thực tế như:
- 🌀 **Hiệu ứng sóng nước động** (animated water waves)
- ⚖️ **Chuyển nước giữa các vật chứa** (liquid transfer)
- 📐 **Góc nghiêng tự động** của bình khi rót
- 📏 **Cốc đo có vạch chia chính xác** (1000ml với 10 vạch chia)
- 🎨 **Giao diện hiện đại** với gradient và glassmorphism

---

## ✨ Tính năng nổi bật

### 🎨 Giao diện và UX
- ✅ Thiết kế hiện đại với **gradient màu xanh dương** chủ đạo
- ✅ **Glassmorphism effect** (backdrop-filter) cho panel và overlay
- ✅ **Responsive design** - hoạt động tốt trên desktop và mobile
- ✅ **Smooth animations** với cubic-bezier transitions
- ✅ **Toast notification** hướng dẫn người dùng lần đầu
- ✅ **Help panel modal** chi tiết với SVG illustrations

### 🧪 Chức năng chính
- ✅ **Kéo thả (Drag & Drop)** bình và cốc để di chuyển
- ✅ **Rót nước tự động** khi bình nghiêng đúng góc và vị trí
- ✅ **Hiệu ứng sóng nước thời gian thực** (sine wave animation)
- ✅ **Thêm/xóa cốc động** (tối đa 5 cốc)
- ✅ **2 loại cốc**:
  - 🥤 Cốc thường (dung tích tùy chỉnh)
  - 📏 Cốc đo 1 lít (có vạch chia 0-1000ml)
- ✅ **Chuyển đổi đơn vị** ml ↔ lít (riêng biệt cho từng đối tượng)
- ✅ **Ẩn/hiện thông tin đơn vị đo** hàng loạt hoặc từng cốc
- ✅ **Settings panel** với các tùy chỉnh:
  - Mức nước hiện tại
  - Dung tích tối đa
  - Đơn vị đo (ml/lít)
  - Hiển thị/ẩn thông tin
  - Bật/tắt vạch chia (cốc đo)

### 🎯 Logic vật lý
- ✅ Tự động **tính toán góc nghiêng** dựa trên vị trí cốc
- ✅ **Tốc độ rót điều chỉnh** theo đơn vị đo (ml nhanh hơn lít)
- ✅ **Giới hạn dung tích** - dừng rót khi cốc đầy
- ✅ **Kiểm tra điều kiện** trước khi rót:
  - Bình phải ở bên phải cốc
  - Góc trái trên bình phải cao hơn cạnh trên cốc
  - Bình phải nghiêng đủ góc (> 10°)
- ✅ **Highlight cốc đang được rót** bằng viền xanh

### 🖼️ Hình ảnh và đồ họa
- ✅ Sử dụng **PNG sprites** cho bình và cốc (empty/full)
- ✅ **Clip mask rendering** cho hiệu ứng nước thực tế
- ✅ **Gradient water effect** với màu xanh dương
- ✅ **Animated water stream** khi rót (gradient + sine wave)
- ✅ **Vạch chia chính xác** trên cốc đo (dựa trên tỷ lệ pixel thực tế)

---

## 🎯 Mục tiêu dự án

1. **Giáo dục STEM**: Giúp học sinh tiểu học hiểu về:
   - Khái niệm thể tích và dung tích
   - Chuyển đổi đơn vị đo (ml ↔ lít)
   - Nguyên lý rót nước (góc nghiêng, vị trí, trọng lực)

2. **Kỹ thuật lập trình**:
   - Thực hành **HTML5 Canvas API**
   - Xử lý **drag & drop** trên cả desktop và mobile
   - Quản lý **state phức tạp** với JavaScript
   - Thiết kế **UI/UX hiện đại** với CSS3

3. **Trải nghiệm người dùng**:
   - Giao diện trực quan, dễ sử dụng
   - Phản hồi thời gian thực
   - Hướng dẫn chi tiết cho người dùng mới

---

## ⚙️ Công nghệ sử dụng

| Công nghệ | Phiên bản | Mô tả |
|-----------|-----------|-------|
| **HTML5** | - | Structure và Canvas API |
| **CSS3** | - | Styling với Flexbox, Grid, Animations |
| **JavaScript (ES6+)** | - | Logic mô phỏng và xử lý sự kiện |
| **Canvas 2D Context** | - | Rendering đồ họa và animations |
| **LocalStorage API** | - | Lưu trạng thái tutorial |
| **Touch Events API** | - | Hỗ trợ mobile touch |

### 📦 Không sử dụng thư viện bên ngoài
- ❌ Không dùng jQuery, React, Vue
- ❌ Không dùng Three.js, PixiJS
- ✅ **100% Vanilla JavaScript**

---

## 🚀 Cách chạy dự án

### Phương pháp 1: Clone và chạy local

```bash
# Clone repository
git clone https://github.com/NguyenNhan209/Water-pouring-simulator.git

# Di chuyển vào thư mục dự án
cd Water-pouring-simulator

# Mở file index.html bằng trình duyệt
# Windows:
start index.html

# macOS:
open index.html

# Linux:
xdg-open index.html
```

### Phương pháp 2: Live Server (khuyến nghị)

```bash
# Cài đặt Live Server (nếu chưa có)
npm install -g live-server

# Chạy server
live-server
```

### Phương pháp 3: Truy cập trực tuyến

🌐 **Demo online**: [https://nguyennhan209.github.io/Water-pouring-simulator](https://nguyennhan209.github.io/Water-drop-simulator/)

---

## 🎮 Hướng dẫn sử dụng

### 1️⃣ Cách rót nước
1. **Kéo bình nước** sang **bên phải** cốc
2. Đặt bình **cao hơn** cốc (góc trái trên bình phải cao hơn cạnh trên cốc)
3. Bình sẽ tự động **nghiêng** và rót nước
4. **Click vào bình** để kích hoạt chế độ rót (với cốc mới tạo)

### 2️⃣ Thêm/Xóa cốc
- Nhấn **"+ Cốc thường"** để thêm cốc bình thường
- Nhấn **"📏 Cốc đo 1L"** để thêm cốc có vạch chia
- Tối đa **5 cốc** cùng lúc
- Xóa cốc trong **⚙ Cài đặt → chọn cốc → 🗑 Xóa**

### 3️⃣ Cài đặt
- Điều chỉnh **dung tích** và **mức nước** của bình/cốc
- Chuyển đổi **đơn vị** giữa ml và lít
- Ẩn/hiện **thông tin đơn vị đo** trên màn hình
- Bật/tắt **vạch chia** trên cốc đo 1L

### 4️⃣ Thao tác khác
- **Kéo thả** bình và cốc để di chuyển vị trí
- Nhấn **"↺ Reset"** để khởi động lại
- Nhấn **"✓ Áp dụng"** trong Cài đặt để lưu thay đổi

---

## 🖼️ Ảnh minh họa

<p align="center">
  <img width="800" alt="Main Interface" src="https://github.com/user-attachments/assets/f1da425c-47bb-4cfd-9cf6-07cb2a3c98af" />
  <br><em>Giao diện chính với bình nước và cốc</em>
</p>

<p align="center">
  <img width="800" alt="Pouring Animation" src="https://github.com/user-attachments/assets/4fdd65c5-2960-4352-a07a-21e03ff7e63f" />
  <br><em>Hiệu ứng rót nước với sóng động</em>
</p>

<p align="center">
  <img width="800" alt="Settings Panel" src="https://github.com/user-attachments/assets/aa927a43-ecac-4b36-b4b4-4a111e05e692" />
  <br><em>Panel cài đặt chi tiết</em>
</p>

---

## 🔧 Cấu trúc dự án

```
Water-pouring-simulator/
│
├── index.html              # File HTML chính (bao gồm CSS và JS inline)
├── README.md               # File này
└── LICENSE                 # Giấy phép GPL v3.0
```

### 📊 Thống kê code

- **HTML/CSS/JS**: ~1600 dòng (trong 1 file)
- **Total size**: ~500KB (chưa nén)

---

## 👥 Thành viên nhóm

<table>
  <tr>
    <th>Họ tên</th>
    <th>Vai trò</th>
    <th>Trường</th>
    <th>Email</th>
  </tr>
  <tr>
    <td><strong>Nguyễn Nhân</strong></td>
    <td>Lập trình chính, Thiết kế giao diện, Mô phỏng vật lý</td>
    <td>Trường Tiểu học Nguyễn Trãi</td>
    <td><a href="mailto:nguyennhan24912@gmail.com">nguyennhan24912@gmail.com</a></td>
  </tr>
  <tr>
    <td><strong>Phạm Hồng Khanh</strong></td>
    <td>Ý tưởng dự án, Thiết kế đồ họa, Kiểm thử</td>
    <td>Trường Tiểu học Nguyễn Trãi</td>
    <td><a href="mailto:phamhongkhanh200586@gmail.com">phamhongkhanh200586@gmail.com</a></td>
  </tr>
</table>

---

## 📝 Changelog

### v1.0.0 (2025-01-XX) - Initial Release
- ✅ Mô phỏng rót nước cơ bản
- ✅ Drag & drop bình và cốc
- ✅ Hiệu ứng sóng nước động
- ✅ Settings panel với tùy chỉnh chi tiết
- ✅ 2 loại cốc: thường và cốc đo
- ✅ Chuyển đổi đơn vị ml/lít
- ✅ Toast notification và help panel
- ✅ Responsive design cho mobile
- ✅ Lưu trạng thái vào LocalStorage
### Planned Features (v1.1.0)
- 🔜 Thêm âm thanh rót nước
- 🔜 Chế độ thử thách (đổ đúng lượng nước)
- 🔜 Thêm nhiều loại cốc khác nhau
- 🔜 Export/Import cấu hình

---

## 🧾 License

This project is licensed under the **GNU General Public License v3.0**.

```
Copyright (C) 2025  Nguyễn Nhân, Phạm Hồng Khanh

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.
```

Xem chi tiết tại [LICENSE](LICENSE) file.

### ⚖️ Điều khoản chính:
- ✅ **Sử dụng tự do** cho mục đích học tập và nghiên cứu (không thương mại)
- ✅ **Sửa đổi và phân phối** với điều kiện giữ nguyên license
- ✅ **Mã nguồn mở** - phải công khai code khi phân phối
- ❌ **Không bảo hành** - sử dụng với trách nhiệm riêng

---

## 🌟 Ghi công

### 🏫 Tổ chức
- **Trường Tiểu học Nguyễn Trãi**
- Thành phố Hải Phòng, Việt Nam
- Năm thực hiện: **2025**

### 📧 Liên hệ
- **Email**: [nguyennhan24912@gmail.com](mailto:nguyennhan24912@gmail.com)
- **GitHub**: [@NguyenNhan209](https://github.com/NguyenNhan209)

---

<p align="center">
  <strong>💬 "Code is like water — it flows, adapts, and reflects creativity."</strong>
  <br><br>
  <img src="https://img.shields.io/github/stars/NguyenNhan209/Water-pouring-simulator?style=social" alt="Stars" />
  <img src="https://img.shields.io/github/forks/NguyenNhan209/Water-pouring-simulator?style=social" alt="Forks" />
  <br>
  <sub>Made with ❤️ by Nhân & Khanh</sub>
</p>

---

### 🔗 Quick Links

- [📥 Download ZIP](https://github.com/NguyenNhan209/Water-pouring-simulator/archive/refs/heads/main.zip)
- [🐛 Report Bug](https://github.com/NguyenNhan209/Water-pouring-simulator/issues)
- [💡 Request Feature](https://github.com/NguyenNhan209/Water-pouring-simulator/issues)
- [🌐 Live Demo](https://nguyennhan209.github.io/Water-drop-simulator/)

---

<p align="center">
  <i>If you found this project useful, please consider giving it a ⭐️!</i>
</p>
