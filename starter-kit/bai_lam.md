# BÀI LÀM – HACKATHON 01

  

-  **Mã đề:** 21

-  **Họ tên:** Phạm Vũ Tuấn Kiệt

-  **Lớp:** CNTT2

-  **Link repository:**

-  **Hệ điều hành (Windows/macOS):** Window

  

## 4.2. Thao tác máy tính cơ bản bằng CLI

  

### Các lệnh đã chạy

  

```shell
PS C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL> Get-ChildItem -Recurse -Force


    Directory: C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/28/2026   1:57 PM                backup
d-----        10/28/2026   1:57 PM                data
d-----        10/28/2026   1:57 PM                docs
d-----        10/28/2026   1:57 PM                logs
d-----        10/28/2026   1:57 PM                media
-a----        10/27/2026   1:32 AM             74 .env
-a----        10/27/2026   1:32 AM           6103 don_qua_thang 12.xlsx
-a----        10/27/2026   1:32 AM           1040 gift.log
-a----        10/27/2026   1:32 AM           6478 logo_qua_luu_niem.PNG
-a----        10/27/2026   1:32 AM             53 mau_goi_qua.txt
-a----        10/27/2026   1:32 AM             22 temp_293.tmp


PS C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL> mv mau_goi_qua.txt docs/
PS C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL> mv logo_qua_luu_niem.PNG media/
PS C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL> cp media/^C
PS C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL> cp media/logo_qua_luu_niem.PNG backup/
PS C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL> rm temp_293.tmp
```
### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

  

```text
PS C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL> Get-ChildItem -Recurse -Force


    Directory: C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/28/2026   2:04 PM                backup
d-----        10/28/2026   2:01 PM                data
d-----        10/28/2026   2:01 PM                docs
d-----        10/28/2026   2:01 PM                logs
d-----        10/28/2026   2:02 PM                media
-a----        10/27/2026   1:32 AM             74 .env


    Directory: C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL\backup


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/27/2026   1:32 AM           6478 logo_qua_luu_niem.PNG


    Directory: C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL\data


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/27/2026   1:32 AM           6103 don_qua_thang 12.xlsx


    Directory: C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL\docs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/27/2026   1:32 AM             53 mau_goi_qua.txt


    Directory: C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL\logs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/27/2026   1:32 AM           1040 gift.log


    Directory: C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL\media


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/27/2026   1:32 AM           6478 logo_qua_luu_niem.PNG

  ```

## 4.3. Lọc log thủ công

  

### Lệnh đã chạy

  

```shell

PS C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL> Get-Content logs/gift.log|Select-String "ERROR"

2026-12-28 07:38:36 [ERROR] Khong tim thay trang /qua-tet (404)
2026-12-28 07:44:36 [ERROR] Het thoi gian cho (timeout)
2026-12-28 07:56:36 [ERROR] Khong tim thay trang /qua-tet (404)
2026-12-28 08:05:36 [ERROR] Thanh toan bi tu choi
2026-12-28 08:08:36 [ERROR] Thanh toan bi tu choi
2026-12-28 08:17:36 [ERROR] Khong tim thay trang /qua-tet (404)
2026-12-28 08:23:36 [ERROR] Het thoi gian cho (timeout)

  

```

  

### 2 dòng lỗi đầu tiên trong daily_report.txt

  

```text

2026-12-28 07:38:36 [ERROR] Khong tim thay trang /qua-tet (404)
2026-12-28 07:44:36 [ERROR] Het thoi gian cho (timeout)

  

```

  

## 4.4. Thao tác với tài liệu Markdown (README.md)

  

> README.md được chấm trực tiếp trên file `README.md` ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

  

- [ ] Heading 1: tên dự án

- [ ] Mô tả ngắn có cả **in đậm** và *in nghiêng*

- [ ] Bảng `Thư mục | Nội dung`, ít nhất 3 dòng dữ liệu

- [ ] Code block chứa lệnh PowerShell/Terminal liệt kê nội dung dự án

- [ ] Task list ít nhất 2 công việc, có ít nhất 1 mục đã hoàn thành

- [ ] Blockquote nhắc không upload `.env`

  

## 4.5. Chạy script auto_report (.ps1 hoặc .sh)

  

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

  

```shell

# Ghi lệnh vào đây (xoá dòng này)

  

```

  

### Kết quả hiển thị

  

```text

(Dán kết quả vào đây – xoá dòng này)

  

```

  

## 4.6. Đếm số dòng lỗi

  

### Lệnh

  

```shell

PS C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL> Get-Content logs/gift.log|Select-String "ERROR"

2026-12-28 07:38:36 [ERROR] Khong tim thay trang /qua-tet (404)
2026-12-28 07:44:36 [ERROR] Het thoi gian cho (timeout)
2026-12-28 07:56:36 [ERROR] Khong tim thay trang /qua-tet (404)
2026-12-28 08:05:36 [ERROR] Thanh toan bi tu choi
2026-12-28 08:08:36 [ERROR] Thanh toan bi tu choi
2026-12-28 08:17:36 [ERROR] Khong tim thay trang /qua-tet (404)
2026-12-28 08:23:36 [ERROR] Het thoi gian cho (timeout)


  

```

  

### Kết quả đếm (Windows: giá trị Count; macOS: con số in ra)

  

```text

PS C:\Users\X\Desktop\starter-kit\Qua Luu Niem Website FINAL> Get-Content logs/gift.log|Select-String "ERROR"|Measure-Object


Count    : 7
Average  :
Sum      :
Maximum  :
Minimum  :
Property :
  

```

  

## 4.7. Báo cáo tổng hợp

  

### Các lệnh đã chạy

  

```shell

# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng (xoá dòng này)

  

```

  

### Nội dung file logs/tong_hop.txt

  

```text

(Dán kết quả vào đây – xoá dòng này)

  

```

  

## 4.8. Excel

  

> Phần Excel được chấm trực tiếp trên file `data/don_qua_thang_12.xlsx`, không cần ghi vào đây.