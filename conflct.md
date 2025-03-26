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
1. Bạn thực hiện chỉnh sửa ở cả `local` và `remote` 
2. Bạn `git push` dữ liệu lên remote. Nhưng máy phát hiện remote cũng đã thay đổi ppp
3. Bạn `pull` code 
4. Bạn thực hiện `git pull`. Github sẽ tiến hành gộp và phát hiện conflict. Vì bạn đã thực hiện chỉnh sửa ở `local` và `remote` nên lúc này conflict sẽ xảy ra. Bạn phải tiến hành xử lí conflict thì mới 
thực hiện các tác vụ bình thường được. 

- `folk`: Lấy của người ta thành của mình 
- `git clone`: Copy nguyên repo về máy của bạn 
- `git checkout -b <branch name>`: Tao nhanh va chuyen toi lun 
- `git branch`: Xem cac nhanh hien co 
- `git checkout <branch_name>`: Di chuyen qua lai giua cac nhanh 
- `git status`: Xem co bao nhieu file thay doi 
- `git remote -v`: Xem cac duong dan hien co 
- `git push -f`: Bat buoc day code len, khong quan tam la code nhu the nao 
- `git commit --amend` Thuc hien voi commit truoc do 
- `git merge <ten_nhanh_gop>`: Thuc hien gop nhanh vao master 
- `git branch -D <ten_branch>`: Xoa branch 
- `git reabse <branch_name>`: Lấy các code của branch_name và đưa vào nhánh hiện tại 
- `git checkout -b branch_name ID`: Khôi phục lại branch có ID đã bị xóa 
- `git reflog`: Hiện các thao tác git đã thực hiện 
Khi chuyen branch thi tu dong cac file cung se chuyen thanh cac file branch tuong ung luc moi duoc tao. Kieu 
nhu branch nao thi file đó vậy á 