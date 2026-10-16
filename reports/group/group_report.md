# Báo cáo nhóm

## 1. Thông tin nhóm

- Tên nhóm: P100 (Team100 — Vcare)
- Đề CS13: Đề 1 — SổSạch, trợ lý đọc hóa đơn đầu vào cho văn phòng kế toán dịch vụ
- Thành viên: xem [team/TEAM.md](../../team/TEAM.md).

## 2. Mục tiêu và cách tiếp cận

Ban lãnh đạo cần lộ trình 12 tháng. Nhóm trả lời ba câu: làm gì trước, khi nào cho máy tự nhập nhiều hơn, khi nào dừng.

Căn cứ lấy từ hồ sơ tình huống Đề 1:
- **Kết quả cổng phát hành bản 2:** đạt 97,3%, 0 lỗi nghiêm trọng, kappa 0,90.
- **Công cụ có sẵn:** phần mềm kế toán đã nhập được hóa đơn điện tử; có dịch vụ tra cứu MST; chưa có dữ liệu hạch toán.
- **Giờ chuyên gia:** chị Hạnh 3 giờ/tuần; một vòng chấm bộ đề tốn 8,5 giờ.
- **Số liệu kinh tế:** 9 dòng ở trang 2.
- **Ràng buộc của chị Hạnh:** "Sai MST hay sai tiền thì không được lần nào."

## 3. Giải pháp

**Ưu tiên (trang 1)** — 6 việc gợi ý, cộng thêm việc 7 là kiểm chứng doanh thu:
- **Làm trước:**
  - Đối chiếu MST (hạng 1): mua, tức tích hợp dịch vụ tra cứu.
  - Gắn cờ hóa đơn (hạng 2): tự làm.
  - Đọc ảnh bản 2 (hạng 4): tự làm, vì đã qua cổng phát hành.
  - Kiểm chứng doanh thu (hạng 3).
- **Nhập hóa đơn điện tử:** mua, vì phần mềm kế toán đã có tính năng này.
- **Gợi ý hạch toán:** chờ, vì chưa có dữ liệu.
- **Hỏi đáp thuế:** không làm, vì rủi ro bị nuốt 0,9.

**Mức tự động (trang 2):**

| Mức | % duyệt | Chi phí/hóa đơn | Biên gộp | Cổng |
|---|---|---|---|---|
| 0 | 100% | 1.704 đ | 24% | — (bản 2 đã phát hành) |
| 1 | 20% | 704 đ | 69% | 0 lỗi MST/tiền trên ≥ 3.000 hóa đơn; cờ ≤ 20%, cờ thừa ≤ 10% |
| 2 | 10% | 579 đ | 74% | 0 lỗi MST/tiền trên ≥ 10.000 hóa đơn, ≥ 3 văn phòng |
| 3 | 5% | 517 đ | 77% | 0 lỗi MST/tiền trên ≥ 30.000 hóa đơn trong 2 tháng, ≥ 10 văn phòng |

Cỡ mẫu chọn theo quy tắc ba: 0 lỗi trên n ca thì lỗi thật dưới khoảng 3/n.

## 4. Kết quả

- **File Excel:** `P100_CS13.xlsx`. Trang 6 tự kiểm tra đạt 8/8, trang 0 đạt 6/6.
- **Kinh tế:** doanh thu 2.256 đ/hóa đơn. Mức 1 trở lên đều có biên ≥ 60%; Mức 0 chỉ 24%. Kịch bản xấu hết tiền ở tháng 7, nên phải lên Mức 1 trong 3 tháng đầu.
- **Slide lãnh đạo:** `P100_CS13_Slide.pptx`.

## 5. Khó khăn và cách xử lý

- **Giờ chuyên gia ít:** chị Hạnh chỉ có 3 giờ/tuần, nên không thể nhờ chị chấm bộ đề lớn. Thay vào đó, cổng dùng hóa đơn thật đã được kế toán viên duyệt 100% ở Mức 0. Chị Hạnh chỉ kiểm 1% (khoảng 120 hóa đơn/tháng, tức khoảng 3 giờ), còn anh Tùng chấm bộ đề.
- **Việc 4 xếp hạng 1 nhưng đã có dịch vụ sẵn:** nhóm chọn Mua (tích hợp) thay vì tự xây.

## 6. Tổng hợp đóng góp

Xem [team/TEAM.md](../../team/TEAM.md).

## 7. Hạn chế và hướng cải thiện

- **Điểm F–L là tự chấm:** tỷ lệ hóa đơn ảnh so với hóa đơn điện tử chưa có trong hồ sơ.
- **Giả định gia hạn chưa kiểm chứng:** văn phòng dùng nhiều sẽ gia hạn hay không, sẽ xem lại ở ngày 90.
- **Tầng Nguy hiểm quá mỏng:** bộ đề 40 ca chỉ có khoảng 3 ca tầng này, nên trước khi lên Mức 2 cần mở rộng bộ đề lên ≥ 80 ca.

## 8. Tài liệu tham khảo

- CS13_HoSoTinhHuong.pdf, Đề 1
- CS13_SlideLop_AIRoadmap.pdf, slide 70–86 (công thức ở slide 74)
- CS13_Roadmap_Mau.xlsx (cách điền)
- Luật Trí tuệ nhân tạo 134/2025/QH15; Nghị định 142/2026/NĐ-CP
