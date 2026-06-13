# BÁO CÁO THỰC HÀNH GIT & GITHUB

## 1. Thông tin học viên

* Họ và tên: Phan Hà Bảo Quyên
* Lớp: KHDL K6

---

## 2. Mục tiêu thực hành

Hiểu vai trò của Git trong quản lý phiên bản phần mềm.
Tạo và quản lý Git repository.
Thực hiện các thao tác cơ bản: clone, add, commit, push, pull, status, log.
Làm việc với branch để thử nghiệm tính năng mới.
Tạo pull request để đề xuất thay đổi.
Biết cách xử lý conflict ở mức cơ bản.
Biết rollback khi AI sinh code lỗi hoặc thay đổi làm hỏng hệ thống.
Hiểu GitHub Flow trong làm việc nhóm.
Biết dùng Issues, Pull Requests và Project board để quản lý công việc.
Nhận thức được các nguyên tắc bảo mật cơ bản khi đưa code lên GitHub.

---

## 3. Nội dung thực hiện

### 3.1 Hoàn thành các module học tập

Đã hoàn thành các module học tập được giao trên Microsoft Learn. (kèm minh chứng)
Part 1: Git/GitHub cơ bản, repository, branch, commit, pull request, GitHub Flow.

Part 2: cộng tác, quản lý dự án, bảo mật repository, pull request nâng cao, tìm kiếm lịch sử thay đổi, quản trị và sử dụng GitHub Copilot ở mức cơ bản.

---

### 3.2 Tạo GitHub Repository cá nhân

Đã tạo repository cá nhân phục vụ cho bài thực hành Git và GitHub.

Link Repository:
https://github.com/quyeennn/Git-Safety-Foundation


---

### 3.3 Thực hiện Commit

Đã thực hiện tối thiểu 10 commit có ý nghĩa trong quá trình phát triển dự án. (kèm minh chứng)


---

### 3.4 Thực hành Branch

Đã có tối thiểu 3 branch để thực hành: `main`, `conflict`, `conflict-2` , `quyeennn-patch-1`


---

### 3.5 Thực hiện Pull Request

Đã có tối thiểu 2 pull request (kèm minh chứng)


---

### 3.6 Thực hành xử lý Merge Conflict
Tình huống mô tả: từ nhánh main tôi tạo nhánh `confict`, sau đó chỉnh sửa `file readme.md` tại dòng 30, sau đó pull request merge. Tiếp theo từ nhánh `main` cũng chỉnh sửa `file readme.md` tại dòng 30, sau đó tạo pull request với nhánh `confict-2`. Hợp nhất nhánh `conflict` vào `main` thành công. Sau đó hợp nhất `confict-2` thì báo lỗi.
Cách xử lý: tôi đã kích hoạt trình chỉnh sửa web Resolve conflicts, tiến hành xóa bỏ các thẻ đánh dấu xung đột (<<<<<<<, =======, >>>>>>>), giữ lại nội dung đồng nhất và tiến hành commit để hoàn thành việc gộp.


### 3.7 Thực hành Rollback/Revert

Sau khi commit sai nội dung, tôi thực hiện lệnh git log --oneline để lấy commit ID, sau đó thực hiện lệnh git revert e54bb88 (e54bb88 là ID của commit sai). Kết quả dự án được khôi phục về trạng thái mong muốn trong khi vẫn giữ nguyên lịch sử commit.

---

## 4. Kết quả đạt được

Sau khi hoàn thành bài thực hành, tôi đã:

* Hiểu quy trình quản lý mã nguồn bằng Git.
* Thành thạo các thao tác commit và push code.
* Biết tạo và quản lý branch.
* Biết tạo Pull Request trên GitHub.
* Thực hành xử lý merge conflict.
* Thực hành rollback/revert thay đổi.
* Nắm được quy trình làm việc nhóm cơ bản trên GitHub.

---
## 5. Danh sách các lệnh sử dụng trong quá trình học
1. Khởi tạo & clone.
- git init → Tạo repository Git mới
- git clone <url> → Sao chép repository từ GitHub về máy
2. Kiểm tra trạng thái
- git status → Xem trạng thái file (đã sửa, chưa commit)
- git log → Xem lịch sử commit
- git log --oneline → Xem lịch sử commit ngắn gọn
3. Làm việc với file
- git add <file> → Thêm file vào staging area
- git add . → Thêm tất cả file đã thay đổi
- git restore <file> → Khôi phục file về trạng thái trước sửa
4. Commit
- git commit -m "message" → Lưu thay đổi vào lịch sử
- git commit --amend → Sửa commit gần nhất
5. Branch (nhánh)
- git branch → Xem danh sách branch
- git branch <name> → Tạo branch mới
- git checkout <name> → Chuyển branch
- git checkout -b <name> → Tạo và chuyển branch mới
- git merge <branch> → Gộp branch vào branch hiện tại
- git branch -d <name> → Xóa branch
6. Remote (GitHub)
- git remote -v → Xem remote repo
- git remote add origin <url> → Kết nối GitHub repo
- git push → Đẩy code lên GitHub
- git push origin <branch> → Đẩy branch cụ thể
- git pull → Lấy code mới từ GitHub về
7. Reset & Revert
- git revert <commit> → Hoàn tác commit (an toàn, tạo commit mới)
- git reset --soft <commit> → Quay lại commit, giữ thay đổi
- git reset --hard <commit> → Quay lại commit, xóa thay đổi
8. So sánh
- git diff → So sánh thay đổi chưa stage
- git diff --staged → So sánh file đã stage

## 6. Tôi sẽ dùng Git như thế nào khi Vibe Code với AI?
* Sử dụng Git như một cơ chế kiểm soát phiên bản để quản lý toàn bộ thay đổi khi làm việc với AI.
* Tạo branch riêng cho từng tính năng hoặc thử nghiệm do AI sinh ra nhằm cô lập thay đổi và tránh ảnh hưởng đến code chính.
* Thực hiện commit thường xuyên sau mỗi thay đổi quan trọng để dễ theo dõi lịch sử và khôi phục khi cần.
* Tạo commit hoặc branch backup trước khi thực hiện các thay đổi lớn do AI đề xuất như refactor hoặc nâng cấp hệ thống.
* Sử dụng `git diff` để kiểm tra chi tiết các thay đổi mà AI tạo ra trước khi chấp nhận tích hợp.
* Sử dụng `git revert` hoặc `git reset` để quay lại trạng thái ổn định khi AI tạo ra lỗi hoặc thay đổi không mong muốn.
* Chỉ thực hiện merge vào nhánh chính thông qua pull request sau khi đã kiểm tra kỹ lưỡng toàn bộ thay đổi.





