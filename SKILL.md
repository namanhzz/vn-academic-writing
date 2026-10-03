---
name: vn-academic-writing
description: Khóa văn phong tiếng Việt cho văn bản khoa học và chính sách, rút từ corpus văn bản thật trước 2023. Dùng khi viết, sửa hoặc soát văn bản tiếng Việt thuộc các loại - bài báo khoa học, tham luận hội thảo; sách chuyên khảo kinh tế; tờ trình, báo cáo, đề án, báo cáo thẩm tra, công văn; thuyết minh đề tài NCKH, đề cương, đề xuất nghiên cứu hoặc tư vấn. Cũng dùng khi người dùng muốn văn bản tiếng Việt bớt "giọng AI", "giọng dịch", hoặc muốn bổ sung một loại văn bản mới vào skill.
---

# Văn phong khoa học và chính sách tiếng Việt

Skill này chỉ lo **ngôn ngữ và văn phong**, không lo nội dung chuyên môn. Mọi quy tắc trong skill được rút ra từ việc đọc toàn văn hàng trăm văn bản thật công bố trước năm 2023, tức trước khi văn bản do AI sinh ra trở nên phổ biến.

## Các loại văn bản

| Loại | File hướng dẫn | Nhận biết yêu cầu |
|---|---|---|
| Bài báo khoa học, tham luận hội thảo | `references/genres/bai-bao-khoa-hoc.md` | bài báo, bài tạp chí, tham luận, kỷ yếu, tóm tắt (abstract), bài nghiên cứu định lượng/định tính |
| Sách chuyên khảo kinh tế | `references/genres/sach-chuyen-khao.md` | sách, chuyên khảo, chương sách, lời nói đầu, lời giới thiệu, bài phân tích dài của chuyên gia |
| Văn bản hành chính – chính sách | `references/genres/van-ban-hanh-chinh.md` | tờ trình, báo cáo (tổng kết, sơ kết, giám sát, đánh giá tác động), đề án, báo cáo thẩm tra, công văn, thông báo kết luận, nghị quyết, quyết định |
| Thuyết minh đề tài, đề xuất nghiên cứu/tư vấn | `references/genres/de-xuat-de-tai.md` | thuyết minh đề tài, đề cương, phiếu đề xuất nhiệm vụ, đề xuất tư vấn, tính cấp thiết, tổng quan, mục tiêu, phần Mở đầu luận án |

Nếu yêu cầu không khớp loại nào, dùng loại gần nhất và nói rõ cho người dùng. Nếu người dùng muốn thêm loại mới, làm theo `references/add-new-genre.md`.

## Quy trình

1. **Xác định loại văn bản** (và tiểu loại, cấp ban hành, người nhận, mẫu bắt buộc nếu có). Nếu thiếu thông tin quyết định văn phong — ví dụ tờ trình gửi Quốc hội hay gửi Sở, thuyết minh theo mẫu cấp quốc gia hay cấp trường — hỏi một câu ngắn hoặc chọn mặc định hợp lý và ghi chú.
2. **Đọc file genre tương ứng** trong `references/genres/`. Cần câu mẫu nguyên văn hoặc bảng tần suất thì tra thêm `references/corpus/<genre>-corpus.md` (file lớn, chỉ đọc phần cần).
3. **Viết theo khung, công thức và tầng từ vựng** của file genre. Nội dung chuyên môn lấy từ người dùng; không bịa số liệu, số hiệu văn bản, tên tác giả hay trích dẫn. Chỗ cần số liệu hoặc số hiệu mà người dùng chưa cung cấp thì để chỗ trống dạng `[số liệu]`, `[Nghị quyết số …]`.
4. **Soát lại** theo `references/anti-ai-patterns.md` và mục "Dấu hiệu thiếu tự nhiên" của file genre trước khi trả.

Khi sửa văn bản có sẵn: giữ nội dung và lập luận của người viết, chỉ đổi ngôn ngữ cho đúng thể loại. Nếu người dùng yêu cầu, liệt kê ngắn các thay đổi chính.

## Quy tắc chung cho cả bốn loại

Những quy tắc này đúng với mọi thể loại trong skill. Quy tắc riêng của từng loại (có thể ghi đè) nằm trong file genre.

1. **Neo lập luận vào căn cứ cụ thể.** Văn bản thật dẫn số hiệu, ngày, cơ quan ban hành ("Nghị quyết số 50-NQ/TW ngày 20/8/2019 của Bộ Chính trị") hoặc tác giả, năm ("Nguyễn Văn A (2018)"). Không mở bài bằng câu khái quát rỗng kiểu "Trong bối cảnh toàn cầu hóa hiện nay, …" mà không có căn cứ đi kèm.
2. **Khung đánh giá kiểu Việt:** kết quả (có rào đón) → "Tuy nhiên," → hạn chế (phủ định mềm: "chưa …", "còn …", "chưa thực sự …") → nguyên nhân (khách quan trước, chủ quan sau) → giải pháp hoặc kiến nghị. Khung này có trong cả bài báo, sách, tờ trình, thuyết minh, với độ đậm nhạt khác nhau.
3. **Cặp đôi và chuỗi đồng nghĩa** là nhịp tự nhiên của tiếng Việt khoa học, không phải lỗi thừa từ: lý luận và thực tiễn; trong và ngoài nước; nói chung … nói riêng; khó khăn, vướng mắc; tồn tại, hạn chế; phân tích, đánh giá; hiệu lực, hiệu quả.
4. **Danh hóa và từ Hán Việt** là trục câu: việc + V, công tác + N, tính + Adj, -hóa (hệ thống hóa, thể chế hóa, cụ thể hóa). Không thay bằng khẩu ngữ hay từ báo chí ("cực kỳ", "siêu", "bùng nổ").
5. **Câu dài vừa phải đến dài**, nối bằng dấu phẩy, chấm phẩy và "nhằm / để / từ đó / trên cơ sở đó". Không viết chuỗi câu ngắn đều nhau kiểu tiếng Anh.
6. **Lặp nguyên thuật ngữ và tên chủ thể** thay vì đổi từ đồng nghĩa cho "văn hay".
7. **Liệt kê kiểu Việt:** "Thứ nhất, … Thứ hai, …", "Một là, … Hai là, …", "(i), (ii), (iii)"; đánh số I. → 1. → a) → - → + (bảng chữ cái tiếng Việt: a b c d đ e g h i k, không có f, j). Không dùng bullet đồ họa (•, ✓, →).
8. **Số và ngày kiểu Việt:** dấu chấm hàng nghìn, dấu phẩy thập phân ("1.212.180 tỷ đồng", "6,7%"); "%" viết liền; "nghìn" không "ngàn" trong văn bản hành chính; "tỷ" không "tỉ"; ngày "ngày 05 tháng 3 năm 2020" hoặc "05/3/2020". Không dùng "VND", "6.7%", "2020-03-05".
9. **Đề mục:** IN HOA TOÀN BỘ (cấp cao) hoặc chỉ viết hoa chữ đầu. Không viết hoa mỗi từ kiểu tiêu đề tiếng Anh.
10. **Không dùng dấu gạch ngang dài (—) để chen ý**, câu hỏi tu từ, câu cảm thán, giọng quảng bá hay truyền cảm hứng ("đột phá ngoạn mục", "hành trình", "kỷ nguyên mới mở ra", "chìa khóa vàng").
11. **Ngôi tự xưng đúng thể loại:** văn bản hành chính không dùng "chúng tôi" (cơ quan tự xưng bằng tên); bài báo dùng "tác giả", "nhóm tác giả", "bài viết", "nghiên cứu này"; luận án dùng "NCS", "tác giả"; đề tài dùng "chúng tôi", "nhóm nghiên cứu", "Đề tài"; sách chuyên khảo một tác giả dùng "tác giả" (ngôi 3) và "người viết", còn sách và báo cáo của viện dùng "chúng tôi", "nhóm nghiên cứu"; "tôi" chỉ dùng trong lời tựa. Chi tiết trong từng file genre.
12. **Từ nối tùy thể loại.** "Tuy nhiên", "Bên cạnh đó", "Nhìn chung", "nhằm" là từ nối chính của văn bản hành chính, bài báo và báo cáo của viện, nhưng lại hiếm trong chuyên khảo một tác giả (ở đó dùng "Nhưng", "Song", "Thế nhưng", "Thật ra"). Xem bảng tần suất trong file genre trước khi chọn.
13. **Dùng "nước ta", "ta", "Đảng và Nhà nước ta"** đúng chỗ trong văn bản chính luận và chính sách. Đây là dấu hiệu văn viết bằng tiếng Việt từ đầu, gần như không có trong văn dịch.

## Cấu trúc skill

```
SKILL.md                         ← file này: định tuyến + quy tắc chung
references/
  genres/                        ← hướng dẫn văn phong từng loại (đọc khi viết)
  corpus/                        ← nguồn, bảng tần suất, kho câu trích nguyên văn (tra khi cần)
  anti-ai-patterns.md            ← danh sách soát "giọng AI / giọng dịch" chung
  genre-template.md              ← khung cho file genre mới
  add-new-genre.md               ← quy trình nghiên cứu và thêm loại văn bản mới
```
