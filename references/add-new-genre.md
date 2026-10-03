# Quy trình bổ sung một loại văn bản mới

Dùng khi người dùng muốn skill "học" thêm một loại văn bản chưa có trong `references/genres/` (ví dụ: luận án tiến sĩ, bài bình luận chính sách trên báo, báo cáo thẩm tra, bài phát biểu, kỷ yếu, tóm tắt chính sách – policy brief, báo cáo thường niên doanh nghiệp...).

Nguyên tắc cốt lõi: **chỉ học ngôn ngữ, không học nội dung**. Mọi quy tắc phải rút ra từ văn bản thật do người viết, không phải từ trực giác.

## Bước 1 — Xác định phạm vi

Ghi rõ trước khi research:
- Tên loại văn bản và tên file sẽ tạo: `references/genres/<slug>.md` (slug không dấu, gạch nối, ví dụ `luan-an-tien-si`).
- Lĩnh vực trọng tâm (kinh tế, quản lý, chính sách...).
- Các tiểu loại cần phủ (ví dụ: luận án → chương tổng quan, chương phương pháp, phần kết luận).

## Bước 2 — Thu thập corpus

Yêu cầu tối thiểu:
- **30–40 văn bản riêng biệt**, đọc toàn văn hoặc gần toàn văn (ít nhất phần mở, thân, kết).
- **Chỉ lấy văn bản công bố trước năm 2023** (trước khi văn bản do AI sinh ra phổ biến). Kiểm tra năm công bố cho từng văn bản; loại bỏ nếu không xác định được năm.
- Đa dạng nguồn: nhiều cơ quan/tác giả/tạp chí khác nhau, không quá 4 văn bản từ cùng một tác giả hoặc cơ quan.
- Ưu tiên nguồn chính thống: trang tạp chí, cổng thông tin cơ quan nhà nước, thuvienphapluat.vn, thư viện số của trường, nhà xuất bản.

Nếu chạy bằng agent, có thể giao nguyên prompt sau (thay phần trong ngoặc nhọn):

```
You are a corpus linguist building a style guide for Vietnamese writing.
Domain: {mô tả loại văn bản}.
HARD REQUIREMENT: read in FULL at least 35 distinct documents published BEFORE 2023.
Use WebSearch + WebFetch. Sources: {danh sách nguồn gợi ý}. Discard 2023+.
Save partial progress early. Analyze LANGUAGE ONLY:
 1. Macro structure and exact headings  2. Opening formulas  3. Authorial voice
 4. Signature phrases/connectors with frequency tiers  5. Citation/number/date conventions
 6. Sentence & paragraph length  7. Closing formulas  8. What looks un-natural/AI-like here.
Output: (A) source list, (B) analysis, (C) 60+ verbatim excerpts grouped by function.
Write to references/corpus/{slug}-corpus.md
```

## Bước 3 — Đúc kết thành file genre

Tạo `references/genres/<slug>.md` theo đúng khung trong `references/genre-template.md`. Mỗi quy tắc nên kèm ít nhất một ví dụ nguyên văn từ corpus. Danh sách nguồn đầy đủ lưu ở `references/corpus/<slug>-corpus.md`.

## Bước 4 — Đăng ký vào SKILL.md

Thêm một dòng vào bảng "Các loại văn bản" trong `SKILL.md` (tên, file, dấu hiệu nhận biết yêu cầu). Nếu loại mới gần với một loại đã có (ví dụ "báo cáo thẩm tra" gần "tờ trình"), ghi chú điểm khác biệt ở cả hai file.

## Bước 5 — Kiểm tra

Viết thử một đoạn 300–400 chữ theo genre mới, sau đó soát theo `references/anti-ai-patterns.md` và phần "Dấu hiệu thiếu tự nhiên" của file genre. Nếu đoạn thử vẫn "nghe như dịch", bổ sung quy tắc còn thiếu.
