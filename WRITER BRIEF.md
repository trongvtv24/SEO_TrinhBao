# TEMPLATE 2 — DRAFT_ARTICLE.md
# (Writer Agent output)

> Mục đích: viết bản nháp hoàn chỉnh dựa trên `CONTENT_BRIEF`, đúng intent và đúng cấu trúc.  
> Người tạo: **Writer Agent**  
> Người nhận: **Editor Agent**

---

## 0) Thông tin bản nháp
- **Draft ID:** [DRAFT-YYYYMMDD-001]
- **Linked Brief ID:** [BRIEF-YYYYMMDD-001]
- **Ngày tạo:** [YYYY-MM-DD]
- **Người tạo:** Writer Agent
- **Trạng thái:** `DRAFT_COMPLETE` | `REVISE_RESEARCH_NEEDED`

---

## 1) Tóm tắt brief (Writer tự xác nhận trước khi viết)
> Bắt buộc để chứng minh Writer hiểu đúng brief.

- **Loại bài:** [Vệ tinh / Commercial / Chủ lực]
- **Mục tiêu bài:** [___]
- **Đối tượng đọc:** [___]
- **Intent chính:** [___]
- **Intent phụ (nếu có):** [___]
- **Central Search Intent (1 câu):**  
  > [___]
- **URL/CTA cần hỗ trợ:** [___]

### Cảnh báo trước khi viết (nếu có)
- `[CẦN RESEARCH LẠI]` [___]
- `[CẦN DỮ LIỆU THẬT]` [___]

> Nếu phần này không rõ → Writer phải trả về Researcher, không tự bẻ hướng.

---

## 2) Metadata Draft (bắt buộc)
- **SEO Title (draft):** [___]
- **Meta Description (draft):** [___]
- **Slug (draft):** [___]
- **H1:** [___]

### Ghi chú metadata (nếu có)
- [___]

---

## 3) Dàn ý thực thi (outline đã dùng)
> Giúp Editor so đối chiếu nhanh với brief.

- **Mở bài**
  - [ ] Hook / xác nhận vấn đề
  - [ ] Lợi ích bài viết
  - [ ] Chuyển vào nội dung

- **H2/H3 đã triển khai**
  - H2. [___]
    - H3. [___]
    - H3. [___]
  - H2. [___]
    - H3. [___]
    - H3. [___]
  - H2. [FAQ]
    - [___]
    - [___]
    - [___]

- **Kết bài / CTA**
  - [___]

---

## 4) Nội dung bản nháp hoàn chỉnh (FULL DRAFT)

> **Quy tắc cho Writer Agent:**
> - Viết full nội dung, không bàn giao outline trống.
> - Không tự bịa dữ liệu.
> - Chỗ thiếu dùng tag `[CẦN DỮ LIỆU THẬT]`.

---

### Mở bài
[Viết mở bài hoàn chỉnh tại đây]

---

### H2. [Tiêu đề H2 số 1]
[Nội dung]

#### H3. [Tiêu đề H3]
[Nội dung]

#### H3. [Tiêu đề H3]
[Nội dung]

---

### H2. [Tiêu đề H2 số 2]
[Nội dung]

#### H3. [Tiêu đề H3]
[Nội dung]

#### H3. [Tiêu đề H3]
[Nội dung]

---

### H2. [Tiêu đề H2 số 3]
[Nội dung]

---

### H2. FAQ
#### [Câu hỏi 1]
[Trả lời]

#### [Câu hỏi 2]
[Trả lời]

#### [Câu hỏi 3]
[Trả lời]

> (Thêm FAQ nếu brief yêu cầu)

---

### Kết bài / CTA
[Nội dung kết bài và lời kêu gọi hành động phù hợp mục tiêu bài]

---

## 5) Internal Link đề xuất (bắt buộc nếu brief có URL hỗ trợ)
> Writer không chèn link thật nếu chưa có URL final thì vẫn phải đề xuất vị trí + anchor.

### Danh sách internal link đề xuất
1. **URL:** [___]
   - **Anchor text:** [___]
   - **Vị trí chèn:** [Mở bài / H2 số ... / Kết bài]
   - **Mục tiêu:** [Điều hướng / hỗ trợ chuyển đổi / đọc thêm]

2. **URL:** [___]
   - **Anchor text:** [___]
   - **Vị trí chèn:** [___]
   - **Mục tiêu:** [___]

---

## 6) Placeholder dữ liệu cần xác nhận (bắt buộc nếu có)
> Dùng đúng tag để Editor/SEO Lead thấy rõ.

### Danh sách `[CẦN DỮ LIỆU THẬT]`
- `[CẦN DỮ LIỆU THẬT]` [Phần / đoạn / claim] — [Cần gì?]
- `[CẦN DỮ LIỆU THẬT]` [Phần / đoạn / claim] — [Cần gì?]

### Danh sách `[CẦN XÁC NHẬN]`
- `[CẦN XÁC NHẬN]` [Thuật ngữ / tên gọi / chính sách / số lượng]
- `[CẦN XÁC NHẬN]` [___]

---

## 7) Ghi chú cho Editor Agent
### 7.1 Điểm Writer tự thấy còn yếu / cần edit mạnh
- [___]
- [___]

### 7.2 Đoạn cần Editor chú ý giữ intent
- [___]

### 7.3 Đoạn có thể rút gọn nếu cần
- [___]

---

## 8) Checklist tự kiểm của Writer (bắt buộc)
- [ ] Đã viết **full draft**, không chỉ outline
- [ ] Bài bám đúng `CONTENT_BRIEF`
- [ ] Không lệch intent chính
- [ ] Có mở bài + thân bài + kết bài
- [ ] Có FAQ theo yêu cầu brief
- [ ] Có CTA phù hợp loại bài
- [ ] Có đề xuất internal link
- [ ] Không tự bịa dữ liệu
- [ ] Đã gắn tag `[CẦN DỮ LIỆU THẬT]` / `[CẦN XÁC NHẬN]` nếu thiếu

---

## 9) Kết luận bàn giao
- **Trạng thái bàn giao cho Editor:** `READY_FOR_EDITING` | `REVISE_RESEARCH_NEEDED`
- **Lý do (nếu cần revise):** [___]