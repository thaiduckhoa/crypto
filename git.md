## tạo repository (repo)

git init
=> nhánh chính master

### git init -b main

=> tạo repo local vs nhánh chính có tên main

## git remote add origin + <url repo>

=> liên kết repo local vs repo remote

## ko đưa thư mục node_modules lên repo remote

-> node_modules chiếm dung lượng rất lớn
-> node_modules có thể cài lại thông qua câu lệnh: npm i

### file .gitignore quy định những thư mục hay file đẩy lên repo remote

=> .gitignore nằm ở thư mục root

### git status

=> kiểm tra sự thay đổi của các file trong dự án

### git add

=> Thêm file vào trong staging

### git add . => dùng để thêm tất cả các file ở trong thư mực hiện tại vào trong staging

### git add -A => dùng để thêm tất cả các file ở trong dự án vào trong staging

### git add <đường dẫn file> => chỉ thêm file cụ thể vào trong staging
