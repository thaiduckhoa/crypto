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

### working directory (file màu đỏ)

### staging (file màu xanh)

=> lúc này file sẵn sàng để đưa lên repo remote

### config git (chỉ chạy duy nhất 1 lần)

### git config --global user.name ""

### git config --global user.email ""

### git commit -m "message"

=> dùng để gắn message vào trong file đang ở staging đc phép đưa lên repo remote

=> mỗi commit có một mã sha (id)

### git log

=> kiểm tra lịch sử commit

### git push -u origin <tên nhánh>

=> đưa code lên repo remote
=> từ lần push code thứ 2: git push

### đưa file từ cái staging về lại working

git reset
git restore -S (đưa tất cả các file đang ở staging về working)
git restore -S <url file> (chỉ đưa duy nhất file về working)

### git checkout <url file>

=> 1. đưa 1 file đang đc chỉnh sửa về trạng thái trc đó

### branch

// dev => Kiểm thử QA và Dev (dev)

// staging => QA Kiểm thử 1 lần (staging)

// production => end user (main/release)

git branch <tên nhánh>
=> tạo ra 1 nhánh mới
=> nhánh mới sẽ chứa toàn bộ code của nhánh đang đứng

git branch -a or git branch
=> Liệt kê tất cả các branch đang có trong repo

git switch <tên nhánh>
=> Chuyển qua nhánh <tên nhánh>

### git pull

=> pull code ở repo remote về local
git pull --no-ff

### git clone <url repo>

=> Dùng để clone source code của 1 repo bất kỳ
