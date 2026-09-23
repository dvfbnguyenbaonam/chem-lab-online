# 🧪 ChemLab Online - Phòng Thí Nghiệm Hóa Học Ảo Trực Tuyến

Website phòng thí nghiệm Hóa học ảo hiện đại, mô phỏng trực quan các phản ứng hóa học (kết tủa, sủi bọt khí, đổi màu chỉ thị pH, phản ứng tỏa nhiệt,...), tích hợp âm thanh Web Audio, Bảng tuần hoàn tra cứu nguyên tố và Trắc nghiệm kiến thức Hóa học (Quiz).

---

## 🚀 Cách 1: Deploy lên Vercel qua Vercel CLI (Nhanh nhất)

Mở Terminal / PowerShell tại thư mục này và chạy lệnh:

```bash
# 1. Đăng nhập và deploy lên Vercel
npx vercel

# Khi được hỏi:
# ? Set up and deploy "..."? -> Yes (Y)
# ? Which scope do you want to deploy to? -> [Chọn tài khoản của bạn]
# ? Link to existing project? -> No (N)
# ? What's your project's name? -> chemlab-online
# ? In which directory is your code located? -> ./
# ? Want to modify these settings? -> No (N)

# 2. Để deploy thẳng lên Production với domain chính thức:
npx vercel --prod
```

Sau khi hoàn tất, Vercel sẽ gửi lại đường link trang web dạng: `https://chemlab-online.vercel.app`.

---

## 🌐 Cách 2: Deploy lên Vercel thông qua GitHub (Khuyên dùng)

1. **Đưa mã nguồn lên GitHub**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit ChemLab Online"
   git branch -M main
   git remote add origin https://github.com/<tai-khoan-cua-ban>/chem-lab-online.git
   git push -u origin main
   ```

2. **Kết nối Vercel**:
   - Truy cập [vercel.com](https://vercel.com) và đăng nhập bằng GitHub.
   - Nhấn **Add New...** -> **Project**.
   - Chọn kho lưu trữ `chem-lab-online` vừa tạo.
   - Framework Preset: Vercel sẽ tự động nhận diện **Vite**.
   - Nhấn **Deploy**. Chỉ sau 30 giây, website sẽ online toàn cầu!

---

## 🛠️ Chạy thử nghiệm ở môi trường Local (Máy tính của bạn)

```bash
# Khởi động máy chủ phát triển
npm run dev

# Mở trình duyệt và truy cập: http://localhost:5173
```

---

## ✨ Tính năng nổi bật

1. **Mô phỏng Dụng cụ Đa dạng**: Cốc đong (Beaker), Bình tam giác (Flask), Ống nghiệm (Test tube).
2. **Kệ Thuốc thử & Hóa chất Đầy đủ**: Axit (HCl, H₂SO₄, HNO₃, CH₃COOH), Bazơ (NaOH, Ba(OH)₂, NH₃), Muối (CuSO₄, FeCl₃, BaCl₂, AgNO₃, Na₂CO₃,...), Kim loại (Fe, Cu, Zn), Chỉ thị màu (Phenolphtalein, Quỳ tím).
3. **Hiệu ứng Phản ứng Đồ họa Đỉnh cao**:
   - Sủi bọt khí rào rào (H₂, CO₂, khí độc NO₂ màu nâu đỏ).
   - Xuất hiện kết tủa màu đặc trưng (Cu(OH)₂ xanh lam, Fe(OH)₃ nâu đỏ, BaSO₄ trắng sữa, AgCl vón).
   - Chuyển màu chỉ thị pH linh hoạt.
   - Phản ứng kinh điển: **Kem đánh răng con voi** (H₂O₂ + xúc tác KI bốc khói bọt trào ngược), Mạ đồng lên đinh sắt.
4. **Tiện ích Bổ trợ**:
   - Đèn cồn khò lửa & Nhiệt kế đo nhiệt độ phản ứng.
   - Máy khuấy từ xoay chất lỏng.
   - Âm thanh sống động (tiếng rót hóa chất, tiếng xèo sủi bọt, tiếng nổ bọt).
   - **Bảng tuần hoàn các nguyên tố hóa học**: Tra cứu số hiệu, khối lượng, chu kỳ, cấu hình electron.
   - **Thử thách Quiz**: Trắc nghiệm dự đoán hiện tượng hóa học kèm pháo hoa và hiệu ứng chúc mừng.
