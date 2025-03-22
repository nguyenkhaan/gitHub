# GIẢI THÍCH HIỆN TƯỢNG CONFLICT 
## 1. Hiểu rõ về git pull và git push 
Git push: Dùng để đẩy code lên Repissratory 

**Chú ý:**: Nó sẽ kiểm tra remote của bạn có đoạn code nào 
mới không. Nếu không có thì mới thực hiện đẩy code, còn nếu có sẽ bắt buộc bạn phải thực hiện git pull 

Git pull: Là sự kết hợp giữa git fetch và git merge. Dùng để hợp nhất code từ remote về local. 

**Chú ý**: Nó sẽ kiểm tra local của bạn, xem có đoạn code nào mới được thêm vào không. 
Nếu không thì mới có thể pull về, nếu không sẽ yêu cầu bạn commit rồi mới có thể thêm. 

## 2. Conflict xảy ra khi nào 
Conflict xảy ra khi bạn thay đổi code ở cả remote và local, dẫn đến Github không biết lựa chọn nhánh nào khi thực 
hiện git pull (có sự merge nhánh) 

