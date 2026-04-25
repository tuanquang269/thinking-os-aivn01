# Thinking OS · Hệ điều hành tư duy CEO Kỷ nguyên AI

Closing keynote deck · AIVN Summit #01 · Hà Nội · 25—26.04.2026
Speaker: **Kevin Kreative** · PATI Group · Wellness Nest

---

## Talk structure (90 phút)

| Tier | Nội dung | Thời lượng | Slides |
|------|----------|------------|--------|
| **I** | Bối cảnh · Vì sao CEO Việt cần OS mới | 12 phút | S01–S05 |
| **II** | Thinking OS · 3 phần (Nhân · Nguyên tắc · Công cụ) | 20 phút | S06–S13 |
| **III** | OS chạy thực chiến tại PATI Group | 38 phút | S14–S26 |
| **IV** | AI Fluency at Parity · 3 việc sáng thứ 2 | 15 phút | S27–S31 |

Tổng: **31 slides · ~2.9 phút/slide · 85 phút nội dung + 5 phút Q&A**

---

## Chạy local

Mở `index.html` trong bất kỳ trình duyệt hiện đại nào. Không cần build step.

```bash
# macOS
open index.html

# hoặc chạy local server
python3 -m http.server 8080
# → http://localhost:8080
```

---

## Deploy GitHub Pages

1. Tạo repo mới trên GitHub (gợi ý tên: `thinking-os-aivn01`)
2. Push toàn bộ folder này lên nhánh `main`
3. Settings → Pages → Source: **Deploy from a branch** → Branch: **main** → Folder: **/ (root)**
4. Live tại `https://[your-github-user].github.io/thinking-os-aivn01/`

Deploy xong thường mất 1-2 phút. Deck là pure HTML/CSS/JS, không cần Jekyll hay build step.

---

## Navigation

| Phím | Hành động |
|------|-----------|
| `→` / `Space` / `PageDown` | Slide kế tiếp |
| `←` / `PageUp` | Slide trước |
| `Home` | Về slide đầu |
| `End` | Đến slide cuối |
| `F` | Toàn màn hình |
| Click trái/phải màn hình | Tới/lui |

Deep link: `index.html#14` → mở thẳng vào slide 14.

---

## Xuất PDF (backup cho event)

1. Mở deck trong **Chrome** hoặc **Edge**
2. `Cmd/Ctrl + P` → Print
3. Destination: **Save as PDF**
4. Paper size: **Custom · 1600 × 900 px** (landscape)
5. Margins: **None**
6. Background graphics: **Enabled**

Print CSS đã configured sẵn để mỗi slide = 1 trang.

---

## PATI metrics · TBD placeholders

Mọi chỗ hiển thị `[N]`, `[X]`, `[Y]` với nền vàng là **placeholder** — Kevin điền số thật trước ngày 25.04.2026.

Danh sách ô cần điền:

**S17 · Tim Cook**
- `[N]` quyết định/ngày (sau)
- `[M]` quyết định/ngày (trước)

**S18 · Bezos**
- `[N]` email/ngày xử lý
- `[X]s` response time (sau)
- `[Y]h` response time (trước)
- `[Z]%` cost/ticket vs human

**S19 · CR7**
- `[N]` SKU giám sát
- `[M]` order/tháng xử lý
- `[X]` ngày 0 lỗi fulfillment

**S20 · Naval**
- `[N]` flows active
- `[X]%` retention rate
- `[Y]×` LTV/CAC ratio

**S21 · Jobs**
- `[N]` pieces content/tháng
- `[X]%` cost per piece vs agency
- `[Y]×` sản lượng nhân

**S22 · Elon**
- `[X]%` conversion rate
- `[Y] VND` AOV
- `[N]` test/tuần

**S26 · Dashboard**
- `[1 vs N]` headcount
- `[X] VND` fixed cost/month
- `[Y] VND` benchmark fixed cost
- `[X] giây` CS response time
- `[Y] giờ` CS response time (trước)
- `[N]×` content output multiplier
- `[Z]%` cost per piece
- `[X] VND` revenue/headcount PATI
- `[Y] VND` revenue/headcount median DTC SEA
- `[M → K]` CEO decision bandwidth

Tổng: ~20 placeholders.

---

## Chỉnh sửa nội dung

Mọi slide là `<section class="slide">` trong `index.html`. Tìm slide theo `data-slide="N"` hoặc comment `<!-- SNN · ... -->`.

Placeholder hiển thị bằng class `.tbd`:

```html
<span class="tbd">[N] email/ngày</span>
```

Khi điền số thật, giữ class `.tbd` nếu muốn highlight vàng, hoặc bỏ class để hiển thị bình thường.

---

## Brand tokens

CSS variables trong `:root` của `index.html`:

```css
--bg: #0a1628;            /* Deep navy */
--gold: #c9a961;          /* xLeader-style gold */
--ink: #f5f0e8;           /* Warm off-white */
--pati-green: #54B94A;    /* Wellness Nest brand */
```

Fonts: **Fraunces** (display serif) · **Plus Jakarta Sans** (body) · **JetBrains Mono** (system labels) — Google Fonts.

---

© 2026 · PATI Group · All rights reserved
