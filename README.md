# 🎮 Game Luyện Tập Câu Đảo Ngữ

## 📝 Mô tả dự án

Một trò chơi tương tác trực tuyến giúp học sinh luyện tập các dạng câu đảo ngữ trong tiếng Anh. Game được thiết kế với giao diện thân thiện, hệ thống chấm điểm tự động và bảng xếp hạng toàn cục, kèm theo bảng điều khiển admin để theo dõi tiến độ học tập của người chơi.

## ✨ Tính năng chính

### 🎯 Hệ thống Game
- **Đăng nhập bắt buộc**: Người chơi phải nhập tên trước khi bắt đầu
- **3 cấp độ khó**: 
  - 🟢 Dễ (10 câu hỏi) - 5 điểm/câu
  - 🟡 Trung bình (15 câu hỏi) - 7 điểm/câu  
  - 🔴 Khó (20 câu hỏi) - 10 điểm/câu
- **Câu hỏi đa dạng**: Bao gồm các dạng câu đảo ngữ phổ biến:
  - Đảo ngữ với "Not only... but also"
  - Đảo ngữ với "Never", "Seldom", "Rarely"
  - Đảo ngữ với "Only when", "Only if"
  - Đảo ngữ với "So/Such", "No sooner"
  - Đảo ngữ với "Little", "Under no circumstances"

### 📊 Hệ thống Chấm điểm & Xếp loại
- **Xuất sắc** (90-100%): 🏆 Vàng
- **Giỏi** (80-89%): 🥈 Bạc
- **Khá** (70-79%): 🥉 Đồng
- **Trung bình** (60-69%): 📋 Cần cố gắng
- **Yếu** (<60%): 📚 Cần học thêm

### 👥 Bảng xếp hạng toàn cục
- Top 10 người chơi có điểm cao nhất
- Hiển thị tên, cấp độ, điểm số và xếp loại
- Dữ liệu được lưu trữ và chia sẻ giữa các phiên

### 🛡️ Hệ thống Admin bảo mật
- **Đăng nhập bảo mật**: Yêu cầu mật khẩu admin
- **Theo dõi người chơi**: Xem danh sách và thống kê chi tiết
- **Quản lý dữ liệu**: Xóa, reset, xuất dữ liệu
- **Phân tích hiệu suất**: Thống kê theo cấp độ và xếp loại

## 🚀 Hướng dẫn cài đặt

### Yêu cầu hệ thống
- Trình duyệt web hiện đại (Chrome, Firefox, Safari, Edge)
- Không cần cài đặt thêm phần mềm

### Cài đặt
1. **Clone repository**:
   ```bash
   git clone https://github.com/[username]/inversion-grammar-game.git
   cd inversion-grammar-game
   ```

2. **Chạy trực tiếp**:
   - Mở file `index.html` bằng trình duyệt
   - Hoặc sử dụng live server để phát triển

3. **Deploy lên web**:
   - Upload file `index.html` lên hosting
   - Hoặc sử dụng GitHub Pages, Netlify, Vercel

## 📖 Hướng dẫn sử dụng

### Cho Người chơi
1. **Truy cập game** và nhập tên của bạn
2. **Chọn cấp độ** phù hợp với trình độ
3. **Làm bài**: Đọc câu hỏi và chọn đáp án đúng
4. **Xem kết quả**: Điểm số và xếp loại hiển thị ngay
5. **Kiểm tra bảng xếp hạng** để so sánh với người khác

### Cho Admin
1. **Nhấn "Đăng nhập Admin"** ở giao diện chính
2. **Nhập mật khẩu**: `admin123` (mặc định)
3. **Quản lý hệ thống**:
   - Xem danh sách người chơi
   - Phân tích thống kê
   - Xuất dữ liệu
   - Reset hệ thống
4. **Đăng xuất** khi hoàn thành

## 🖼️ Screenshots

*Đang cập nhật screenshots...*

<!-- Thêm screenshots tại đây -->
![Game Interface](screenshots/game-interface.png)
![Admin Dashboard](screenshots/admin-dashboard.png)
![Leaderboard](screenshots/leaderboard.png)

## ⚙️ Cấu hình Admin

### Thay đổi mật khẩu Admin
Trong file `index.html`, tìm và sửa dòng:
```javascript
const ADMIN_PASSWORD = 'admin123'; // Thay đổi mật khẩu tại đây
```

### Tùy chỉnh câu hỏi
Câu hỏi được lưu trong mảng `questions` theo cấu trúc:
```javascript
{
    question: "Câu hỏi",
    options: ["A. Đáp án 1", "B. Đáp án 2", "C. Đáp án 3", "D. Đáp án 4"],
    correct: 0, // Index của đáp án đúng
    level: "easy" // easy, medium, hard
}
```

## 🛠️ Công nghệ sử dụng

- **HTML5**: Cấu trúc trang web
- **CSS3**: Styling và responsive design
- **JavaScript (ES6+)**: Logic game và tương tác
- **LocalStorage**: Lưu trữ dữ liệu cục bộ
- **Bootstrap Icons**: Icon set
- **Font Awesome**: Biểu tượng bổ sung

## 📁 Cấu trúc dự án

```
inversion-grammar-game/
│
├── index.html              # File chính chứa toàn bộ ứng dụng
├── README.md              # Tài liệu hướng dẫn
├── screenshots/           # Thư mục chứa ảnh minh họa
│   ├── game-interface.png
│   ├── admin-dashboard.png
│   └── leaderboard.png
└── LICENSE               # Giấy phép sử dụng
```

## 🤝 Đóng góp

Chúng tôi hoan nghênh mọi đóng góp! Để đóng góp:

1. **Fork** repository này
2. **Tạo branch** cho tính năng mới: `git checkout -b feature/amazing-feature`
3. **Commit** thay đổi: `git commit -m 'Add amazing feature'`
4. **Push** lên branch: `git push origin feature/amazing-feature`
5. **Tạo Pull Request**

### Ý tưởng đóng góp
- [ ] Thêm nhiều dạng câu đảo ngữ khác
- [ ] Tích hợp âm thanh và hiệu ứng
- [ ] Chế độ multiplayer
- [ ] Thống kê chi tiết hơn
- [ ] Xuất kết quả PDF
- [ ] Tích hợp với Google Classroom

## 📋 Todo List

- [ ] Thêm chế độ luyện tập không giới hạn thời gian
- [ ] Tích hợp API để lưu trữ dữ liệu cloud  
- [ ] Thêm câu hỏi có giải thích chi tiết
- [ ] Phát triển mobile app
- [ ] Hệ thống achievement/badge
- [ ] Chế độ thi đấu theo nhóm

## 📄 License

Dự án này được phân phối dưới giấy phép MIT. Xem file `LICENSE` để biết thêm chi tiết.

## 📞 Liên hệ

- **Email**: [your-email@example.com]
- **GitHub**: [https://github.com/[username]]
- **Website**: [your-website.com]

## 🙏 Lời cảm ơn

- Cảm ơn tất cả giáo viên tiếng Anh đã đóng góp ý kiến về nội dung câu hỏi
- Cảm ơn cộng đồng developer đã hỗ trợ và đóng góp
- Đặc biệt cảm ơn các học sinh đã tham gia test và phản hồi

---

⭐ **Nếu dự án hữu ích, hãy star repository này!** ⭐

---

*Phát triển với ❤️ để giúp học sinh học tiếng Anh hiệu quả hơn*
