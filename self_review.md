# Tự đánh giá — Nguyễn Văn Nhất · G06

## Rà soát bốn ảnh

| Ảnh | Đối tượng | Loại lỗi | Ghi chú | Đã sửa? |
|---|---|---|---|---|
| S03_ir | Ghế giữa | wrong_class | Ghế được gán occupied = no dù bên trong có hình giống trẻ đang ngồi. Cần hỏi coach. | Chờ xác nhận quy tắc |
| S06_rgb | Ghế bên trái ảnh | missing | Vùng rear_right tối nên cần tăng độ sáng hiển thị để kiểm lại. | Cần rà trên CVAT |
| D02 | Khóe ngoài hai mắt | ok | Mắt trái có y = 719, mắt phải có y = 519, đúng thứ tự trên ảnh xoay. | Đã giải thích trong check_final.txt |
| D03 | Trạng thái mắt và điểm mí | guess | Cả hai mắt đang là open dù phản xạ trên kính làm khó xác nhận khe mắt. | Cần rà trên CVAT |

## Lỗi lặp lại và cách tránh

Các ảnh S03, S06 và S07 có ca ghế được đánh occupied = no dù có hình giống trẻ đang ngồi. Khi rà, cần kiểm bên trong ghế trước khi xác nhận ghế trống và ghi tên ảnh để hỏi coach.

## Review chéo

Bài này thực hiện tự rà soát bốn ảnh. Mục review chéo E3 được bỏ qua theo lựa chọn của người làm.
