# GIẢI THÍCH HIỆN TƯỢNG CONFLICT 
## 1. Hiểu rõ về git pull và git push 
Git push: Dùng để đẩy code lên Repissratory 

**Chú ý:**: Nó sẽ kiểm tra remote của bạn có đoạn code nào 
mới không. Nếu không có thì mới thực hiện đẩy code, còn nếu có sẽ bắt buộc bạn phải thực hiện git pull 

Git pull: Là sự kết hợp giữa git fetch và git merge. Dùng để hợp nhất code từ remote về local. 

**Chú ý**: Nó sẽ kiểm tra local của bạn, xem có đoạn code nào mới được thêm vào không. 
Nếu không thì mới có thể pull về, nếu không sẽ yêu cầu bạn commit rồi mới có thể thêm. 

## 2. Conflict xảy ra khi nào 
Trong trường hợp hai nhánh đã đủ điện kiện merge. Conflict sẽ có thể xảy ra khi bạn thay đổi code ở cả remote và local

**Ví dụ 1:** \
1. Bạn thực hiện chỉnh sửa ở cả `local` và `remote` 
2. Bạn `git pull` dữ liệu về máy. Nhưng máy sẽ yêu cầu bạn phải commit trước để không bị mất code (Cái số 2)
3. Bạn `commit` code 
4. Bạn thực hiện `git pull`. Lúc này hai nhánh đã đủ điện kiện gộp. Github sẽ tiến hành gộp và phát hiện conflict. 
Vì bạn đã thực hiện chỉnh sửa ở `local` và `remote` nên lúc này conflict sẽ xảy ra. Bạn phải tiến hành xử lí conflict thì mới 
thực hiện các tác vụ bình thường được. 

**Ví dụ 2:**
1. Bạn thực hiện chỉnh 