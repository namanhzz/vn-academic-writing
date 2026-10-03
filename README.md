# vn-academic-writing

Skill cho Claude, dùng để khóa văn phong tiếng Việt khi viết văn bản khoa học và chính sách. Skill chỉ lo ngôn ngữ và văn phong, không lo nội dung chuyên môn.

Mọi quy tắc được rút ra từ việc đọc toàn văn văn bản thật **công bố trước năm 2023**, tức trước khi văn bản do AI sinh ra trở nên phổ biến:

| Loại văn bản | Corpus |
|---|---|
| Bài báo khoa học, tham luận hội thảo | 37 bài (27 bài tạp chí, 10 tham luận), 2016–2022 |
| Sách chuyên khảo kinh tế, sách của viện, báo cáo thường niên | 42 nguồn (30 đọc toàn văn hoặc phần lớn), 2007–2022 |
| Tờ trình, báo cáo, đề án, thẩm tra, công văn | 68 văn bản, 2010–2022 |
| Thuyết minh đề tài NCKH, đề xuất nghiên cứu/tư vấn | 39 tài liệu, 2010–2022 |

## Cài đặt

Claude Code (cá nhân):

```bash
git clone https://github.com/namanhzz/vn-academic-writing.git ~/.claude/skills/vn-academic-writing
```

Hoặc trong một project: clone vào `.claude/skills/vn-academic-writing`.

Claude.ai / Claude Desktop: nén thư mục thành `.zip` và tải lên ở phần Skills.

## Cách dùng

Yêu cầu Claude viết hoặc sửa văn bản thuộc một trong bốn loại trên, ví dụ:

- "Viết phần tính cấp thiết cho thuyết minh đề tài cấp Bộ về tín dụng xanh"
- "Sửa tóm tắt bài báo này cho đúng văn phong tạp chí Việt"
- "Soạn tờ trình của Sở gửi UBND tỉnh về đề án …"
- "Viết lời nói đầu cho cuốn sách chuyên khảo về …"
- "Đoạn này đọc có giống AI viết không, sửa lại"

Skill sẽ tự chọn file hướng dẫn phù hợp trong `references/genres/`.

## Thêm loại văn bản mới

Xem `references/add-new-genre.md`. Tóm tắt: thu thập và đọc 30–40 văn bản thật trước 2023, phân tích ngôn ngữ, viết file `references/genres/<loại>.md` theo `references/genre-template.md`, lưu nguồn vào `references/corpus/`, rồi thêm một dòng vào bảng trong `SKILL.md`. Có thể chỉ cần nói với Claude: "bổ sung loại văn bản X vào skill vn-academic-writing".

## Cấu trúc

```
SKILL.md                    định tuyến + quy tắc chung
references/genres/          hướng dẫn văn phong từng loại
references/corpus/          danh sách nguồn, bảng tần suất, câu trích nguyên văn
references/anti-ai-patterns.md
references/genre-template.md
references/add-new-genre.md
```

## Lưu ý

Các câu trích trong `references/corpus/` được dùng làm bằng chứng ngôn ngữ cho nghiên cứu văn phong, kèm nguồn đầy đủ. Đoạn mẫu trong `references/genres/` là tự soạn theo quy tắc, số liệu và trích dẫn trong đó chỉ để minh họa.
