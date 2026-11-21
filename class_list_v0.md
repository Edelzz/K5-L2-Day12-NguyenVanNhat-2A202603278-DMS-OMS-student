# Danh sách lớp v0 — Nguyễn Văn Nhất · G06

## DMS

| Lớp / thuộc tính | Giá trị | Để làm gì | Nhìn thấy trên IR? |
|---|---|---|---|
| face | Hộp khuôn mặt | Xác định vùng cần phân tích mắt và hướng đầu | Có, nếu mặt đủ rõ |
| eye_left / eye_right | open / closed / unknown | Theo dõi thời gian nhắm mắt qua nhiều khung để hỗ trợ phát hiện buồn ngủ | Có, tùy độ nét và phản xạ kính |
| glasses | none / clear / sun / unknown | Đánh giá khi nào quan sát mắt kém tin cậy | Gọng thường thấy được, loại tròng có thể khó phân biệt |
| gaze_zone | road / mirror_l / mirror_r / mirror_c / cluster / center / lap / other | Ước lượng tài xế nhìn vùng nào và theo dõi thời gian rời mắt khỏi đường | Có khi thấy mắt hoặc hướng đầu đủ rõ |
| face13 | 13 tọa độ và cờ che khuất | Ước lượng hướng đầu và hình dạng khe mắt | Tùy vùng bị che và độ nét |
| hand.on_wheel | yes / no / unknown | Xác định tay nào đang chạm vô lăng | Có khi thấy điểm tiếp xúc |
| phone.state | held / mounted / lap | Phân biệt điện thoại đang cầm với điện thoại trên giá hoặc đùi | Có khi nhận ra hình dạng máy |

## OMS

| Lớp / thuộc tính | Giá trị | Để làm gì | Nhìn thấy trên IR? |
|---|---|---|---|
| person | Hộp người | Xác định ghế có người lớn | Có nếu còn thấy hình dáng |
| seat | driver / front_passenger / rear_left / rear_middle / rear_right | Gắn người hoặc vật với đúng vị trí trong xe | Có dựa vào vị trí trong ảnh |
| seatbelt | worn_correct / worn_incorrect / not_worn / unknown | Hỗ trợ nhắc thắt dây theo vị trí ngồi | Tùy tương phản và che khuất |
| child_seat | Hộp ghế trẻ em | Nhận biết vị trí lắp ghế trẻ em | Thường thấy qua hình dạng |
| infant_seat.facing | rear / front | Xác định hướng lắp nôi để hỗ trợ kiểm tra bố trí ghế | Có khi nhìn rõ cấu trúc ghế |
| object.type | bag / box / cup / other | Phân biệt đồ để lại trên ghế với người ngồi | Có khi thấy đường viền đủ rõ |

## Hai câu hỏi leo thang

1. Ở `S03_ir`, ghế giữa trông như có trẻ đang ngồi. Guideline có cho phép gán box ghế trong trường hợp này không? Trong lúc chờ coach, đánh dấu ca cần xác minh và tránh xác nhận `occupied = no`.
2. Ở `D03`, phản xạ che một phần khe mắt nhưng vẫn thấy đường viền kính. Cần thấy tối thiểu phần nào của khe mắt để gán `open`? Trong lúc chờ coach, giữ `unknown` cho mắt chưa xác định được trạng thái và đánh cờ theo khả năng định vị từng điểm.
