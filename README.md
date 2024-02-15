# Những gì cần biết để cài ROM cho Xiaomi/Redmi/Poco

## 1. Chuẩn bị các file cần tải
* Minimal ADB and Fastboot (đã có sẵn)
* MiSetup3.2.1.3111_2717 (đã có sẵn)
* MiFlash20220507 (đã có sẵn)
* Miflash unlock
<br> https://drive.google.com/file/d/1iau6Wcr16BPFj5EJ-JyfI1UzEu0wmawl/view?usp=sharing
* File T.W.R.P có đuôi là <b>.img</b>
<br> https://twrp.me/Devices/
* File ROM
<br> https://sourceforge.net/projects/xiaomi-eu-multilang-miui-roms/files/xiaomi.eu/
<br> https://mifirm.net/

## Lưu ý:
* Khi bị Brick/Soft Brick/cần chạy lại phần mềm thì flash lại ROM gốc của máy
  * Đối với máy xách tay: Flash lại ROM CN
  * Đối với máy quốc tế: Flash lại ROM Global
* ROM Global, ROM CN tải về phải giải nén để flash bằng phần mềm MiFlash
* ROM EU tải về nếu dùng T.W.R.P để flash thì không cần phải giải nén

## 2. Cài driver
<br> Bước 1: Cài đặt <b>MiSetup3.2.1.3111_2717</b>
<br> Bước 2: Chạy file <b>XiaoMiFlash.exe</b> trong thư mục MiFlash20220507
<br> Bước 3: Nhìn trên thanh công cụ chọn <b>Driver</b> => <b>Install</b>
<br>
<br> Như vậy là đã cài đặt xong driver.

## 3. Unlock bootloader
<br> Vì Xiaomi đổi chính sách mới nên phần này sẽ update sau

## 4. Cài ROM
### 4.1. Flash ROM bằng MiFlash20220507
<br> Bước 1: Chạy file <b>XiaoMiFlash.exe</b>
<br> Bước 2: Đưa thiết bị vào chế độ fastboot (Giữ phím giảm âm lượng + phím nguồn cho tới khi nào xuất hiện logo <b>fastboot</b>)
<br> Bước 3: Kết nối thiết bị với máy tính
<br> Bước 4: Ấn <b>Refresh</b> để phần mềm nhận thiết bị
<br> Bước 5: Chọn <b>Select</b> sau đó dẫn đến thư mục chưa ROM đã tải về
<br> Bước 6: Tích chọn <b>clean all</b> ở bên dưới trước khi nhấn <b>flash</b> nếu không sẽ bị Brick
<br> Chờ 5-10' cho tới khi thấy điện thoại boot vào hệ thống và <b>KHÔNG ĐƯỢC RÚT DÂY CÁP KẾT NỐI HOẶC ĐÓNG PHẦN MỀM</b> trong lúc đang flash nếu không muốn Brick máy

### 4.2. Flash ROM bằng T.W.R.P
<br> Bước 1: (Áp dụng với lần đầu tiên vào T.W.R.P) Chọn <b>Wipe</b> => <b>Format Data</b> => Nhập "yes" và ấn vào dấu V
<br> Đợi quá trình format diễn ra xong => nhấn vào biểu tượng ngôi nhà để trở về trang chủ => Chọn Reboot => Recovery
<br> Bước 2: Copy ROM vào máy (không giải nén file)
<br> Bước 3: Ở màn hình chính chọn <b>Install</b> => Chọn ROM vừa sao chép
<br> Bước 4: Sau khi ROM chạy xong => Chọn <b>Wipe Cache/Dalvik</b> => Chờ quá trình này chạy xong
<br> Bước 5: Chọn <b>Reboot System</b>

### 4.3. Flash ROM dùng Hybrid để cài ROM EU hoặc cập nhật ROM EU(Áp dụng cho thiết bị sản xuất từ cuối năm 2022 trở đi)
<br> Bước 1: Đưa thiết bị vào chế độ fastboot (Giữ phím giảm âm lượng + phím nguồn cho tới khi nào xuất hiện logo <b>fastboot</b>)
<br> Bước 2: Kết nối thiết bị với máy tính
<br> Bước 3: Giải nén ROM EU
<br> Bước 4:

* Trường hợp Flash lần đầu: Chọn <b>windows_fastboot_first_install_with_data_format</b>
* Trường hợp Flash để cập nhật ROM: Chọn <b>windows_fastboot_update_rom</b>

<br> Chờ Flash xong phần mềm tự tắt và máy tự động Reboot System