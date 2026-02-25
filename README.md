# Quy Trình Tự Động Hoá Sản Xuất Content SEO (SEO Content Pipeline)

Chào mừng bạn đến với dự án **SEO Content Pipeline**. Đây là bộ quy chuẩn và hệ thống Prompt chuyên sâu giúp tự động hóa và tối ưu hóa quy trình sản xuất nội dung chuẩn SEO, đảm bảo đánh trúng Search Intent và mang lại giá trị chuyển đổi cao.

Dự án này có thể áp dụng cho:
- **Đội ngũ (Team) Content truyền thống:** Dùng các quy trình và biểu mẫu (Brief, Template) để chuẩn hoá cách làm việc.
- **AI Writer / AI Agent:** Dùng các System Prompt và Pipeline để tự động hóa quy trình viết bài với các mô hình ngôn ngữ lớn (ChatGPT, Claude, Gemini...).

## 📂 Cấu Trúc Thư Mục & File Quan Trọng

### 1. Tài liệu nền tảng
- `Tong the SEO quy trinh.md`: Quy trình SEO tổng thể. Đây là file **quan trọng nhất** cần đọc để hiểu mindset cốt lõi: từ xác định Intent, chia cấp nội dung (Bố/Mẹ - Con - Cháu), đến lập Outline và tối ưu On-page.

### 2. Các Template Bài Viết SEO
Dùng để tham khảo cấu trúc chuẩn cho từng loại bài viết khác nhau:
- `template-seo-bai-chu-luc-ho-tro-chuyen-doi.md`: Dành cho trang bán hàng, dịch vụ (Transactional/Commercial).
- `template-seo-bai-commercial-so-sanh-chon-mua.md`: Dành cho dạng bài review, so sánh, top list.
- `template-seo-bai-ve-tinh-keo-traffic.md.md`: Dành cho dạng bài cung cấp thông tin (Informational), mục đích kéo traffic và link về bài chủ lực.

### 3. Biểu mẫu (Templates/Briefs)
Dành cho quy trình làm việc thủ công giữa các thành viên:
- `CONTENT_BRIEF.md`: Mẫu Brief dùng để research và lên dàn ý.
- `WRITER BRIEF.md`: Mẫu hướng dẫn chi tiết dành cho người viết.
- `EDIT_BRIEF.md`: Mẫu checklist dành cho Editor để kiểm duyệt bài.

### 4. Hệ thống AI Agents (Thư mục `/agents`)
Tuyển tập các System Prompt siêu chi tiết, biến AI thành những chuyên gia SEO thực thụ.
- `Agent_seo-pipeline.md` (Orchestrator): Đóng vai trò là TỔNG QUẢN LÝ. Bạn chỉ cần đưa đề bài, Agent này sẽ tự động chạy ngầm cả 3 khâu: Research -> Viết -> Edit. (Khuyên dùng)
- `Agent_seo-researcher.md`: Chuyên gia phân tích từ khóa, đối thủ và thiết lập Outline / Intent bài viết.
- `Agent_seo-writer.md`: Chuyên gia viết bài chuẩn SEO dựa trên cái Brief đã được cung cấp.
- `Agent_seo-editor.md`: Chuyên gia biên tập, bắt lỗi logic, văn phong và đối chiếu Brief xem viết có đúng mục tiêu không.

*(Lưu ý: Các file `[Role] System Promt.md` ở thư mục gốc là phiên bản rút gọn, cũ hơn so với phiên bản trong thư mục `/agents`).*

## 🚀 Hướng Dẫn Sử Dụng

### CÁCH 1: Dùng luồng Auto Pipeline 100% với AI (Khuyên dùng)
Đây là cách nhanh nhất để có một bài SEO chuẩn gọn gàng.
1. Mở ChatGPT / Claude / Gemini (nên dùng các model tư duy làm việc tốt như Claude 3.5 Sonnet hoặc GPT-4o).
2. Copy toàn bộ nội dung trong file `agents/Agent_seo-pipeline.md` và dán vào làm **System Prompt** (hoặc gửi vào làm tin nhắn đầu tiên).
3. Cung cấp **Đề bài SEO** cho AI. Thông tin tối thiểu cần:
   - Chủ đề hoặc từ khóa hạt giống (Seed Keyword).
   - Ngành hàng/Lĩnh vực.
   - Website hoặc URL trang đích chủ lực cần điều hướng traffic về.
   - Mục tiêu bài viết.
4. AI sẽ tự động đóng 3 vai (Researcher -> Writer -> Editor) làm việc tuần tự. Nếu có lỗi, AI sẽ tự tạo vòng lặp **REVISE** xử lý trong nội bộ. Cuối cùng, bạn sẽ nhận được một bài viết hoàn chỉnh và Checklist On-page để đăng bài.

### CÁCH 2: Dùng từng Agent độc lập (Kiểm soát chi tiết từng khâu)
Nếu bạn muốn tự kiểm soát và duyệt tay từng bước:
1. **Bước 1 (Giao việc cho AI Researcher):** Mở file `Agent_seo-researcher.md` copy đưa cho AI kèm yêu cầu từ khóa. AI sẽ trả ra cho bạn 1 bản **CONTENT BRIEF**. Bạn lấy brief này đọc, bổ sung, chỉnh sửa thủ công nếu muốn.
2. **Bước 2 (Giao việc cho AI Writer):** Mở 1 phiên chat mới, dùng file `Agent_seo-writer.md` làm System Prompt, sau đó cung cấp cái **CONTENT BRIEF** xịn xò ở bước 1 vào cho nó viết. AI sẽ xuất ra **Bài Nháp**.
3. **Bước 3 (Giao việc cho AI Editor):** Lại mở 1 phiên chat khác, dùng `Agent_seo-editor.md` làm System Prompt, đưa cả **CONTENT BRIEF** gốc + **Bài Nháp** ở bước 2 vào để AI soát lỗi, gọt giũa văn phong và xuất bản phiên bản cuối.

### CÁCH 3: Dành cho Team Content con người (Quy trình tiêu chuẩn)
1. Cả team (Leader, SEOer, Writer) cần đọc kĩ `Tong the SEO quy trinh.md`.
2. Trưởng nhóm SEO hoặc Content Leader điền các yêu cầu vào file `CONTENT_BRIEF.md`.
3. Giao Brief cho Content Writer viết. Bạn Writer sẽ vận dụng các form mẫu `template-seo-bai...` tương ứng với thể loại để gõ bài.
4. Giao bài viết cho Content Editor duyệt theo checklist trong thẻ `EDIT_BRIEF.md`.

## 📌 Triết Lý Cốt Lõi (Core Mindset của dự án)
Hệ thống này được thiết kế và xây dựng theo chuẩn thực chiến, ưu tiên chuyển đổi, tránh viết bài rác:
1. **Central Search Intent (Ý định tìm kiếm trung tâm):** Mỗi một bài viết phải đánh trúng một intent rõ ràng nhất, không viết lan man (Ví dụ: người dùng tìm "cách lắp camera", thì đi thẳng vào cách lắp đặt, đừng mở bài luyên thuyên lịch sử ra đời của cái camera).
2. **Dữ liệu thật, KHÔNG Bullshit (Hạn chế AI Hallucination):** Bài viết AI thường bị đặc tả chung chung hoặc tự bịa thông số. Quy trình này bắt buộc các Agent đánh tag Placeholder `[CẦN DỮ LIỆU THẬT]` vào các chỗ như giá bán, thông số chuyên sâu... để người duyệt đắp dữ liệu thật của brand vào.
3. **Link Chủ Lực (Điều hướng phễu):** Viết bài vệ tinh là để kéo và điều hướng dòng traffic đổ dồn về các URL chuyển đổi hái ra tiền (Cấp Bố/Mẹ). Tuyệt đối không viết bài kéo traffic xong để đó thoát trang.

---
*Chúc bạn và team xuất bản được những nội dung SEO lên top, đánh trúng insight khách hàng và mang lại chuyển đổi cao!*
