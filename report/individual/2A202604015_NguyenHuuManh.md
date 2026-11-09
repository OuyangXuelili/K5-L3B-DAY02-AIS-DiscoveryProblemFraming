# Báo cáo cá nhân — 2A202604015_NguyenHuuManh

> Bản lưu sau lab. Họ tên, MSSV và nhóm đã được đối chiếu. Các vấn đề và sơ đồ ở mục 2–3 ghi lại nội dung chuẩn bị. Hồ sơ chưa kèm dữ liệu trải nghiệm do thành viên xác nhận.

## 1. Thông tin học viên

- Họ tên: Nguyễn Hữu Mạnh
- MSSV: 2A202604015
- Nhóm: AIS
- Link repo nhóm: (https://github.com/OuyangXuelili/K5-L3B-DAY02-AIS-DiscoveryProblemFraming.git).
- Vai trò dự kiến: Tìm cách làm có sẵn và tổng hợp CP6.

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu cần ghi từ một lần thật | Ví dụ giả lập |
|---|---|---|---|---|
| 1 | Tốn thời gian | Khi thấy một công cụ có tính năng phù hợp trên trang hướng dẫn, tôi muốn biết nhóm có quyền dùng tính năng đó hay không, để tránh chọn cách làm mà nhóm không thực hiện được. | Thành viên tìm công cụ cho nhóm | Tính năng cụ thể từng phải kiểm, quyền tài khoản, số nguồn mở và số phút xác minh. | Xác minh một tính năng qua 2 nguồn mất 19 phút, trong đó đối chiếu quyền mất 10 phút. |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi đọc một nhận định về công cụ nhưng chưa rõ căn cứ, tôi muốn tìm đoạn tài liệu gốc chứng minh đúng nội dung, để có thể giữ, sửa hoặc bỏ nhận định đó. | Người kiểm tra nguồn trước khi chốt báo cáo | Một claim cụ thể từng rà, số link đã mở, số phút và phần phải sửa. | Kiểm một claim mất 17 phút và phải thu hẹp một cụm từ vì nguồn chỉ nói tới một loại tài khoản. |
| 3 | Pain từ người khác | Khi mỗi người trình bày một phương án với thước đo khác nhau, tôi muốn đưa các phương án về cùng tiêu chí và cùng phạm vi, để cả nhóm thấy được đánh đổi trước khi chốt. | Người tổng hợp lựa chọn và thành viên phải chọn | Hai phương án từng so, tiêu chí ban đầu, số lượt phải hỏi lại hoặc số phút chuẩn hóa. | So hai phương án mất 17 phút và 2 lượt hỏi để dùng cùng phạm vi. |
| 4 | Lặp lại | Khi mở báo cáo và thấy sơ đồ vừa sửa không hiển thị, tôi muốn xác định vị trí cú pháp sai hoặc phần chưa được hỗ trợ, để có thể sửa đúng chỗ và chia sẻ lại. | Thành viên viết báo cáo có sơ đồ | Lần sửa thật, số lần mở preview hoặc sửa thử, thời gian đến khi hiển thị. | Sửa một sơ đồ mất 11 phút qua 3 lượt xem trước. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi thấy hai phiên bản báo cáo có ngưỡng đo khác nhau, tôi muốn biết dữ liệu hay phản biện nào dẫn đến thay đổi, để dùng đúng ngưỡng trong phần quyết định. | Thành viên rà lại tiêu chí thành công | Một trường từng đổi, hai bản, số phút truy lý do và nguồn chứng minh. | Tra lý do đổi ngưỡng giữa 2 bản mất 13 phút, chỉ một bản có ghi nguồn. |

Trong lượt soạn minh họa, ưu tiên các ý có actor, đầu ra và bước nghẽn quan sát được. 

## 3. Top 3 Problem Cards và quy trình nháp (CP2)

Các sơ đồ ghi lại quy trình đề xuất để kiểm. Hồ sơ chưa có số đo hoặc ước lượng có nguồn cho các bước.

| Rank | Problem | Vì sao chọn | Điều cần chưa chắc |
|---|---|---|---|
| 1 | Xác định một tính năng dùng được với tài khoản nhóm | Đầu ra có thể kiểm lại qua quyền hoặc tài liệu chính thức. | Vướng ở việc đọc tài liệu hay ở việc chưa biết nhóm có tài khoản gì? |
| 2 | Truy lại nguồn của một claim trong báo cáo | Có thể so sánh claim trước và sau khi kiểm. | Một link mở được có thật sự đủ chứng minh chính xác claim đang viết không? |
| 3 | So sánh hai cách làm theo cùng tiêu chí | Đo được công sức chuẩn hóa và chất lượng so sánh. | Có thể đối chiếu công bằng hai phương án trên cùng đầu vào hay cần tách các trường hợp sử dụng? |

Các thời lượng và mục tiêu bổ sung là giả lập. Dùng số đo từ một lượt thật để xác lập baseline.

### Card 1 — Xác định một tính năng dùng được với tài khoản nhóm

| Trường | Nội dung  |
|---|---|
| Job Story | Khi thấy một công cụ có tính năng phù hợp trên trang hướng dẫn, tôi muốn biết nhóm có quyền dùng tính năng đó hay không, để tránh chọn cách làm mà nhóm không thực hiện được. |
| Actor | Thành viên tìm công cụ cho nhóm. |
| Bối cảnh | Tính năng nhìn có vẻ phù hợp, còn điều kiện tài khoản hoặc quyền nhóm chưa rõ. |
| Quy trình hiện tại | Xem sơ đồ nháp bên dưới. |
| Bottleneck | Bước 3. Đối chiếu điều kiện tài khoản và quyền nhóm. Chưa có số đo và căn cứ xác nhận. |
| Impact | Có thể phải đổi công cụ hoặc làm lại quy trình đã đề xuất. Ghi trường hợp cụ thể. |
| Success metric | Số phút xác minh một tính năng và số phương án phải đổi vì thiếu quyền. Chưa có baseline và mục tiêu đã xác nhận. |
| Baseline → mục tiêu minh họa | 19 → tối đa 10 phút xác minh mỗi tính năng. Kết luận ghi cả nguồn điều kiện và kết quả kiểm quyền tài khoản. |
| Phương án không dùng AI | Dùng một bảng có cột tính năng, điều kiện, quyền hiện có và nguồn xác minh. |
| Giả thuyết về AI | AI có thể gợi ý từ khóa để tìm hướng dẫn. Quyền được xác minh trên tài khoản thực tế. |
| Cảm nhận nhanh | No AI với bảng tính năng, điều kiện và nguồn. |
| Giả thuyết can thiệp | No AI nếu chỉ kiểm vài lựa chọn với tài liệu gốc. |

```text
1. Ghi tính năng bắt buộc cho quy trình [2 phút minh họa]
   ↓
2. Mở tài liệu chính thức [4 phút minh họa]
   ↓
3. Đối chiếu điều kiện tài khoản và quyền nhóm [10 phút minh họa, bước nghẽn]
   ↓
4. Ghi kết luận và nguồn [3 phút minh họa]
```

**Tổng thời gian minh họa** — 19 phút.

### Card 2 — Truy lại nguồn của một claim trong báo cáo

| Trường | Nội dung |
|---|---|
| Job Story | Khi đọc một nhận định về công cụ nhưng chưa rõ căn cứ, tôi muốn tìm đoạn tài liệu gốc chứng minh đúng nội dung, để có thể giữ, sửa hoặc bỏ nhận định đó. |
| Actor | Người kiểm tra nguồn trước khi chốt báo cáo. |
| Bối cảnh | Một claim được ghi vào báo cáo trong lúc research, có link nhưng cần đối chiếu đoạn hỗ trợ. |
| Quy trình hiện tại | Xem sơ đồ nháp bên dưới. |
| Bottleneck | Bước 3. So nội dung nguồn với phạm vi claim. Chưa có số đo và căn cứ xác nhận. |
| Impact | Có thể mất thời gian dò lại hoặc để lại claim vượt quá phạm vi nguồn. Ghi số claim đã sửa và thời gian. |
| Success metric | Số phút kiểm một nhận định và số nhận định quan trọng thiếu nguồn hỗ trợ. Chưa có baseline và mục tiêu đã xác nhận. |
| Baseline → mục tiêu minh họa | 17 → tối đa 9 phút mỗi claim. Mọi claim quan trọng giữ lại đều có đoạn nguồn hỗ trợ. |
| Phương án không dùng AI | Ghi tên trang, phần liên quan và ngày kiểm ngay khi đưa claim vào bảng. |
| Giả thuyết về AI | AI có thể gợi ý trang liên quan. Người rà đọc đoạn gốc rồi quyết định giữ, sửa hay bỏ. |
| Cảm nhận nhanh | No AI cho các claim quan trọng trong phạm vi lab. |
| Giả thuyết can thiệp | No AI. Người phụ trách vẫn mở nguồn và tự xác định nội dung được chứng minh. |

```text
1. Khoanh claim cần xác minh [2 phút minh họa]
   ↓
2. Mở nguồn đang được dẫn [3 phút minh họa]
   ↓
3. So nội dung nguồn với phạm vi claim [9 phút minh họa, bước nghẽn]
   ↓
4. Sửa claim hoặc đổi nguồn [3 phút minh họa]
```

**Tổng thời gian minh họa** — 17 phút.

### Card 3 — So sánh hai cách làm theo cùng tiêu chí

| Trường | Nội dung |
|---|---|
| Job Story | Khi mỗi người trình bày một phương án với thước đo khác nhau, tôi muốn đưa các phương án về cùng tiêu chí và cùng phạm vi, để cả nhóm thấy được đánh đổi trước khi chốt. |
| Actor | Người tổng hợp lựa chọn và thành viên phải chọn. |
| Bối cảnh | Hai cách xử lý cùng một vấn đề nhưng mô tả thành công bằng tiêu chí khác nhau. |
| Quy trình hiện tại | Xem sơ đồ nháp bên dưới. |
| Bottleneck | Bước 3. Đưa cách đo về cùng đơn vị và ngữ cảnh. Chưa có số đo và căn cứ xác nhận. |
| Impact | Có thể chọn dựa trên thước đo thiếu tương đương. Ghi ví dụ nhóm phải sửa cách so sánh hoặc đổi quyết định. |
| Success metric | Số lượt làm rõ trước khi hai phương án dùng chung một tiêu chí đo. Chưa có baseline và mục tiêu đã xác nhận. |
| Baseline → mục tiêu minh họa | 2 → tối đa 1 lượt hỏi lại. Hai phương án dùng cùng đơn vị, phạm vi và điều kiện đạt. |
| Phương án không dùng AI | Chốt một bảng tiêu chí trước khi tìm và trình bày phương án. |
| Giả thuyết về AI | AI có thể chỉ ra khác biệt cách diễn đạt. Nhóm tự xác định điều kiện và tiêu chí dùng chung. |
| Cảm nhận nhanh | No AI với khung so sánh đã chốt. |
| Giả thuyết can thiệp | No AI nếu số phương án nhỏ và người dùng thống nhất được tiêu chí. |

```text
1. Liệt kê hai phương án [2 phút minh họa]
   ↓
2. Chốt phạm vi đầu vào chung [4 phút minh họa]
   ↓
3. Đưa cách đo về cùng đơn vị và ngữ cảnh [8 phút minh họa, bước nghẽn]
   ↓
4. Ghi đánh đổi và chọn [3 phút minh họa]
```

**Tổng thời gian minh họa** — 17 phút.

### Nội dung chuẩn bị pitch

Card 1 là đề xuất ưu tiên trong bản chuẩn bị. Câu hỏi đã soạn — Vướng ở việc đọc tài liệu hay ở việc chưa biết nhóm có tài khoản gì? Hồ sơ chưa có ghi nhận buổi pitch hoặc chỉnh sửa sau phản biện của thành viên.

**Phản biện AI trong lúc chuẩn bị** — Tách việc sản phẩm có tính năng khỏi việc tài khoản nhóm được quyền dùng và quy trình có phù hợp.

## 4. Tôi đã tham gia phần nào?

| Vai trò dự kiến | Phần việc để chuẩn bị | Tham chiếu |
|---|---|---|
| Research và CP6 | Đối chiếu ba nguồn sản phẩm, so bốn mức can thiệp, đề xuất thử bảng No AI nếu CP4 xác nhận nhu cầu. | Mục 3.3 và 6–8 trong [báo cáo nhóm](../team/group_report.md) |

**Câu hỏi để luyện pitch** — Nếu mọi góp ý đã tập trung trong tài liệu thì bảng riêng còn giải quyết phần nào?

Sau buổi pitch, hãy phản biện nhận được và thay đổi thực tế.

## 5. Dùng AI

| Mục | AI hỗ trợ trong lần cập nhật | Cách rà trước khi dùng |
|---|---|---|
| CP1 | Bổ sung ví dụ định lượng theo từng Job Story. | Thay ví dụ bằng quan sát và số liệu của thành viên. |
| CP2 | Gợi ý thời lượng, chỉ số thử và câu hỏi phản biện. | Tách việc sản phẩm có tính năng khỏi việc tài khoản nhóm được quyền dùng và quy trình có phù hợp. |
| CP7 | Soạn reflection mẫu cho một kịch bản giả lập. | Tự viết lại theo sự việc và quyết định mình thực sự tham gia. |

## 6. Reflection (CP7)

> **Mẫu do AI soạn cho kịch bản giả lập.** 

**6.1. Điều rút ra từ các card**

Trong kịch bản research, tài liệu mô tả chức năng giao việc có thể đúng nhưng vẫn chưa xác nhận AIS dùng được. Cần kiểm loại tài khoản, quyền trên tài liệu và nơi người góp ý thực tế gửi yêu cầu.

**6.2. Lúc dễ chọn giải pháp quá sớm**

Tự động hóa dễ trở thành đích đến trước khi đo bước nghẽn. Với một bản nháp và hai nguồn đã biết, thử quy ước thủ công có thể cho thấy việc giữ nguồn và trạng thái đã giải quyết được bao nhiêu công sức.

**6.3. Phản biện làm đổi cách làm**

Google Docs có thể xử lý hội thoại tại chỗ. Nếu mọi góp ý đã vào cùng tài liệu, trạng thái sẵn có có thể đủ. Điều đó làm thay đổi phạm vi thử bảng sang các vòng sửa có việc quan trọng nằm ngoài luồng.

**6.4. Điều CP4 cần kiểm**

CP4 cần xác nhận tần suất dùng hai kênh và hậu quả của việc bỏ sót. Tài liệu công cụ giúp hiểu thao tác có thể làm, còn các ca gần nhất mới giúp đánh giá thao tác đó có cần thiết.

**6.5. Chỗ khó của Problem Statement**

Khó nhất trong v1 là cân bằng thời gian với chất lượng. Nếu một lượt nhanh hơn nhưng sót việc liên quan tiêu chí chấm, lượt đó không đạt. Vì vậy phép đo phải gồm cả thời gian lập bảng và kiểm danh sách.

**6.6. Việc sẽ đổi khi làm lại**

Nếu làm lại, nên chọn hai tập có độ khó tương đương, đổi thứ tự giữa các người thử và nhờ người thứ hai đối chiếu nguồn. Sau ba lượt so sánh, xem trung vị và số lỗi trước khi đổi quyết định.

**6.7. Giải thích mạch bài toán**

Trong một vòng sửa, người tổng hợp cần biết góp ý nào còn mở khi nhận xét đến từ chat và bình luận tài liệu. Quy trình bắt đầu khi xác định bản nháp và kết thúc khi chốt danh sách. Bước nghẽn dự kiến là đối chiếu ý mới, ý trùng và ý đã xử lý. Mục tiêu thử là giảm ít nhất 25% trung vị thời gian với 0 góp ý quan trọng bị sót. Người phụ trách xác nhận nguồn và chốt ý mâu thuẫn. Phương án dự kiến là bảng thủ công No AI. Quyết định là Not Yet cho tới khi có bằng chứng CP4.

## 7. Tài liệu tham khảo

- [Worksheet](../../docs/01-worksheet.md)
- [Rubric](../../RUBRIC.md)
