# ungdungkiso
Dưới đây là **báo cáo kết quả** ngắn gọn cho đoạn mã Flask trên, trình bày rõ chức năng chính và kết quả đạt được:

---

#

### **1. Mục tiêu**

Phát triển một ứng dụng web sử dụng Flask để thực hiện ký số và xác thực chữ ký số cho tệp tin bằng thuật toán RSA kết hợp các hàm băm như SHA256, SHA384, SHA512.

---

### **2. Chức năng chính**

* **Tạo cặp khóa RSA** với kích thước tùy chọn: 512, 1024, 2048, 4096 bit.
* **Tải lên tệp và ký số**: Tệp được ký bằng khóa riêng tư và lưu metadata chữ ký.
* **Xác thực chữ ký số**: Kiểm tra tính hợp lệ của tệp đã ký bằng khóa công khai.
* **Tải xuống khóa công khai/riêng tư** và các tệp đã ký.
* **Hiển thị danh sách các tệp đã ký** cùng thông tin liên quan.

---

### **3. Công nghệ sử dụng**

* **Ngôn ngữ**: Python
* **Framework**: Flask
* **Thư viện mã hóa**: `cryptography`
* **Giao diện**: Flask templates (HTML)

---

### **4. Kết quả đạt được**

* Hệ thống có khả năng tạo cặp khóa RSA và lưu trữ an toàn.
* Tệp tin sau khi ký số được đính kèm metadata, lưu trữ vào thư mục riêng.
* Xác thực tệp đã ký cho kết quả chính xác: hợp lệ hoặc không hợp lệ.
* Hỗ trợ tải về khóa và các tệp đã ký thông qua giao diện người dùng.
* Giao tiếp client-server hiệu quả qua JSON và hỗ trợ phản hồi thông báo rõ ràng.

---

### **5. Hạn chế và hướng phát triển**

* Chưa có xác thực người dùng (user login).
* Chưa hỗ trợ lưu trữ metadata lâu dài bằng CSDL.
* Có thể mở rộng thêm tính năng ký nhiều tệp cùng lúc, giao diện trực quan hơn.

---![image](https://github.com/user-attachments/assets/e7078a36-ffe0-4ffe-bc25-5484d431ba50)



