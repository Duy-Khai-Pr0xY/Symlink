# Symlink
#### vào docker (docker ps) sau đó chọn môi trường (docker exec -ti docker_ID bash)
#### Symlink kh phải là 1 file mà nó là 1 loại liên kết đặc biệt trỏ đến 1 file trong thư mục gốc (Giống như shotcut) nó giống như ảnh ảo của file gốc 
#### Để tạo symlink trên linux ta sử dụng câu lệnh "ln -s duong_dan_file_goc ten-cua_link", ">>" đẩy dữ liệu vào cuối cùng của file
#### Symlink trên linux không thể di chuyển được trên internet được do không phải một file thực sự (trình duyệt đã đọc file gốc rồi gửi đi chứ không phải gửi symlink đi)
# Sử dụng tính năng nén 
#### Trên linux zip hỗ trợ nén và giải nén symlink (zip -y ten_file_zip file_muon_zip)
# Chặn chức năng up file php
#### up ra ngoài file documentRoot (tạo 1 symlink hướng ra ngoài folder bị chặn)
#### sau đó write vào symlink
#### thử up một symlink lên folder
# Symlink kh chỉ dẫn thẳng đến ứng dụng(read,write,excute) mà còn dẫn thẳng đến folder (list) list được cái file trên folder
#### RCE 1: tạo 1 thư mục link_to_root sau đó zip và đẩy lên server
#### RCE 2: ghi file vào thư mục /var/www/html ==> upload file zip chứa shell.php trong thư mục link_to_..... (trùng tên) 
