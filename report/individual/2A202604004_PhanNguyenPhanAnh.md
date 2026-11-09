# Báo cáo cá nhân — 2A202604004_PhanNguyenPhanAnh

## 1. Thông tin học viên

- Họ tên — Phan Nguyễn Phan Anh
- MSSV — 2A202604004
- Nhóm — AIS
- Link repo nhóm — https://github.com/OuyangXuelili/K5-L3B-DAY02-AIS-DiscoveryProblemFraming
- Vai trò dự kiến — Kiểm chứng và tổng hợp bằng chứng CP4.

## 2. Scan problem (CP1)

| # | Lăng kính | Job Story gợi ý | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi phải viết nhận định từ nhiều cuộc trao đổi, tôi muốn lần lại đúng ghi chú của từng nhận định, để giải thích được vì sao tôi đưa ra kết luận đó. | Người tổng hợp ghi chú hoặc phản hồi | Một nhận định từng phải dò lại, số ghi chú đã mở, số phút đối chiếu và kết quả. |
| 2 | Tốn thời gian | Khi cần dùng ảnh trao đổi làm minh chứng trong repo, tôi muốn giữ được chi tiết liên quan sau khi che thông tin riêng, để người đọc kiểm tra được bằng chứng. | Người chuẩn bị ảnh cho báo cáo | Số ảnh và số lần phải xem hoặc xử lý lại ở một lần thật. Chỉ dùng ảnh có quyền chia sẻ. |
| 3 | Pain từ người khác | Khi một người chỉ mô tả việc họ làm bằng các từ như khó hoặc lâu, tôi muốn xin được một lần đã xảy ra với đủ ngữ cảnh, để xác định chính xác bước họ gặp khó khăn. | Người ghi nhận phản hồi về một quy trình | Số lượt hỏi thêm để lấy được một ví dụ, thời lượng hoặc mục còn thiếu sau buổi hỏi. |
| 4 | Lặp lại | Khi tổng hợp câu trả lời từ nhiều lượt thu thập, tôi muốn xác định phản hồi nào đã được ghi, để đếm đúng số mẫu dùng trong báo cáo. | Người xử lý phản hồi của một nhóm nhỏ | Số dòng được rà, cách phát hiện dòng trùng, số mẫu bị ảnh hưởng trong một lần cụ thể. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi đặt các mốc thời gian từ nhiều nguồn vào cùng một bảng, tôi muốn biết số nào đã bấm giờ và số nào do người khác nhớ lại, để diễn giải kết quả theo đúng mức chắc chắn. | Người đối chiếu số liệu trong báo cáo | Một bảng từng có số liệu thiếu nhãn, số dòng phải kiểm lại và nguồn đối chiếu. |


## 3. Top 3 Problem Cards và quy trình nháp (CP2)

Các sơ đồ ghi lại quy trình đề xuất để kiểm. Hồ sơ chưa có số đo hoặc ước lượng có nguồn cho các bước.

| Hạng nháp | Vấn đề | Vì sao đáng xem xét | Điều cần xác nhận |
|---|---|---|---|
| 1 | Gắn nhận định tổng hợp với đúng ghi chú nguồn | Có đầu vào, đầu ra và lỗi quan sát được trong một lượt rà. | Bước nghẽn là tìm ghi chú hay diễn giải nội dung của ghi chú? |
| 2 | Ẩn thông tin nhận diện trong ảnh minh chứng | Có thể đo thời gian với một ảnh đã được phép xử lý. | Các ảnh cần thiết có thật sự được phép đưa vào báo cáo không? |
| 3 | Làm rõ một câu trả lời quá chung | Phân biệt được ý kiến chung với một sự kiện cụ thể. | Thời gian hỏi thêm có đổi lại dữ liệu cụ thể hơn hay chỉ kéo dài buổi hỏi? |

### Card 1 — Gắn nhận định tổng hợp với đúng ghi chú nguồn

| Trường | Nội dung cần đối chiếu |
|---|---|
| Job Story | Khi phải viết nhận định từ nhiều cuộc trao đổi, tôi muốn lần lại đúng ghi chú của từng nhận định, để giải thích được vì sao tôi đưa ra kết luận đó. |
| Actor | Người tổng hợp ghi chú hoặc phản hồi. |
| Bối cảnh | Một đoạn tổng hợp dùng dữ liệu từ nhiều ghi chú ngắn. |
| Quy trình hiện tại | Xem sơ đồ nháp bên dưới. |
| Bottleneck | Bước 3. Đối chiếu nhận định với đúng câu hoặc mốc thời gian. Chưa có số đo và căn cứ xác nhận. |
| Impact | Một nhận định có thể bị ghi rộng hơn những gì nguồn nói. Ghi số nhận định phải sửa hoặc số phút truy lại. |
| Success metric | Số phút truy nguồn mỗi nhận định và số nhận định quan trọng thiếu nguồn. Chưa có baseline và mục tiêu đã xác nhận. |
| Baseline → mục tiêu minh họa | 18 → tối đa 10 phút mỗi nhận định. Các nhận định quan trọng có mã dẫn tới đúng câu hoặc mốc nguồn. |
| Phương án không dùng AI | Gắn mã ẩn danh ngay khi ghi chú và trỏ mã đó từ bảng tổng hợp. |
| Giả thuyết về AI | AI có thể gợi ý ghi chú liên quan. Người tổng hợp kiểm đoạn gốc và phạm vi nhận định. |
| Cảm nhận nhanh | No AI với mã nguồn gắn ngay khi ghi. |
| Giả thuyết can thiệp | No AI nếu mã nguồn rõ và số ghi chú nhỏ. |

```text
1. Đọc nhận định dự kiến [2 phút minh họa]
   ↓
2. Tìm các ghi chú có liên quan [4 phút minh họa]
   ↓
3. Đối chiếu nhận định với đúng câu hoặc mốc thời gian [9 phút minh họa, bước nghẽn]
   ↓
4. Gắn mã nguồn và sửa nhận định [3 phút minh họa]
```

**Tổng thời gian minh họa** — 18 phút.

### Card 2 — Ẩn thông tin nhận diện trong ảnh minh chứng

| Trường | Nội dung cần đối chiếu |
|---|---|
| Job Story | Khi cần dùng ảnh trao đổi làm minh chứng trong repo, tôi muốn giữ được chi tiết liên quan sau khi che thông tin riêng, để người đọc kiểm tra được bằng chứng. |
| Actor | Người chuẩn bị ảnh cho báo cáo. |
| Bối cảnh | Một nhóm cần chia sẻ ảnh đã được phép dùng trong báo cáo. |
| Quy trình hiện tại | Xem sơ đồ nháp bên dưới. |
| Bottleneck | Bước 2. Rà các vùng có tên hoặc dữ liệu riêng. Chưa có số đo và căn cứ xác nhận. |
| Impact | Có thể phải thay ảnh nhiều lần hoặc ảnh không còn đủ ngữ cảnh. Ghi số lượt và thời gian thực. |
| Success metric | Số phút chuẩn bị một ảnh. Điều kiện an toàn đề xuất là 0 chi tiết riêng bị lộ trong bản được phép chia sẻ. |
| Baseline → mục tiêu minh họa | 16 → tối đa 10 phút mỗi ảnh. Người thứ hai kiểm bản xuất và ghi nhận 0 chi tiết riêng bị lộ. |
| Phương án không dùng AI | Dùng danh sách vị trí cần rà và người thứ hai kiểm ảnh sau khi xuất. |
| Giả thuyết về AI | AI có thể gợi ý vùng chứa tên nhưng người chuẩn bị và người rà duyệt bản xuất. |
| Cảm nhận nhanh | No AI cho ảnh được phép dùng và phạm vi nhỏ. |
| Giả thuyết can thiệp | No AI để giữ toàn bộ thao tác trên bản sao và để con người quyết định phần phải che. |

```text
1. Chọn chi tiết cần giữ [2 phút minh họa]
   ↓
2. Rà các vùng có tên hoặc dữ liệu riêng [7 phút minh họa, bước nghẽn]
   ↓
3. Che chi tiết và xuất bản sao [4 phút minh họa]
   ↓
4. Mở bản sao để rà lại [3 phút minh họa]
```

**Tổng thời gian minh họa** — 16 phút.

### Card 3 — Làm rõ một câu trả lời quá chung

| Trường | Nội dung cần đối chiếu |
|---|---|
| Job Story | Khi một người chỉ mô tả việc họ làm bằng các từ như khó hoặc lâu, tôi muốn xin được một lần đã xảy ra với đủ ngữ cảnh, để xác định chính xác bước họ gặp khó khăn. |
| Actor | Người ghi nhận phản hồi về một quy trình. |
| Bối cảnh | Một cuộc trao đổi ngắn về lần người tham gia gặp khó khăn. |
| Quy trình hiện tại | Xem sơ đồ nháp bên dưới. |
| Bottleneck | Bước 3. Hỏi thêm về bước cụ thể và hệ quả. Chưa có số đo và căn cứ xác nhận. |
| Impact | Có thể tốn thêm lượt hỏi hoặc kết thúc mà chưa có tình huống cụ thể để kiểm chứng. Đếm mục thiếu trong snapshot thật. |
| Success metric | Số lượt hỏi bổ sung để ghi đủ thời điểm, bước làm và hệ quả. Chưa có baseline và mục tiêu đã xác nhận. |
| Baseline → mục tiêu minh họa | 2 → tối đa 1 lượt hỏi bổ sung. Phiếu ghi vẫn phải có thời điểm, bước đã xảy ra và hệ quả. |
| Phương án không dùng AI | Chuẩn bị bộ câu gợi mở về hành vi đã xảy ra và xin kể theo thứ tự bước. |
| Giả thuyết về AI | AI có thể gợi ý câu hỏi để luyện trước. Người phỏng vấn tự hỏi người thật. |
| Cảm nhận nhanh | No AI trong lúc kiểm chứng. |
| Giả thuyết can thiệp | No AI. Người hỏi tự lắng nghe và chọn câu tiếp theo. |

```text
1. Đặt câu hỏi mở về lần gần nhất [2 phút minh họa]
   ↓
2. Nghe câu trả lời ban đầu [3 phút minh họa]
   ↓
3. Hỏi thêm về bước cụ thể và hệ quả [6 phút minh họa, bước nghẽn]
   ↓
4. Ghi lại tình huống và phần còn thiếu [2 phút minh họa]
```

**Tổng thời gian minh họa** — 13 phút.


## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Chuẩn bị pitch Card 1, **Gắn nhận định tổng hợp với đúng ghi chú nguồn**. Câu hỏi mở là bước nào tốn công hơn, tìm ghi chú hay kiểm xem ghi chú có hỗ trợ nhận định. | Đề xuất đo riêng thời gian tìm ghi chú và thời gian đối chiếu để xác định bước nghẽn. |
| Phản biện bài của bạn khác | Câu hỏi dự kiến cho Card C1. Nếu hai góp ý cùng nhắc một đoạn nhưng yêu cầu sửa khác nhau, nhóm sẽ ghi thế nào? | Đề xuất chỉ gộp khi hai ý yêu cầu cùng một thay đổi và giữ cả hai mã nguồn. Ý mâu thuẫn để **Chờ chốt**. |
| Nhận phản biện | Câu hỏi luyện pitch. Có mã ghi chú rồi thì đã đủ để chứng minh nhận định chưa? | Trong Card 1, bổ sung tiêu chí trỏ đúng câu hoặc mốc nguồn và kiểm phạm vi của nhận định. Chưa có phản biện từ buổi pitch được ghi lại. |
| Gom cluster / cây OST | Khi rà các ứng viên, đề xuất tách khó khăn **truy nguồn** khỏi khó khăn **xác định trạng thái**. | Giúp làm rõ hai nhánh của C1 cần kiểm riêng, tìm đủ góp ý và biết việc nào vẫn còn mở. |
| Chọn candidate problem | Đề xuất kiểm C1 trong phạm vi một bản nháp, hai nguồn và một vòng sửa. | Có thể hỏi về một sự việc cụ thể và xác định mốc bắt đầu, kết thúc để bấm giờ. |
| Kiểm chứng / research | Theo phân công CP4, chuẩn bị hỏi 2–3 người ngoài nhóm về vòng sửa gần nhất. Tách thời gian bấm giờ khỏi số nhớ lại và hỏi cả trường hợp bình luận tài liệu đã đủ dùng. | Kế hoạch kiểm chứng nằm ở mục 3.1–3.2 của [báo cáo nhóm](../team/group_report.md). Kết quả phỏng vấn hoặc khảo sát chờ bổ sung. |
| Quy trình nhóm | Đề xuất khi tái hiện một vòng sửa, ghi riêng thời gian đọc bình luận, tìm trong chat, đối chiếu và xác nhận danh sách. | Cách ghi giúp kiểm bước nào tốn công và đo đến lúc chốt danh sách, trước khi bắt đầu sửa nội dung. |
| Problem Statement | Đề xuất dùng một lần sửa cụ thể để kiểm lại người gặp vấn đề, bước nghẽn và hệ quả đã xảy ra. | Nhóm có căn cứ thu hẹp bài toán vào người thực sự phải đối chiếu hai nguồn và chọn chỉ số phù hợp. |
| Mức can thiệp AI | Đề xuất thử bảng **No AI** nếu CP4 xác nhận vấn đề. Người phụ trách đọc nguồn và xác nhận trạng thái từng mục. | Có thể kiểm tác động của việc gom góp ý và ghi trạng thái trước khi cân nhắc tự động hóa. |
| Quyết định | Ghi nhận đề xuất **Not Yet** vì hồ sơ chưa có kết quả CP4. Khi có bằng chứng, dùng mục tiêu giảm ít nhất 25% thời gian trung vị và không sót góp ý quan trọng để đánh giá lượt thử. | Xác định bước tiếp theo là kiểm chứng vấn đề và đo baseline trước khi quyết định có thử bảng hay không. |

---

## 5. Dùng AI

| Mục | AI hỗ trợ trong lần cập nhật | Cách rà trước khi dùng |
|---|---|---|
| CP1 | Bổ sung ví dụ định lượng theo từng Job Story. | Thay ví dụ bằng quan sát và số liệu của thành viên. |
| CP2 | Gợi ý thời lượng, chỉ số thử và câu hỏi phản biện. | Thêm tiêu chí trỏ đúng đoạn nguồn và kiểm phạm vi nhận định thay vì chỉ đếm số ghi chú đã mở. |
| CP7 | Soạn reflection mẫu cho một kịch bản giả lập. | Tự viết lại theo sự việc và quyết định mình thực sự tham gia. |

## 6. Reflection (CP7)

**6.1. Điều rút ra từ các card**

Một kịch bản để tập CP4 là người được hỏi nói tổng hợp rất lâu nhưng chưa kể lần nào. Cần hỏi họ mở nguồn gì, làm theo thứ tự nào và phải làm lại việc gì trước khi gọi một bước là bước nghẽn.

**6.2. Lúc dễ chọn giải pháp quá sớm**

Chuẩn bị sẵn một bảng theo dõi dễ làm câu hỏi nghiêng về giải pháp. Trong ví dụ, câu hỏi nên xoay quanh lần sửa gần nhất và cách người đó biết một góp ý đã được xử lý.

**6.3. Phản biện làm đổi cách làm**

Phản biện trong bản mẫu là trích đúng câu vẫn có thể diễn giải rộng quá. Cách sửa là giữ mã nguồn và mốc thời gian, rồi so phạm vi của kết luận với điều người tham gia thực sự mô tả.

**6.4. Điều CP4 cần kiểm**

Một ca phản bác hữu ích là nhóm tập trung nhận xét trong tài liệu và xử lý nhanh. Khi gặp ca đó, cần ghi lý do cách hiện tại có hiệu quả và thu hẹp bài toán vào nhóm dùng hai nguồn.

**6.5. Chỗ khó của Problem Statement**

Problem Statement cần nói rõ hệ quả quan sát được. Cụm từ dễ bỏ sót vẫn là một giả thuyết cho tới khi có ví dụ hoặc phép đối chiếu cho thấy việc quan trọng đã bị bỏ khỏi danh sách.

**6.6. Việc sẽ đổi khi làm lại**

Nếu làm lại, nên đánh mã nguồn ngay khi ghi chú và phân biệt ba phần trong tổng hợp. Đó là lời kể của người tham gia, số đo quan sát và diễn giải của nhóm. Cách chia này giúp truy lại từng nhận định.

**6.7. Giải thích mạch bài toán**

Trong một vòng sửa, người tổng hợp cần biết góp ý nào còn mở khi nhận xét đến từ chat và bình luận tài liệu. Quy trình bắt đầu khi xác định bản nháp và kết thúc khi chốt danh sách. Bước nghẽn dự kiến là đối chiếu ý mới, ý trùng và ý đã xử lý. Mục tiêu thử là giảm ít nhất 25% trung vị thời gian với 0 góp ý quan trọng bị sót. Người phụ trách xác nhận nguồn và chốt ý mâu thuẫn. Phương án dự kiến là bảng thủ công No AI. Quyết định là Not Yet cho tới khi có bằng chứng CP4.

## 7. Tài liệu tham khảo

- [Worksheet](../../docs/01-worksheet.md)
- [Rubric](../../RUBRIC.md)
