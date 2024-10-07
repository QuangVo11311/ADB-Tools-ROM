# Dưới đây là hướng dẫn cài ROM cho Xiaomi/Redmi/Poco được sắp xếp gọn gàng và dễ theo dõi:

---

## 1. Chuẩn bị các file cần tải:
- **Minimal ADB and Fastboot** (Đã có sẵn)
- **MiSetup3.2.1.3111_2717** (Đã có sẵn)
- **MiFlash20220507** (Đã có sẵn)
- **Xiaomi Community** [Tải về tại đây](https://drive.google.com/file/d/1Db7ujnbLjGoGMpBtK-1C97aLgjdTt5Zr/view?usp=sharing)
- **Miflash Unlock** [Tải về tại đây](https://drive.google.com/file/d/1iau6Wcr16BPFj5EJ-JyfI1UzEu0wmawl/view?usp=sharing)
- **File TWRP** (.img) [Tải về tại đây](https://twrp.me/Devices/)
- **File ROM** 
  - [Xiaomi EU ROM](https://sourceforge.net/projects/xiaomi-eu-multilang-miui-roms/files/xiaomi.eu/)
  - [Global/CN ROM](https://mifirm.net/)

### Lưu ý:
- **Khi bị Brick/Soft Brick** hoặc cần chạy lại phần mềm: flash lại ROM gốc.
  - Máy xách tay: Flash ROM CN
  - Máy quốc tế: Flash ROM Global
- ROM Global/CN: Giải nén để flash bằng MiFlash.
- ROM EU: Không cần giải nén khi flash bằng TWRP.

---

## 2. Cài Driver:
1. Cài đặt **MiSetup3.2.1.3111_2717**.
2. Chạy file **XiaoMiFlash.exe** trong thư mục **MiFlash20220507**.
3. Trong MiFlash, chọn **Driver** → **Install**.

---

## 3. Unlock Bootloader:
### 3.1. Đối với thiết bị xuất xưởng chạy HyperOS
1. Chuẩn bị tài khoản Xiaomi.
2. Cài và mở ứng dụng **Xiaomi Community**. Chọn vùng Global.
3. Đăng nhập vào Xiaomi Community, vào **ME** → **Unlock Bootloader** → Yêu cầu mở khóa.
4. Sau khi app thông báo thành công, vào Cài đặt → Tùy chọn nhà phát triển, bật **OEM Unlock**.
5. Vào **Mi Unlock Status** → Add Xiaomi account.
6. Dùng **Miflash Unlock** để kiểm tra thời gian unlock và chờ (khoảng 3 ngày).

### 3.2. Đối với thiết bị xuất xưởng chạy MIUI
1. Chuẩn bị tài khoản Xiaomi.
2. Vào Cài đặt → Tùy chọn nhà phát triển → Bật **OEM Unlock**.
3. Vào **Mi Unlock Status** → Add Xiaomi account.
4. Kiểm tra thời gian unlock trong **Miflash Unlock**. Chờ (thường từ 7 ngày đến 3 tháng).

---

## 4. Cài ROM:
### 4.1. Flash ROM bằng MiFlash20220507:
1. Chạy **XiaoMiFlash.exe**.
2. Đưa máy vào chế độ **Fastboot** (Giữ nút giảm âm lượng + nút nguồn).
3. Kết nối thiết bị với máy tính, nhấn **Refresh** để MiFlash nhận diện thiết bị.
4. Chọn **Select** và dẫn đến thư mục chứa ROM đã tải.
5. Chọn **Clean All**, sau đó nhấn **Flash**. Chờ quá trình hoàn tất và KHÔNG ngắt kết nối trong lúc flash.

### 4.2. Flash ROM bằng TWRP:
1. (Lần đầu vào TWRP) Chọn **Wipe** → **Format Data** → Nhập "yes" → Dấu V.
2. Sau khi format, chọn **Reboot** → **Recovery**.
3. Copy ROM vào máy mà không giải nén.
4. Trong TWRP, chọn **Install** → Chọn ROM vừa copy.
5. Sau khi flash xong, chọn **Wipe Cache/Dalvik** rồi **Reboot System**.

### 4.3. Flash ROM dùng Hybrid (cài ROM EU hoặc cập nhật ROM EU):
1. Đưa máy vào **Fastboot** (Giữ nút giảm âm lượng + nút nguồn).
2. Kết nối máy với PC.
3. Giải nén ROM EU.
   - Lần đầu flash: Chọn **windows_fastboot_first_install_with_data_format**.
   - Cập nhật ROM: Chọn **windows_fastboot_update_rom**.
4. Chờ hoàn thành, máy sẽ tự động reboot vào hệ thống.

---

Chúc bạn thành công!
