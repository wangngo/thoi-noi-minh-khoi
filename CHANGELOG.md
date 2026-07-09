# CHANGELOG — Thiệp thôi nôi bé Minh Khôi

Trang mời self-contained (Bundled Page / DCLogic) — 1 file `index.html`, deploy GitHub Pages:
https://wangngo.github.io/thoi-noi-minh-khoi/

Kỹ thuật sửa (decode/re-encode template JSON, gotcha `</script>`): xem memory `bundled-page-dclogic-editing`.

## 2026-07-09 — Bản chủ đề siêu anh hùng (chờ khách phản hồi)
- **Nền xanh dương**: gradient `#1c6fd6 → #3f8ee6 → #7ec0f5 → #c3e4fb`; chữ header đổi trắng + shadow cho hợp nền. (`3371f62`)
- **Ảnh mới của bé**: thay ảnh chân dung (crop tròn `object-position:center 20%`). (`3371f62`)
- **Cảnh rượt đuổi** thay hàng emoji tĩnh: siêu nhân bay dẫn trước, **Minh Khôi lái siêu xe đuổi theo** (ảnh mặt bé nhỏ trong xe, vạch tốc độ, khói xả, xe rung); trễ pha 0.55s để xe bám sau. (`36328f3`)
- **Siêu nhân bay ngang bằng SVG tự vẽ** (thay emoji 🦸 đứng): thân nằm ngang kiểu Superman, tay đấm tới, áo choàng đỏ bay sau, sao vàng ngực, mặt nạ xanh. (`e07c860`)

### Đang chờ
- Phản hồi của khách (bố mẹ bé) về bản chủ đề siêu anh hùng. Các hướng chỉnh nhanh nếu cần: đổi màu áo choàng, tốc độ bay, kích thước siêu nhân, thêm chữ comic "ĐUỔI THEO!".

### Gotcha vận hành
- GitHub Pages queue có lúc **kẹt** (run "queued" >5 phút). Xử lý: `gh run cancel <id>` run kẹt + push commit rỗng để kích lại; verify live bằng marker không dính escape (vd path `M60 24 Q95 6`), KHÔNG grep chuỗi có dấu `"` (bị JSON-escape thành `\"`).
- Trình duyệt cache `max-age=600` → hard-refresh (Cmd+Shift+R) hoặc thêm `?v=<n>`.

## 2026-07-08 — Bản gốc
- Thiệp thôi nôi nền pastel, ảnh bé, countdown → nút thêm lịch (Google/ICS), confetti, RSVP tracking qua Google Form. Fix thẻ `</script>` khiến confetti + nút lịch không chạy. (`05c0eb0`, `7cf56b8`)
