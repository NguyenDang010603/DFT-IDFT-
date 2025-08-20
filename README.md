# DFT-IDFT

Repo này triển khai **Discrete Fourier Transform (DFT)** và **Inverse Discrete Fourier Transform (IDFT)** để phân tích và tái tạo tín hiệu rời rạc.  
Mục tiêu chính là giúp hiểu rõ cơ chế biến đổi Fourier trên miền rời rạc và kiểm chứng việc khôi phục tín hiệu gốc từ miền tần số.

---

## 📌 Nội dung chính
- **Tính toán DFT**: Chuyển đổi tín hiệu từ miền thời gian sang miền tần số.  
- **Tính toán IDFT**: Khôi phục tín hiệu ban đầu từ miền tần số.  
- **So sánh**: Đối chiếu tín hiệu gốc và tín hiệu tái tạo sau IDFT để kiểm chứng.  
- **Biểu diễn trực quan**: Vẽ đồ thị tín hiệu trên cả miền thời gian và miền tần số.

---

## ⚙️ Cách hoạt động
1. Người dùng nhập vào một tín hiệu rời rạc (vector mẫu).  
2. Chương trình tính **DFT** bằng công thức ma trận hoặc vòng lặp:  

   X[k] = Σ (n=0 → N-1) x[n] * e^(-j2πkn/N)

3. Kết quả thu được là **phổ tần số** của tín hiệu.  
4. Từ phổ tần số, chương trình thực hiện **IDFT**:  

   x[n] = (1/N) Σ (k=0 → N-1) X[k] * e^(j2πkn/N)

5. So sánh tín hiệu tái tạo với tín hiệu gốc để kiểm chứng tính đúng đắn.  
6. Hiển thị đồ thị:
   - Tín hiệu gốc trên miền thời gian.  
   - Phổ biên độ và pha trên miền tần số.  
   - Tín hiệu tái tạo sau IDFT.  

---

## 🚀 Cách chạy chương trình
1. Clone repo về máy:
   ```bash
   git clone https://github.com/NguyenDang010603/DFT-IDFT-.git
   ```
2. Mở trong MATLAB hoặc Octave.  
3. Chạy file `DFT.m` (hoặc file chính của bạn).  
4. Quan sát kết quả trên đồ thị.

---

## 🖼️ Kết quả kỳ vọng
- Đồ thị tín hiệu gốc.  
- Phổ biên độ/pha sau DFT.  
- Tín hiệu khôi phục được sau IDFT gần như trùng khớp tín hiệu gốc.  

---

## 📖 Ứng dụng
- Phân tích tín hiệu trong xử lý tín hiệu số (DSP).  
- Hiểu cơ chế của biến đổi Fourier trong thực tế.  
- Cơ sở cho các ứng dụng nâng cao như xử lý âm thanh, hình ảnh, truyền thông số.

---

## 👤 Tác giả
Nguyễn Đăng – Repo phục vụ học tập và minh họa nguyên lý DFT/IDFT.
