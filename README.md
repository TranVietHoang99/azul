# 🟦 Azul

Game **Azul** (Michael Kiesling, Plan B Games) cho 2 người, chơi ngay trên trình duyệt: lấy gạch men từ xưởng, xếp vào hàng chờ rồi lát lên tường.

## Chế độ chơi
- **Chơi với máy**: nhập tên, bấm *Chơi với máy*.
- **Online 1 đấu 1**: bấm *Tạo phòng*, gửi mã hoặc link cho bạn bè; bạn bè nhập mã và bấm *Vào phòng*.
  Người tạo phòng phải **giữ tab mở**, vì máy chủ phòng giữ trạng thái ván chơi.

## Luật tóm tắt (bản 2 người)
- 100 viên, 5 màu. Mỗi vòng có 5 xưởng × 4 viên, giữa bàn có thẻ đi trước.
- Tới lượt: lấy **tất cả** viên cùng một màu ở một xưởng (phần còn lại đẩy ra giữa bàn) hoặc ở giữa bàn
  (người đầu tiên lấy từ giữa bàn nhận thẻ đi trước: −1 điểm, được đi trước vòng sau).
- Xếp vào một hàng chờ (hàng 1–5 chứa 1–5 viên), mỗi hàng một màu, không trùng màu đã có trên tường ở hàng đó. Viên thừa rơi xuống sàn.
- Hết gạch thì lát tường: mỗi hàng chờ đầy đưa 1 viên lên tường. Viên đứng riêng +1; nối nhau thì cộng chuỗi ngang và dọc.
  Sàn trừ −1, −1, −2, −2, −2, −3, −3.
- Trận kết thúc sau vòng có người lát kín một hàng ngang. Thưởng: hàng ngang +2, cột dọc +7, đủ 5 viên một màu +10.
  Bằng điểm thì ai nhiều hàng ngang hơn thắng.

## Cách bấm
- Bấm một viên ở xưởng / giữa bàn để chọn màu, rồi bấm hàng trên bảng của bạn (hàng hợp lệ viền xanh, sàn viền đỏ).
- Rê chuột lên hàng để xem trước viên nào vào hàng, viên nào rơi xuống sàn.
- Phím 1–5 chọn hàng, 0 bỏ xuống sàn, Esc chọn lại.

## Kỹ thuật
Một file `index.html` duy nhất. Kết nối P2P bằng [PeerJS](https://peerjs.com/), cùng khung với Jaipur, 7 Wonders Duel và Floristry.
Chạy thử: `npx http-server azul -p 5183`.
