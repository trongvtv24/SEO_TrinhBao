# TEMPLATE 3 — EDIT_REPORT.md
# (Editor Agent output: gồm EDITED_ARTICLE + EDIT_REPORT)

> Mục đích: biên tập bản nháp để tăng logic, giọng văn, độ rõ ràng nhưng giữ đúng intent và mục tiêu bài trong `CONTENT_BRIEF`.  
> Người tạo: **Editor Agent**  
> Người nhận tiếp theo: SEO Lead / Publish stage (hoặc trả về Writer/Researcher)

---

## 0) Thông tin phiên biên tập
- **Edit ID:** [EDIT-YYYYMMDD-001]
- **Linked Brief ID:** [BRIEF-YYYYMMDD-001]
- **Linked Draft ID:** [DRAFT-YYYYMMDD-001]
- **Ngày biên tập:** [YYYY-MM-DD]
- **Người tạo:** Editor Agent
- **Trạng thái:** `PASS` | `REVISE_WRITER` | `REVISE_RESEARCH`

---

## 1) Kiểm tra đầu vào (bắt buộc)
### 1.1 Tài liệu đã đối chiếu
- [ ] `CONTENT_BRIEF`
- [ ] `DRAFT_ARTICLE`

### 1.2 Xác nhận hiểu brief (Editor)
- **Loại bài:** [Vệ tinh / Commercial / Chủ lực]
- **Mục tiêu bài:** [___]
- **Intent chính:** [___]
- **Central Search Intent (1 câu):**  
  > [___]

### 1.3 Kết quả kiểm nhanh trước khi edit
- **Draft có đúng loại bài không?** [Có / Không]
- **Draft có lệch intent lớn không?** [Có / Không]
- **Draft có thiếu section bắt buộc không?** [Có / Không]
- **Draft có dấu hiệu tự bịa dữ liệu không?** [Có / Không]

> Nếu “Có” ở các lỗi hướng đi lớn → cân nhắc `REVISE_WRITER` hoặc `REVISE_RESEARCH` thay vì cố edit vá.

---

## 2) EDITED_ARTICLE (Bản đã biên tập hoàn chỉnh)
> Dán toàn bộ nội dung sau biên tập tại đây.  
> Giữ các placeholder `[CẦN DỮ LIỆU THẬT]` / `[CẦN XÁC NHẬN]` nếu chưa được xác minh.

---

### Metadata (đã biên tập nếu có chỉnh)
- **SEO Title:** [___]
- **Meta Description:** [___]
- **Slug:** [___]
- **H1:** [___]

---

### Nội dung đã biên tập (FULL)
[PASTE FULL EDITED ARTICLE HERE]

---

### Internal link block (nếu giữ/điều chỉnh)
1. **URL:** [___]
   - **Anchor text:** [___]
   - **Vị trí:** [___]

2. **URL:** [___]
   - **Anchor text:** [___]
   - **Vị trí:** [___]

---

## 3) EDIT_REPORT (Báo cáo biên tập)

### 3.1 Kết luận
- **Kết quả:** `PASS` | `REVISE_WRITER` | `REVISE_RESEARCH`

### 3.2 Tóm tắt lý do kết luận (2–6 dòng)
[___]

---

## 4) Những chỉnh sửa chính đã thực hiện
> Chỉ tập trung vào logic / giọng văn / độ rõ ràng (đúng vai Editor).

### 4.1 Logic & cấu trúc
- [ ] Sắp xếp lại trình tự ý
- [ ] Cắt bớt đoạn lan man
- [ ] Gộp ý trùng
- [ ] Tách đoạn quá dài
- [ ] Làm rõ chuyển đoạn
- **Chi tiết chỉnh sửa:**  
  - [___]
  - [___]

### 4.2 Giọng văn & độ rõ ràng
- [ ] Rút gọn câu dài
- [ ] Làm rõ thuật ngữ
- [ ] Chuẩn hóa giọng văn
- [ ] Tăng khả năng đọc trên mobile
- **Chi tiết chỉnh sửa:**  
  - [___]
  - [___]

### 4.3 Bảo toàn intent & mục tiêu bài
- **Cách đã giữ intent:** [___]
- **Đoạn từng có nguy cơ lệch intent (nếu có):** [___]

---

## 5) Lỗi còn tồn tại / cần xử lý tiếp
> Ghi rõ để bước sau không bỏ sót.

### 5.1 Dữ liệu chưa xác nhận
- `[CẦN DỮ LIỆU THẬT]` [___]
- `[CẦN XÁC NHẬN]` [___]

### 5.2 Vấn đề thuộc về Writer (nếu trả Writer)
- [___]
- [___]

### 5.3 Vấn đề thuộc về Researcher (nếu trả Research)
- [___]
- [___]

---

## 6) Tiêu chí trả bài (nếu không PASS)
### 6.1 Nếu `REVISE_WRITER`
> Dùng khi hướng đúng nhưng thực thi viết chưa đạt.

**Lý do trả Writer:**
- [ ] Thiếu section bắt buộc
- [ ] Lan man / lặp ý nhiều
- [ ] Chưa bám outline
- [ ] FAQ/CTA/internal link block thiếu
- [ ] Viết khó hiểu / chưa đủ rõ
- [ ] Khác: [___]

**Yêu cầu Writer sửa cụ thể:**
1. [___]
2. [___]
3. [___]

### 6.2 Nếu `REVISE_RESEARCH`
> Dùng khi lỗi nằm ở hướng đi / brief.

**Lý do trả Researcher:**
- [ ] Intent mơ hồ / mâu thuẫn
- [ ] Keyword cluster lệch intent
- [ ] Outline không phù hợp loại bài
- [ ] Thiếu dữ liệu cốt lõi trong brief
- [ ] Thiếu phân tích SERP Top 10 đối thủ (bỏ qua Ads)
- [ ] SERP direction sai
- [ ] Khác: [___]

**Yêu cầu Researcher sửa cụ thể:**
1. [___]
2. [___]
3. [___]

---

## 7) Checklist tự kiểm của Editor (bắt buộc)
- [ ] Đã đối chiếu cả brief và draft trước khi edit
- [ ] Bài sau edit vẫn đúng loại bài
- [ ] Không lệch intent chính
- [ ] Logic mạch lạc hơn bản nháp
- [ ] Giọng văn rõ ràng, dễ đọc hơn
- [ ] Không tự thêm claim vô căn cứ
- [ ] Không xóa phần quan trọng (FAQ/CTA/internal link block) mà không ghi chú
- [ ] Đã giữ / đánh dấu các placeholder dữ liệu thiếu
- [ ] Kết luận `PASS / REVISE_WRITER / REVISE_RESEARCH` rõ ràng

---

## 8) Handoff note cho bước tiếp theo (SEO/Publish hoặc vòng sửa)
### Nếu `PASS`
- **Sẵn sàng cho bước SEO On-page / Publish:** [Có]
- **Khuyến nghị tối ưu tiếp (nếu có):**
  - [___]
  - [___]

### Nếu `REVISE_WRITER` hoặc `REVISE_RESEARCH`
- **Ưu tiên sửa trước:** [___]
- **Không cần sửa thêm ở vòng này:** [___]