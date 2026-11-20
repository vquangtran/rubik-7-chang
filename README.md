# Rubik 7 Chặng

Trò chơi/hướng dẫn học giải khối rubik qua 7 chặng, viết dưới dạng một trang HTML tự chứa (HTML + CSS + JS inline).

## Chạy thử

Mở trực tiếp `index.html` trong trình duyệt, hoặc chạy một server tĩnh:

```bash
python3 -m http.server 8000
```

rồi vào http://localhost:8000.

## Cấu trúc

- `index.html` — toàn bộ ứng dụng (bản gốc từ artifact).

## Cách chơi

Mục tiêu: giúp trẻ vượt qua nỗi sợ "khó", hiểu **vì sao** làm từng việc chứ không chỉ làm theo. Không chấm điểm, không đua thời gian.

### Tổng quan trước, chi tiết sau

- **Trang chủ** chỉ có ba thứ chính: nút **Học tiếp** (lúc nào cũng chỉ một việc cần làm tiếp), **Bản đồ** 7 chặng xếp theo 3 tầng
  (tầng dưới: chặng 1–2, tầng giữa: chặng 3, tầng trên: chặng 4–7; mỗi chặng có hình khối khi xong chặng đó), và **3 việc của mỗi chặng**.
  Quy tắc vàng, ôn tập, người học được thu gọn bên dưới.
- **Làm quen với khối** (8 trang): ô giữa, viên cạnh/viên góc, *xếp từng tầng từ dưới lên*, tên gọi, cách xoay, dấu trên khối, 3 việc, quy tắc vàng.
  Trang "Xếp từng tầng" có nút **Xem máy giải cả khối**: máy giải trọn một khối trong khoảng nửa phút, vừa giải vừa báo đang ở chặng nào,
  và giải thích vì sao cần công thức.

### Mỗi chặng có 3 việc

1. **Hiểu**: một màn tổng quan gồm *Đích* (khối lớn hiện đúng kết quả), *Vì sao làm chặng này*, và 3 *Ý chính* (bấm dòng có ▸ để máy minh họa trên khối).
   Từ đây vào thẳng Làm theo, hoặc xem máy làm mẫu từng bước. Công thức, trường hợp khác, máy làm mẫu từng trường hợp được thu gọn.
2. **Làm theo**: vòng 1 có mũi tên hồng, vòng 2 chỉ còn lời nhắc. Bước đang làm nằm trên cùng.
3. **Tự làm**: tự giải trên máy, rồi chuyển sang **Trên khối thật** ngay trong cùng thẻ.

Thi tốt nghiệp sau chặng 7, ôn lại sau 1, 3, 7 ngày.

### Ít chữ: mỗi câu một việc

- Dòng lệnh chỉ nói **một hành động** ("Xoay tầng trên."). Kết quả và lý do nằm ở hai dòng riêng, mỗi dòng một ý ngắn.
- Bước nào gộp 2 việc thì tách thành 2 bước (ví dụ "khớp màu" và "xoay mặt đó 2 lần" ở chặng 1).
- Trang Làm quen, quy tắc vàng, lời báo khi không xoay được: đều là các dòng ngắn, không viết thành đoạn.
- Khi sửa lời, giữ quy tắc này: một câu = một hành động hoặc một đối tượng, khoảng 10 từ trở lại.

### Bước nào cũng nói rõ "được gì" và "vì sao"

- Mỗi bước (ở màn máy làm mẫu, Làm theo, và khi xin Gợi ý) có một ô vàng: **✅ Được** (xong bước này thì khối thành thế nào) và **💡 Vì sao** (lý do phải làm như vậy).
- Mỗi công thức có một dòng nói nó *làm được việc gì* (ví dụ Thang máy: cột phải lên đón viên góc, rồi xuống trả), không chỉ là dãy nước xoay.
- Nội dung nằm trong `KNOW` (vì sao của chặng, ý chính, được gì/vì sao của từng bước), `FWHY` (công thức), và `g`/`w` của từng `seg(...)` trong bộ giải.

### Không xoay được thì luôn nói vì sao

- Lời ngắn hiện trên khối, còn **lý do đầy đủ nằm lại** trong ô cam "Vì sao không xoay được?" cho đến khi con bấm "Mình hiểu rồi" hoặc xoay được nước tiếp theo.
- Lớp giữa: vì nó mang 6 ô giữa, là mốc màu của mỗi mặt. Đang Nhìn quanh: vì mặt trước không còn ở trước mặt nên các nút sẽ xoay nhầm lớp.
  Thẻ Hiểu / Khối thật: vì ở đó máy làm mẫu hoặc chỉ là hình để so. Khối đã xong: vì xoay thêm sẽ làm hỏng.
- Ở Làm theo, xoay khác hướng dẫn thì khối quay lại chỗ cũ, kèm lý do theo đúng tình huống: đang giữa công thức nào, hoặc vì sao chặng 7 không xoay cả khối.
- Nút **📖 Quy ước** có thêm mục "Vì sao có lúc không xoay được" gom tất cả các lý do trên.

### Những thứ giữ nguyên

- **Quy ước gọi tên**: mỗi từ chỉ có một nghĩa; từ có quy ước thì gạch chân, bấm vào là hiện nghĩa và khối nhấp nháy đúng chỗ.
  Nhãn Mặt trước / Mặt phải / Mặt trên luôn có trên khối; viền hồng = viên đang nói tới, vòng tròn = chỗ cần tới, mũi tên = hướng xoay.
- **Gợi ý 3 mức**: Gợi ý nhẹ (vẫn tính là tự làm) → Gợi ý → Chỉ từng bước. Ngồi yên 30 giây thì được nhắc nhẹ.
- **Khen sự chăm chỉ**: khối nào giải xong cũng được tính; mốc 3, 5, 10, 20… khối; tự giải 3 khối ở một chặng là Thành thạo 🏅.
- Không đồng hồ, không đếm nước khi học; chỉ bài thi tốt nghiệp có đồng hồ.
- **Quy tắc vàng**: 7 điều, có ở trang chủ (thu gọn), trang cuối phần Làm quen, và mỗi chặng nhắc lại 1 điều phù hợp.
- **Hiệu ứng**: pháo giấy khi xong, âm thanh + rung (nút 🔊 để tắt).
