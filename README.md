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

Người học là trẻ 9–10 tuổi. Mục tiêu: con hiểu **vì sao** làm từng việc, nhưng không phải đọc một "tài liệu hướng dẫn" kiểu người lớn.

### Cách trình bày cho trẻ (đúc từ tìm hiểu về UX và học tập của trẻ em)

- **Lời hướng dẫn là lời nói, không phải văn bản.** Mỗi lần chỉ một bong bóng, một ý ngắn, giọng bố mẹ nói với con ("Xoay tầng trên. Đưa bạn góc vào vòng tròn.").
  Không gạch đầu dòng, không nhãn kiểu "Kết quả:", "Vì sao:".
- **Cho xem thay vì mô tả.** Khối tự diễn đúng lời đang nói; viên đang nhắc tới có viền hồng, chỗ cần tới có vòng tròn, hướng xoay có mũi tên.
- **Kết quả hiện ra đúng lúc nó xảy ra.** Làm xong một bước, máy reo ngay trên khối ("Bạn góc về nhà rồi!") thay cho dòng mô tả in sẵn.
- **Lý do không bày sẵn.** Con tò mò thì bấm **"Vì sao thế?"** trong bong bóng; lý do là một câu cụ thể, nhìn thấy được trên khối.
- **Gọi tên theo thế giới của trẻ**, dùng nhất quán: *bạn cạnh*, *bạn góc*, *bạn hồng* (viên có viền hồng), *về nhà* (đúng chỗ), *chiêu* (công thức),
  *Thang máy*, *đổi ghế*, xếp khối *như xây nhà* (móng, tầng giữa, nóc). Giọng văn trong trẻo, hóm hỉnh nhẹ, nhìn bằng mắt trẻ con.
- **Xem → làm cùng → tự làm**, giúp đỡ giảm dần: có mũi tên, hết mũi tên, rồi chỉ còn gợi ý khi con xin.
- **Giọng đọc (tùy chọn).** Máy có giọng tiếng Việt thì hiện nút 🗣 trên thanh tiêu đề và nút "🔈 Nghe" trong bong bóng. Mặc định tắt.

Khi sửa lời: một câu một ý, khoảng 10 từ; xưng "con"; viên là "bạn"; động từ cụ thể; tránh từ trừu tượng.

### Trang chủ

- Nút **Học tiếp** (lúc nào cũng chỉ một việc cần làm tiếp), **Bản đồ 7 chặng** xếp theo 3 tầng kèm hình khối khi xong từng chặng, và 3 việc của mỗi chặng.
  Quy tắc vàng, ôn tập, người học được thu gọn bên dưới.
- **Làm quen với khối** (9 trang, mỗi trang một lời): ô giữa, màu của mỗi mặt, các bạn nhỏ, xây từng tầng (có nút **Xem máy xây cả khối**:
  máy giải trọn một khối trong khoảng nửa phút và báo đang ở chặng nào), mặt trước, cách xoay, dấu trên khối, ba việc, quy tắc vàng.

### Mỗi chặng có 3 việc

1. **Xem**: 4 thẻ kể chuyện. Thẻ đầu là hình khối khi xong chặng; các thẻ sau mỗi thẻ một ý, khối tự diễn. Thẻ cuối có nút xem máy làm cả chặng,
   các chiêu của chặng, và các trường hợp lạ (thu gọn).
2. **Làm theo**: vòng 1 có mũi tên hồng, vòng 2 không còn mũi tên. Mỗi lúc chỉ một bong bóng cho bước đang làm.
3. **Tự làm**: tự giải trên máy, rồi chuyển sang **Trên khối thật** ngay trong cùng thẻ.

Thi tốt nghiệp sau chặng 7, ôn lại sau 1, 3, 7 ngày.

### Không xoay được thì luôn nói vì sao

- Lời ngắn hiện trên khối, lý do nằm lại trong ô cam cho đến khi con bấm "Con hiểu rồi" hoặc xoay được nước tiếp theo.
- Lớp giữa: các ô giữa phải ngồi yên làm mốc. Đang Nhìn quanh: bấm nút dễ nhầm lớp. Thẻ Xem / Khối thật: khối chỉ là hình mẫu. Khối đã xong: xoay nữa là hỏng.
- Ở Làm theo, xoay khác hướng dẫn thì khối tự quay lại, kèm một câu ngắn (ví dụ "Chiêu phải làm đúng thứ tự.").
- Nút **📖 Quy ước** gom tên gọi và các lý do trên; bấm một dòng thì khối nhấp nháy đúng chỗ.

### Nội dung nằm ở đâu trong mã

- `KNOW[k].story`: các thẻ kể chuyện của chặng (lời + hình khối tự diễn). `FWHY`: mỗi chiêu làm được việc gì. `INTRO`: các trang Làm quen.
- Trong bộ giải, mỗi `seg(t, …, { g, w })`: `t` là lời nói cho bước, `g` là lời reo khi xong, `w` là lý do khi con hỏi.

### Những thứ giữ nguyên

- **Gợi ý 3 mức**: Gợi ý nhẹ (vẫn tính là tự làm) → Gợi ý → Chỉ từng bước. Ngồi yên 30 giây thì được nhắc nhẹ.
- **Khen sự chăm chỉ**: khối nào giải xong cũng được tính; mốc 3, 5, 10, 20… khối; tự giải 3 khối ở một chặng là Thành thạo 🏅.
- Không đồng hồ, không đếm nước khi học; chỉ bài thi tốt nghiệp có đồng hồ.
- **Quy tắc vàng**: 7 điều, có ở trang chủ (thu gọn), trang cuối phần Làm quen, và mỗi chặng nhắc lại 1 điều phù hợp.
- **Hiệu ứng**: pháo giấy khi xong, âm thanh + rung (nút 🔊 để tắt).
