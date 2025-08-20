# Cách 1: Gỡ bằng dịch vụ Windows
- Nhấn Win + R, gõ services.msc → Enter.
- Tìm SolidWorks Flexnet Server hoặc SolidWorks Licensing Service.
- Chuột phải → Stop (dừng dịch vụ).
- Sau đó thử xóa lại folder.

# Cách 2: Xóa bằng Command Prompt (Administrator)
- Nhấn Win + S, gõ cmd → chuột phải → Run as administrator.
- Gõ lệnh để dừng service:
```bash
net stop "SolidWorks Flexnet Server"
```
hoặc
```bash
net stop "SolidWorks Licensing Service
```
- Xong gõ tiếp để xóa service khỏi Windows:
```bash
sc delete "SolidWorks Flexnet Server"
```
Cuối cùng, xóa folder:
```bash
rmdir /s /q "C:\SolidWorks_Flexnet_Server"
```

# Cách 3: Safe Mode
- Nếu vẫn không xóa được, khởi động lại Windows ở chế độ Safe Mode → rồi xóa thủ công folder đó.
