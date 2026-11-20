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

- **7 chặng × 4 bước**: Xem → Làm theo → Tự làm → Khối thật. Thi tốt nghiệp sau chặng 7, ôn lại sau 1, 3, 7 ngày.
- **Sao mỗi khối** (Tự làm, Thi, Ôn, Luyện tự do): đếm số nước xoay (không tính xoay cả khối), so với số nước máy cần:
  ≤ 1,3× → ★★★, ≤ 2× → ★★, còn lại ★. Lưu kỷ lục sao / ít nước nhất / nhanh nhất.
- **Gợi ý nhẹ**: chỉ khoanh viên cần làm và tên tình huống; vẫn được tính qua chặng, tối đa ★★.
  **Gợi ý** đầy đủ thì khối đó không tính qua chặng.
- **Thành thạo 🏅**: đúng 3 khối liên tiếp không gợi ý ở một chặng.
- **Hiệu ứng**: pháo giấy khi xong, âm thanh + rung (nút 🔊 trên thanh tiêu đề để tắt).
