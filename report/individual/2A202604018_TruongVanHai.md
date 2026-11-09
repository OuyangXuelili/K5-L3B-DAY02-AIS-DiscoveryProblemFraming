# Báo cáo cá nhân — 2A202604018_TruongVanHai

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Trương Văn Hải
- MSSV: 2A202604018
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: AIS
- Link repo nhóm: [Link repo nhóm](https://github.com/OuyangXuelili/K5-L3B-DAY02-AIS-DiscoveryProblemFraming)

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi cần chốt lịch họp nhóm mà mỗi người gửi giờ rảnh ở một tin nhắn khác nhau, tôi muốn biết khung giờ mọi người có thể tham gia, để chốt lịch với ít lượt hỏi lại. | Người điều phối cuộc họp | Lần hẹn gần nhất, số thành viên, số lượt hỏi lại và số phút từ khi bắt đầu tổng hợp đến khi xác định được giờ họp. |
| 2 | Pain từ người khác | Khi chia một báo cáo thành nhiều phần, tôi muốn xác định phạm vi và đầu ra của từng phần, để mỗi nội dung được giao cho đúng người. | Người chia việc và người viết báo cáo | Lần phân công gần nhất, số phần chồng nhau, phần nào phải bỏ hoặc sửa lại và mất bao lâu. |
| 3 | Cần đọc, tổng hợp nhiều thông tin | Khi cần giải thích vì sao nhóm đã chọn một phương án từ buổi thảo luận trước, tôi muốn tìm được căn cứ và phương án đã cân nhắc, để tiếp tục việc đang làm mà không phải tranh luận lại từ đầu. | Thành viên cần giải thích quyết định nhóm | Quyết định cụ thể, số nơi đã tra, số phút tìm và có phải hỏi lại ai không. |
| 4 | Tốn thời gian | Khi cả nhóm phải ghép nhiều phần trình bày vào một khung giờ ngắn, tôi muốn biết phần nào cần cắt trước lúc tập dượt, để trình bày đủ ý trong thời gian quy định. | Người chuẩn bị bài thuyết trình nhóm | Thời lượng cho phép, thời gian lần tập gần nhất, số lượt phải tập lại. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi hai hướng dẫn tôi đang dùng diễn đạt yêu cầu khác nhau, tôi muốn xác nhận cách hiểu áp dụng cho phần mình làm, để tránh mất công sửa sai hướng. | Thành viên phụ trách một mục báo cáo | Yêu cầu cụ thể, hai nguồn, số phút tra cứu và câu hỏi xác nhận đã gửi nếu có. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Bổ sung ví dụ định lượng theo từng Job Story: giữ lại khung cấu trúc và định hướng số đo, thay ví dụ giả định bằng quan sát và số liệu thực tế của thành viên.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Chốt lịch họp nhóm qua nhiều lượt nhắn | Dễ xác định mốc bắt đầu, đầu ra và số lượt nhắn. | Có mất công chủ yếu ở lúc đối chiếu, hay ở lúc chờ người chưa phản hồi? |
| 2 | Phát hiện hai người nhận phần việc chồng nhau | Có thể đối chiếu bản phân công với đầu ra thật. | Các phần giao nhau do phân công mơ hồ hay do đề bài vốn có chung dữ liệu? |
| 3 | Tìm lại căn cứ khi nhóm chọn phương án | Phân biệt được việc có kết luận với việc tìm được lý do. | Nhóm có cần tìm lý do thường xuyên hay chỉ cần xem lựa chọn cuối? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần chốt lịch họp nhóm mà mỗi người gửi giờ rảnh ở một tin nhắn khác nhau, tôi muốn biết khung giờ mọi người có thể tham gia, để chốt lịch với ít lượt hỏi lại. |
| Actor | Người điều phối cuộc họp. |
| Thời điểm / bối cảnh | Nhóm có hạn chốt lịch cho một buổi họp, giờ rảnh được gửi rời rạc. |
| Quy trình hiện tại (3–7 bước) | 1. Gửi các khung giờ dự kiến; 2. Thu giờ rảnh từ từng người; 3. Đối chiếu điểm giao và hỏi lại các câu mơ hồ; 4. Chốt và thông báo giờ họp. (Xem sơ đồ nháp bên dưới). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3. Đối chiếu điểm giao và hỏi lại các câu mơ hồ (9 phút minh họa, bước nghẽn). Chưa có số đo và căn cứ xác nhận. |
| Impact (nếu không giải thì sao) | Có thể phải nhắn hỏi lại hoặc đổi lịch. Ghi hậu quả thực tế từ lần hẹn gần nhất. |
| Success metric (baseline → target) | 17 → tối đa 10 phút thao tác cho một lần hẹn 4 người; giảm từ 2 xuống tối đa 1 lượt hỏi lại (số phút chủ động để tìm giờ phù hợp và số lượt hỏi lại, ghi riêng thời gian chờ phản hồi). |
| Phương án không dùng AI | Cho mọi người điền vào một bảng giờ chung với giờ khóa phản hồi. |
| Giả thuyết về AI (nếu có) | Nếu mọi người ghi giờ theo cùng định dạng, có thể dùng quy tắc lọc giao nhau. (No AI. Chỉ cân nhắc Rule để tìm giao điểm nếu mọi người nhập theo các khung giờ cố định). |
| Cảm nhận nhanh | Rule (sau khi chuẩn hóa đầu vào) / No AI |

Quy trình nháp hiện tại:

```text
1. Gửi các khung giờ dự kiến [2 phút minh họa]
   ↓
2. Thu giờ rảnh từ từng người [4 phút minh họa]
   ↓
3. Đối chiếu điểm giao và hỏi lại các câu mơ hồ [9 phút minh họa, bước nghẽn]
   ↓
4. Chốt và thông báo giờ họp [2 phút minh họa]

Tổng thời gian minh họa: 17 phút.
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi chia một báo cáo thành nhiều phần, tôi muốn xác định phạm vi và đầu ra của từng phần, để mỗi nội dung được giao cho đúng người. |
| Actor | Người chia việc và người viết báo cáo. |
| Thời điểm / bối cảnh | Hai thành viên được phân công các phần có liên quan của cùng một bản báo cáo. |
| Quy trình hiện tại (3–7 bước) | 1. Đọc yêu cầu đầu ra; 2. Liệt kê các phần cần làm; 3. Đối chiếu các phần có cùng đầu ra; 4. Chốt người phụ trách và ranh giới. (Xem sơ đồ nháp bên dưới). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3. Đối chiếu các phần có cùng đầu ra (8 phút minh họa, bước nghẽn). Chưa có số đo và căn cứ xác nhận. |
| Impact (nếu không giải thì sao) | Có thể viết trùng hoặc phải chỉnh lại nội dung giữa hai phần. Đếm số phần bị ảnh hưởng. |
| Success metric (baseline → target) | 2 → 0 cặp đầu ra chồng nhau trong 7 mục (đối chiếu bảng phân công với đầu ra của từng mục). |
| Phương án không dùng AI | Mỗi đầu việc ghi một đầu ra và một người chịu trách nhiệm chính. Dùng bước cả nhóm đọc lại phân công trước khi bắt đầu. |
| Giả thuyết về AI (nếu có) | AI có thể gợi ý hai mục mô tả đầu ra tương tự. Người chia việc xác nhận phạm vi. |
| Cảm nhận nhanh | No AI (với đầu ra và người chịu trách nhiệm rõ) |

Quy trình nháp hiện tại:

```text
1. Đọc yêu cầu đầu ra [3 phút minh họa]
   ↓
2. Liệt kê các phần cần làm [4 phút minh họa]
   ↓
3. Đối chiếu các phần có cùng đầu ra [8 phút minh họa, bước nghẽn]
   ↓
4. Chốt người phụ trách và ranh giới [2 phút minh họa]

Tổng thời gian minh họa: 17 phút.
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần giải thích vì sao nhóm đã chọn một phương án từ buổi thảo luận trước, tôi muốn tìm được căn cứ và phương án đã cân nhắc, để tiếp tục việc đang làm mà không phải tranh luận lại từ đầu. |
| Actor | Thành viên cần giải thích quyết định nhóm. |
| Thời điểm / bối cảnh | Một quyết định cũ ảnh hưởng tới việc chỉnh sửa báo cáo hiện tại. |
| Quy trình hiện tại (3–7 bước) | 1. Xác định quyết định cần giải thích; 2. Tra ghi chú họp; 3. Dò lý do và phương án thay thế trong trao đổi; 4. Xác nhận lại căn cứ với người chốt. (Xem sơ đồ nháp bên dưới). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3. Dò lý do và phương án thay thế trong trao đổi (10 phút minh họa, bước nghẽn). Chưa có số đo và căn cứ xác nhận. |
| Impact (nếu không giải thì sao) | Phải hỏi lại hoặc lặp lại phần thảo luận. Ghi thời gian và số người đã phải hỏi. |
| Success metric (baseline → target) | 18 → tối đa 8 phút đến khi tìm được lý do chọn và một phương án từng cân nhắc. Xác nhận qua ghi chú gốc. |
| Phương án không dùng AI | Lưu một dòng cho mỗi quyết định gồm lựa chọn, lý do và nơi đã chốt. |
| Giả thuyết về AI (nếu có) | AI có thể gợi ý đoạn nhắc tới một lựa chọn. Thành viên mở nguồn trước khi dùng lý do. |
| Cảm nhận nhanh | No AI (nếu quyết định đã có một dòng lưu) |

Quy trình nháp hiện tại:

```text
1. Xác định quyết định cần giải thích [2 phút minh họa]
   ↓
2. Tra ghi chú họp [3 phút minh họa]
   ↓
3. Dò lý do và phương án thay thế trong trao đổi [10 phút minh họa, bước nghẽn]
   ↓
4. Xác nhận lại căn cứ với người chốt [3 phút minh họa]

Tổng thời gian minh họa: 18 phút.
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Dễ xác định mốc bắt đầu, đầu ra và số lượt nhắn; card là đề xuất ưu tiên trong bản chuẩn bị.
- Câu hỏi muốn nhóm phản biện: Có mất công chủ yếu ở lúc đối chiếu, hay ở lúc chờ người chưa phản hồi? Nếu thời gian chủ yếu là chờ phản hồi thì bảng giờ chung giảm được phần nào?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chưa tách thời gian chủ động đối chiếu khỏi thời gian chờ phản hồi, làm sai lệch đo lường tác động của bảng giờ. | Đồng ý | Tách riêng thời gian chủ động đối chiếu khỏi thời gian chờ để đo đúng tác động của bảng giờ; bổ sung câu hỏi phản biện về việc chờ người chưa phản hồi. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Chuẩn bị và pitch Card 1 (Chốt lịch họp nhóm qua nhiều lượt nhắn). Đưa ra câu hỏi thảo luận về thời gian đối chiếu và thời gian chờ. | Nhóm cân nhắc và so sánh C4 với C1 và C2 theo phạm vi và khả năng đo lường. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: "Nếu thời gian chủ yếu là chờ phản hồi thì bảng giờ chung giảm được phần nào?" và "Nếu góp ý đã được chốt ngay trong tài liệu thì bước nào còn đáng cải thiện?" | Giúp nhóm làm rõ ranh giới giữa thời gian thao tác và thời gian chờ, hoàn thiện giả định A2. |
| Nhận phản biện | Câu hỏi tôi nhận được: Có mất công chủ yếu ở lúc đối chiếu, hay ở lúc chờ người chưa phản hồi? | Tôi đã sửa gì: Tách riêng thời gian chủ động đối chiếu khỏi thời gian chờ để đo đúng tác động của phương án bảng giờ. |
| Gom cluster / cây OST | Đưa 12 card của nhóm về cùng cách trình bày theo actor và bước nghẽn; chuẩn bị so sánh C1, C2 và C4 theo phạm vi và khả năng đo. | Cấu trúc hóa 12 card của nhóm và hỗ trợ xây dựng cây cơ hội OST cho C1. |
| Chọn candidate problem | Cùng nhóm phân tích và đối chiếu các card; đồng thuận chọn C1 (góp ý còn mở ở nhiều kênh) làm candidate chính vì có phạm vi rõ và dễ đo lường. | Thống nhất candidate C1 cho báo cáo nhóm. |
| Kiểm chứng / research | Tham gia rà soát bản đồ giả định (Assumption Map A1-A5) và chuẩn bị kế hoạch phỏng vấn người tổng hợp góp ý. | Định hình các giả định cần kiểm chứng ở CP4. |
| Quy trình nhóm | Tham gia thảo luận và rà soát sơ đồ quy trình hiện tại (5 bước) và quy trình tương lai (bảng thủ công dùng chung). | Thống nhất sơ đồ quy trình trước/sau cho nhóm. |
| Problem Statement | Tham gia thảo luận xây dựng v0 và v1, xác định rõ actor, bước nghẽn và success metric (giảm ≥25% thời gian, 0 góp ý bị sót). | Hoàn thiện Problem Statement v1 của nhóm. |
| Mức can thiệp AI | Phân tích ma trận mức độ can thiệp (mơ hồ cao × phức tạp thấp), đề xuất mức No AI (bảng thủ công). | Nhóm thống nhất mức can thiệp đề xuất là No AI. |
| Quyết định | Đồng thuận quyết định đề xuất là "Not Yet", cần kiểm chứng thêm ở CP4 trước khi triển khai pilot. | Đưa ra quyết định Not Yet và tiêu chí dừng/tiếp tục rõ ràng cho nhóm. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Bổ sung ví dụ định lượng và dấu hiệu thực tế theo từng Job Story. | Gợi ý các khía cạnh đo lường (thời gian, tần suất, số người). | Đưa ra số liệu giả định chung chung, chưa sát với bối cảnh thực tế của học viên. | Thay thế ví dụ và số liệu bằng quan sát, trải nghiệm thực tế của bản thân. |
| CP2 Problem Card | Gợi ý thời lượng minh họa các bước, chỉ số thử nghiệm và câu hỏi phản biện card. | Tạo khung phân bổ thời lượng 3–7 bước và đặt câu hỏi gợi ý bước nghẽn. | Gộp chung thời gian chờ phản hồi vào thời gian thao tác chủ động của người điều phối. | Tách riêng thời gian chủ động đối chiếu khỏi thời gian chờ để đo đúng tác động của bảng giờ. |
| CP4 Research | Gợi ý các giả định cần kiểm chứng và cấu trúc câu hỏi phỏng vấn. | Liệt kê nhanh các góc nhìn Value, Usability, Feasibility. | Các câu hỏi còn mang tính dẫn dắt giải pháp ("có thích dùng tool không"). | Sửa câu hỏi hướng vào hành vi thực tế ở vòng sửa gần nhất, không hỏi về công cụ mới. |
| CP5 Quy trình | Vẽ khung sơ đồ quy trình hiện tại và quy trình tương lai. | Trực quan hóa luồng các bước từ input đến output. | Chưa làm rõ ranh giới ai là người chốt khi có ý kiến trái chiều. | Bổ sung bước chốt của người phụ trách nội dung và xử lý ý mâu thuẫn. |
| CP5–6 Problem Statement | Soạn thử câu Problem Statement theo mẫu chuẩn. | Đảm bảo đầy đủ các thành phần Actor, Bottleneck, Metric. | Metric đưa ra thường là tên công cụ hoặc chưa có ranh giới rõ ràng. | Chuyển thành metric đo lường kết quả cụ thể (giảm ≥25% thời gian, 0 góp ý quan trọng bị sót). |
| CP6 Mức can thiệp / quyết định | Phân tích các mức giải pháp từ No AI đến Agent trên ma trận. | Nêu rõ ưu nhược điểm và rủi ro của từng mức công nghệ. | Thường có xu hướng đề xuất áp dụng ngay AI/Agent dù chưa có đủ dữ liệu kiểm chứng. | Giữ vững đề xuất mức No AI (bảng thủ công) và quyết định Not Yet theo đúng nguyên tắc rubric. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi so các card trong kịch bản, việc nhiều người thấy bất tiện chưa đủ để xác định bước nghẽn. Card lịch họp cần ghi riêng thời gian chờ phản hồi và công tổng hợp giờ rảnh của người điều phối.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Trong shortlist minh họa, một card có số phút lớn chưa chắc dễ kiểm. Cần đầu vào tương đương giữa các lần và một mốc kết thúc mà mọi người hiểu giống nhau, chẳng hạn lúc lịch được xác nhận.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Một phản biện có thể làm đổi thứ hạng là nhóm đã ghim đường dẫn bản chính. Khi đó card tìm đúng bản giảm giá trị, còn đối chiếu góp ý vẫn đáng xem nếu nhận xét tiếp tục đến từ hai kênh.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

CP4 cần hỏi người mới tổng hợp một vòng sửa và cả người thấy cách hiện tại đã đủ. Hai loại tình huống giúp xác định nhóm nào thực sự có vấn đề trước khi hỏi về một công cụ mới.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất là chuyển tên công cụ thành kết quả có thể đo. Với C1, kết quả là danh sách việc còn mở đã được xác nhận. Giữ nguồn cho từng mục giúp người khác kiểm lại danh sách đó.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, nên dành thời gian pitch tương đương cho từng card và ghi lý do loại trong lúc thảo luận. Người không dự họp có thể đọc lý do và kiểm vì sao nhóm nghiêng về một ứng viên.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Trong một vòng sửa, người tổng hợp cần biết góp ý nào còn mở khi nhận xét đến từ chat và bình luận tài liệu. Quy trình bắt đầu khi xác định bản nháp và kết thúc khi chốt danh sách. Bước nghẽn dự kiến là đối chiếu ý mới, ý trùng và ý đã xử lý. Mục tiêu thử là giảm ít nhất 25% trung vị thời gian với 0 góp ý quan trọng bị sót. Người phụ trách xác nhận nguồn và chốt ý mâu thuẫn. Phương án dự kiến là bảng thủ công No AI. Quyết định là Not Yet cho tới khi có bằng chứng CP4.

---

## 7. Tài liệu tham khảo

- [Worksheet](../../docs/01-worksheet.md)
- [Rubric](../../RUBRIC.md)
