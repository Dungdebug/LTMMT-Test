# LTMMT-Test

Dự án học tập theo quy tắc quản lý repository Git của môn LTMMT.

## Mục tiêu
- Quản lý mã nguồn theo workflow chuẩn GitHub
- Theo dõi công việc bằng Issue
- Phân nhánh theo quy tắc cá nhân
- Review và merge thông qua Pull Request

## Quy định bắt buộc

### 1. Thông tin cá nhân
Mỗi sinh viên phải cấu hình git local đúng định danh:

```bash
git config --global user.name "MSSV_HoVaTen"
git config --global user.email "email_sinh_vien@domain"
```

Ví dụ:
```bash
git config --global user.name "23110001_NguyenVanA"
git config --global user.email "23110001@student.edu.vn"
```

### 2. Quản lý công việc bằng Issue
- Mỗi task phải tạo một Issue riêng
- Mỗi Issue chỉ gán đúng 1 người chịu trách nhiệm chính
- Gắn label và milestone phù hợp

### 3. Chiến lược phân nhánh
Tên nhánh theo mẫu:

```bash
feature/<MSSV>-issue-<So_Issue>-<Ten_ngan_gon>
```

Ví dụ:
```bash
feature/23110001-issue-5-login-form
```

### 4. Commit message
Dùng chuẩn Conventional Commits:

```bash
git commit -m "feat: thêm chức năng đăng nhập"
git commit -m "fix: sửa lỗi crash khi mất kết nối mạng"
git commit -m "refactor: tối ưu code xử lý API"
git commit -m "docs: cập nhật hướng dẫn cài đặt"
```

### 5. Pull Request
- Tạo PR từ nhánh cá nhân vào nhánh chính
- Mô tả rõ ràng: đã làm gì, ảnh hưởng, kết quả chạy
- Có ít nhất 1 reviewer khác approve
- Không được tự approve cho chính mình

### 6. Bảng đóng góp
Phải duy trì bảng thống kê đóng góp ở đây.

## Bảng đóng góp

| MSSV | Họ và tên | Công việc đã thực hiện | Merge Requests |
|------|-----------|----------------------|----------------|
| 23110001 | Nguyễn Văn A | Xây dựng core network (TCP/UDP) | !1, !3, !7 |
| 23110002 | Trần Thị B | Thiết kế giao diện Client | !2, !4, !6 |

## Cấu trúc đề xuất

```text
.
├── README.md
├── .gitignore
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── task.md
│   │   └── bug_report.md
│   └── pull_request_template.md
├── src/
├── docs/
└── tests/
```

## Bắt đầu làm việc

```bash
git checkout main
git pull origin main
git checkout -b feature/23110001-issue-1-initial-setup
```

## Liên kết quan trọng
- Repository: https://github.com/Dungdebug/LTMMT-Test
- Issues: https://github.com/Dungdebug/LTMMT-Test/issues
- Pull Requests: https://github.com/Dungdebug/LTMMT-Test/pulls

## Lưu ý
- Không commit các thư mục build, cache, file nhị phân lớn
- Không dùng tài khoản hoặc máy của người khác để commit thay
- Tất cả thay đổi phải đi qua Issue -> Branch -> Commit -> PR -> Review
