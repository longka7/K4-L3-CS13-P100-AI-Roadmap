# K4-L3-CS13-P100-AI-Roadmap

- **Nhóm:** P100 (Team100 — Vcare) · Track 1 · Khóa 4
- **Đề:** Đề 1 — SổSạch, trợ lý đọc hóa đơn đầu vào cho văn phòng kế toán dịch vụ
- **1 việc:** 1 hóa đơn được đọc, đối chiếu và nhập vào phần mềm kế toán
- **Thành viên và phân công:** [team/TEAM.md](team/TEAM.md)

## Bài nộp

| File | Nội dung |
|---|---|
| [P100_CS13.xlsx](P100_CS13.xlsx) | Excel làm bài, trang 0–6; tự kiểm tra 8/8 |
| [P100_CS13_Slide.pptx](P100_CS13_Slide.pptx) | 1 slide lãnh đạo, số liệu khớp trang 5 |
| [reports/group/group_report.md](reports/group/group_report.md) | Báo cáo nhóm |

## Ba câu trả lời

- **Làm gì trước:** đối chiếu MST người bán bằng dịch vụ tra cứu có sẵn (hạng 1, mua) và gắn cờ hóa đơn cần người xem (hạng 2). Song song, vận hành bản 2 đọc ảnh và kiểm chứng doanh thu với 30% văn phòng dùng nhiều.
- **Khi nào để AI tự làm nhiều hơn:**
  - Lên Mức 1 (duyệt 20%, chi phí 704 đ/hóa đơn, biên 69%) khi không có lỗi MST/tiền nào trên ít nhất 3.000 hóa đơn thật, gắn cờ ≤ 20%, cờ thừa ≤ 10% và chị Hạnh xác nhận.
  - Lên Mức 2 (duyệt 10%, biên 74%) khi không có lỗi MST/tiền nào trên ít nhất 10.000 hóa đơn của ≥ 3 văn phòng.
- **Khi nào dừng:**
  - Có 1 lỗi MST/tiền lọt vào sổ → lùi ngay về Mức 0.
  - Doanh thu bình quân < 3,71 triệu/văn phòng trong 2 tháng liên tiếp, trên ≥ 10 văn phòng → dừng mở rộng.
