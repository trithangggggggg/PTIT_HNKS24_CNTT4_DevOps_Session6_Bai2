# Báo cáo Thực hành Bài 2: Cấu hình phân quyền Nhóm và sudoers bằng visudo

## 1. Tạo nhóm và tài khoản người dùng mới

Tạo nhóm `devops-admin` và người dùng `deployer`, sau đó thêm `deployer` vào nhóm `devops-admin`:

```bash
sudo groupadd devops-admin
sudo adduser --gecos "" deployer
sudo usermod -aG devops-admin deployer