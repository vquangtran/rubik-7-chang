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

Mục tiêu: giúp trẻ vượt qua nỗi sợ "khó", chịu khó thực hành và học từng bước nhỏ. Không chấm điểm, không đua thời gian.

- **7 chặng × 4 bước**: Xem → Làm theo → Tự làm → Khối thật. Thi tốt nghiệp sau chặng 7, ôn lại sau 1, 3, 7 ngày.
- **Màn Xem từng bước một**: mở đầu bằng hình kết quả, rồi mỗi lần chỉ một bước, khối tự làm mẫu đúng bước đó.
  Công thức được nhắc trong bước nào thì hiện ngay ở bước đó. Có thể chuyển sang xem tất cả các bước cùng lúc.
- **Lời từng bước ngắn gọn**: mỗi bước một câu ngắn nói việc cần làm; lời giải thích chỉ hiện ở bước đang làm.
  Trên khối luôn có nhãn **Mặt trước / Mặt phải / Mặt trên**; mặt mà bước đang làm nói tới thì nhãn đổi sang màu hồng.
  Chỗ cần đưa viên tới được khoanh **vòng tròn** ngay trên khối, không phải tả bằng lời ("góc trên bên phải của mặt trước").
- **Quy ước gọi tên**: mỗi từ (mặt trước, tầng trên, cột phải, viên cạnh, cánh hoa, khớp màu, tên công thức…) chỉ có một nghĩa.
  Trong lời hướng dẫn, từ nào có quy ước thì gạch chân: bấm vào là hiện nghĩa và khối nhấp nháy đúng chỗ đó.
  Nút **📖 Quy ước** dưới khối mở cả bảng. Dưới các bước có dòng chú thích: viền hồng = viên đang nói tới, vòng tròn = chỗ cần tới, mũi tên = hướng xoay.
- **Không xoay được thì luôn nói vì sao**: xoay sai ở màn Làm theo (khối quay lại chỗ cũ, có lời giải thích ngay dưới bước đang làm),
  kéo khối ở màn Xem / Khối thật, bấm nút khi đang Nhìn quanh, vuốt lớp giữa, khối đã xong, chưa có bước để lùi.
- **Gợi ý 3 mức**: Gợi ý nhẹ (chỉ nói tình huống, khoanh viên cần làm, vẫn tính là tự làm) → Gợi ý → Chỉ từng bước.
- **Nhắc nhẹ**: ngồi yên 30 giây ở màn Tự làm thì nút Gợi ý nhẹ nhấp nháy kèm lời nhắc; ở vòng 2 màn Làm theo thì nhắc nút "Chỉ cho mình bước này".
- **Khen sự chăm chỉ**: khối nào giải xong cũng được tính là đã luyện (kể cả khi có gợi ý). Đếm số khối mỗi chặng và tổng cộng, có mốc 3, 5, 10, 20… khối.
- **Thành thạo 🏅**: tự giải 3 khối ở một chặng (cộng dồn, không cần liên tiếp).
- Không đồng hồ, không đếm nước khi học; chỉ bài thi tốt nghiệp có đồng hồ.
- **Quy tắc vàng**: 7 điều giúp học tốt, có ở trang chủ, trang cuối phần Làm quen, và mỗi chặng nhắc lại 1 điều phù hợp.
- **Hiệu ứng**: pháo giấy khi xong, âm thanh + rung (nút 🔊 trên thanh tiêu đề để tắt).
