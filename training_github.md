# 😍CƠ BẢN VỀ GIT😍
## ❓0. Cơ chế của Git 
![Hinh_anh](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR4IkgIwsGWN52UBrCWimoeCqeQ4fo2F91_mg&s)

```md
Công việc được chia nhỏ thành từng branch. Các branch sẽ được nhân viên làm và chỉnh sửa trước, sau cùng mới được gộp vào nhánh master để tạo thành sản phẩm hoàn thiện. 
```
![Hinh_anh2](https://i.ytimg.com/vi/7jG1Bo84SGc/hq720.jpg?sqp=-oaymwEhCK4FEIIDSFryq4qpAxMIARUAAAAAGAElAADIQj0AgKJD&rs=AOn4CLB1JwpTtPzlr8_b08fRxFmFsasfBw)
```md
Local: Nôm na là cái máy tính của chúng ta, là nơi soạn thảo code offline 

Remote: Là kho lưu trữ code chung (online) 

Ta có thể sử dụng các lệnh của Github để đẩy code từ local (máy) lên online (remote), cũng có thể lấy code từ remote về local . Ngoài ra, trên remote cũng xảy ra hiện tượng gộp nhánh như ở hình 1. 
```

>Nói chung, chỉ cần nhớ tên tiếng anh vài cái sau cho dễ 

💻 **branch**: Nhánh 

💻 **local**: Máy của mình 

💻 **remote**: Cái kho online 

💻 **push**: Thao tác đẩy code lên online  

💻 **clone / pull**: Thao tác kéo code về máy 


## 💟1. Làm đầu tiên trong ngày 
```md
**Thao tác folk**: Mỗi company có 1 cái github riêng (chủ). Mình sẽ tiến hành đưa cái github riêng của công ty đó về github của mình và chỉnh sửa ngay trên github của mình. Rồi mới đua code lên lại github của công ty. 
```
`git clone <url>`: Lấy code từ github về máy *(chỉ làm duy nhất một lần trong ngày)* 
## 💔2. Chẻ nhánh 
1. Chia nhỏ công việc 
2. Tránh rủi ro  

📝 `git branch:`: Hiển thị tất cả tên nhánh hiện có

📝 `git checkout <ten_nhanh>`: Chuyển sang nhánh khác 

📝 `git branch <ten_nhanh>`: Tạo một nhánh mới 

🔖**Lệnh gộp:** Sử dụng `git checkout -b <ten_nhanh>` để tạo 1 nhánh mới và chuyển sang nhánh đó luôn 

>Tự tìm hiểu muốn xóa 1 nhánh thì làm như thế nào xem?
## 3. 😙Đưa code lên github 
- 📝 `git init`: Khởi tạo kho lưu trữ trên local 
- 📝 `git add .`: Thêm dữ liệu vào kho lưu trữ 
- 📝 `git commit -m "Complted_Task26"`: Commit để tránh mất code 
- 📝 `git push <url> <ten_nhanh>`: Đưa code lên nhánh 
## 4. 😠Cập nhật code mới nhất về máy (Làm sai dễ bị chửi) 
- 📝 `git pull <url> <ten_nhanh>`: Lấy code mới nhất từ **nhánh** về máy 
## 5. Một số lệnh kiểm tra 
- 📝 `git remote -v`: Xem đường link hiện có. 
- 📝 `git remote add <name> <url>`: Thêm một đường link 
- 📝 `git remote remove <name>`: Xóa đường link 
- 📝 `git status`: Xem co bao nhieu file thay doi 
- 📝 `git log --oneline`: Xem lịch sử gõ lệnh git. Để thoát thì gõ :q 

>Có 1 lệnh ngắn gọn hơn **git log --oneline** nữa, thử tìm cái lệnh này xem? 
