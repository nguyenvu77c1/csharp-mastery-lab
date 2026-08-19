# 🌐 HƯỚNG DẪN DEPLOY WEB APP LÊN INTERNET (MIỄN PHÍ 100%)

Trang web **C# Mastery Lab & AI Learning Platform** là một ứng dụng **Standalone SPA (Single Page Application)** chạy trực tiếp trên trình duyệt, không cần backend server phức tạp. Bạn có thể deploy lên internet hoàn toàn miễn phí chỉ trong 1 phút để truy cập trên điện thoại (4G/5G/Wifi khác mạng) bất cứ khi nào!

---

## 🚀 CÁCH 1: Kéo thả lên Netlify Drop (Đơn giản nhất - Không cần tài khoản Git - 30 giây)

1. Truy cập trang web miễn phí: **[https://app.netlify.com/drop](https://app.netlify.com/drop)**
2. Mở thư mục `d:\CODE\CSharp\` trên máy tính.
3. Kéo thả file `index.html` (hoặc kéo cả thư mục `d:\CODE\CSharp`) thả vào ô vòng tròn trên trang Netlify Drop.
4. Đợi 5 giây, Netlify sẽ cấp cho bạn một đường link website online vĩnh viễn (Ví dụ: `https://csharp-mastery-lab.netlify.app`).
5. **Mở link đó trên điện thoại** là có thể học và chat với AI Gemini mọi lúc mọi nơi!

---

## 🚀 CÁCH 2: Deploy qua Vercel (Tốc độ cao nhất & Miễn phí)

1. Truy cập **[https://vercel.com](https://vercel.com)** và đăng nhập.
2. Cài đặt Vercel CLI (nếu muốn deploy bằng 1 dòng lệnh terminal):
   ```bash
   npm i -g vercel
   cd d:\CODE\CSharp
   vercel deploy --prod
   ```
3. Hoặc kéo thả project lên Vercel Dashboard -> Nhận ngay link `https://csharp-lab.vercel.app`.

---

## 🚀 CÁCH 3: Deploy lên GitHub Pages (Miễn phí vĩnh viễn)

1. Tạo một repository mới trên GitHub (Ví dụ: `csharp-mastery-lab`).
2. Push file `index.html` lên nhánh `main`:
   ```bash
   cd d:\CODE\CSharp
   git init
   git add index.html
   git commit -m "Deploy CSharp Mastery Lab"
   git branch -M main
   git remote add origin https://github.com/<username>/csharp-mastery-lab.git
   git push -u origin main
   ```
3. Vào **Settings** của Repo trên GitHub -> chọn tab **Pages** -> mục **Branch** chọn `main` -> bấm **Save**.
4. Sau 1 phút, bạn sẽ có link: `https://<username>.github.io/csharp-mastery-lab/`.

---

## 🚀 CÁCH 4: Chạy Local Host + Mở ra Internet qua Cloudflare Tunnel / ngrok (Không cần deploy)

Nếu bạn muốn chạy server ngay trên máy tính và mở link ra cho điện thoại truy cập:
1. Mở Terminal PowerShell tại `d:\CODE\CSharp`:
   ```powershell
   npx serve .
   ```
2. Dùng Cloudflare Tunnel (Miễn phí, không cần tài khoản):
   ```powershell
   npx cloudflared tunnel --url http://localhost:3000
   ```
3. Cloudflare sẽ in ra một đường link công khai dạng `https://xyz.trycloudflare.com` để bạn mở trên điện thoại!

---

## 📱 LƯU Ý KHI SỬ DỤNG TRÊN ĐIỆN THOẠI:
- Khi mở trên điện thoại, bấm nút **`☰` ở góc trên bên trái** để mở danh mục 26 bài học.
- Bấm nút **`🤖 Chat với AI` ở góc dưới bên phải** để mở toàn màn hình chat với Gemini Copilot.
- Bấm nút **`AI Key`** trên Topbar để dán các key Gemini của bạn vào (Dữ liệu API key được lưu an toàn riêng trong bộ nhớ trình duyệt điện thoại của bạn).
- Hỗ trợ lưu màn hình chính dạng Web App (PWA): Trên Safari iPhone bấm *Chia sẻ -> Thêm vào MH chính*, trên Android Chrome bấm *Menu 3 chấm -> Thêm vào màn hình chính*.
