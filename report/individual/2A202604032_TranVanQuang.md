# Báo cáo cá nhân — 2A202604032_TranVanQuang

## 1. Thông tin học viên

- Họ tên — Trần Văn Quang
- MSSV — 2A202604032
- Nhóm — AIS
- Link repo nhóm — (<https://github.com/OuyangXuelili/K5-L3B-DAY02-AIS-DiscoveryProblemFraming>).
- Vai trò dự kiến — Quy trình, cách đo và Problem Statement v0 ở CP5.

---

## 2. Scan problem (CP1)

Bảng ghi các đề xuất đã chuẩn bị và loại dấu hiệu cần kiểm.

| # | Lăng kính | Job Story gợi ý | Ai chịu ảnh hưởng? | Dữ liệu cần bổ sung từ một lần thật | Ví dụ giả lập |
|---:|---|---|---|---|---|
| 1 | Cần tổng hợp nhiều thông tin | Khi nhóm bắt đầu sửa một bản nháp đã được góp ý ở nhiều chỗ, tôi muốn biết góp ý nào còn mở, để mỗi việc được xử lý đúng một lần. | Người tổng hợp hoặc sửa bài nhóm | Bản nháp nào, có mấy kênh, mất bao lâu để gom, có góp ý nào bị bỏ sót hoặc sửa trùng. | Rà 7 bình luận và 5 tin nhắn mất 24 phút, trong đó đối chiếu mất 11 phút. |
| 2 | Tốn thời gian | Khi mở lại bài đang làm dở, tôi muốn biết đâu là bản mới nhất, để tiếp tục chỉnh từ đúng nội dung. | Người quay lại sửa bài nhóm | Lần tìm gần nhất, số bản hoặc số link đã mở, thời gian tìm và hậu quả nếu sửa sai bản. | Mở 3 link và xác nhận bản mới nhất mất 15 phút. |
| 3 | Pain từ người khác | Khi một buổi họp kết thúc, tôi muốn biết ai đã nhận từng đầu việc, để cả nhóm có thể bắt đầu mà không phải hỏi lại. | Người giao việc và người thực hiện | Số đầu việc chưa rõ người nhận, số tin nhắn hỏi lại hoặc thời gian chờ xác nhận. | Rà 6 đầu việc mất 14 phút, 2 việc cần hỏi ai nhận. |
| 4 | Cần đọc nhiều thông tin | Khi nhận một đề lab có nhiều tệp hướng dẫn, tôi muốn xác định đúng yêu cầu của mục mình phụ trách, để dành thời gian cho đúng phần được chấm. | Người làm bài lab | Mục từng phải tra, các tệp đã mở, thời gian tra và điều đã phải hỏi lại. | Đối chiếu 3 tệp hướng dẫn cho một mục mất 18 phút. |
| 5 | Lặp lại | Khi quay lại một nội dung từng học, tôi muốn tìm đúng ví dụ đã lưu, để có thể tiếp tục bài đang làm. | Người học hoặc người hỗ trợ bạn học | Lần tìm gần nhất, số nơi đã tìm, thời gian và kết quả. | Tìm một ví dụ ở hai thư mục và một đoạn chat mất 9 phút. |

---

## 3. Top 3 Problem Cards và quy trình nháp (CP2)

Thứ tự dưới đây là đề xuất. Hồ sơ chưa có số đo hoặc ước lượng có nguồn cho các bước.

### Bảng chọn top 3

| Hạng nháp | Vấn đề | Lý do ưu tiên | Điều cần xác nhận |
|---:|---|---|---|
| 1 | Xác định góp ý còn mở khi sửa bản nháp nhóm | Đo được thời gian gom và số góp ý còn sót hoặc bị ghi trùng. | Có vòng sửa thực sự dùng hai kênh không? |
| 2 | Tìm bản mới nhất trước khi sửa | Có thể quan sát một lần tìm và đối chiếu link. | Có từng mất thời gian hoặc sửa nhầm bản không? |
| 3 | Xác nhận ai nhận việc sau buổi họp | Có thể đếm đầu việc thiếu người nhận và lượt hỏi lại. | Có lần họp cụ thể để mô tả không? |

Các thời lượng và mục tiêu bổ sung là giả lập. Dùng số đo từ một lượt thật để xác lập baseline.

### Problem Card #1 — Góp ý còn mở ở nhiều kênh

| Trường | Giả thuyết cần đối chiếu |
|---|---|
| Job Story và actor | Khi bắt đầu sửa bản nháp đã được nhận xét, tôi muốn thấy các góp ý còn mở để biết việc nào cần sửa. Actor là thành viên tổng hợp góp ý. |
| Bối cảnh | Một bản nháp, một vòng sửa, có góp ý ở chat và bình luận tài liệu. |
| Quy trình và bottleneck | Xem sơ đồ. Nghi vấn chính là đối chiếu góp ý ở hai nơi để xác định việc nào trùng, việc nào đã xử lý. |
| Impact | Có thể phải hỏi lại hoặc sửa một ý hai lần. Ghi số lần hoặc thời gian từ một vòng sửa thật. |
| Success metric | Số phút để lập danh sách góp ý còn mở và số góp ý bị bỏ sót. Chưa có baseline và mục tiêu đã xác nhận. |
| Baseline → mục tiêu minh họa | 24 → tối đa 18 phút để chốt một vòng khoảng 12 ghi nhận. Bấm giờ tới khi danh sách được duyệt, kiểm 0 góp ý quan trọng bị sót. |
| Phương án không dùng AI | Ghi góp ý thành một danh sách chung có đoạn liên quan, nguồn, người nhận và trạng thái. |
| Giả thuyết về AI | AI có thể gợi ý cặp nhận xét gần nghĩa. Người phụ trách mở hai nguồn và tự chốt. |
| Cảm nhận nhanh | No AI cho vòng thử đầu. |
| Giả thuyết can thiệp | Bắt đầu ở No AI. Nếu khâu gom còn nặng sau khi thử danh sách chung, kiểm tra khả năng dùng Rule cho góp ý có mã mục. |

**Quy trình nháp hiện tại**

```text
Mở đúng bản nháp [2 phút minh họa] → đọc comment [4 phút minh họa] → tìm góp ý trong chat [5 phút minh họa]
→ đối chiếu góp ý và trạng thái [11 phút minh họa, bước nghẽn]
→ ghi danh sách cần sửa [2 phút minh họa]
```

**Tổng thời gian minh họa** — 24 phút.

### Problem Card #2 — Tìm bản mới nhất trước khi sửa

| Trường | Giả thuyết cần đối chiếu |
|---|---|
| Job Story và actor | Khi quay lại sửa bài sau một lần bàn giao, tôi muốn mở đúng bản mới nhất, để các chỉnh sửa của tôi nằm trong bản nhóm sẽ dùng. Actor là người tiếp tục chỉnh bản nháp. |
| Bối cảnh | Nhóm chia sẻ nhiều link hoặc bản sao trong một đợt chỉnh sửa. |
| Quy trình và bottleneck | Xem sơ đồ. Bước có thể nghẽn là đối chiếu các link và xác nhận bản đang dùng. |
| Impact | Phải hỏi lại hoặc chuyển phần đã sửa sang bản chính. Ghi trường hợp và số phút thật nếu có. |
| Success metric | Số phút mỗi lần xác định bản đúng và số lần mở nhầm bản. Chưa có baseline và mục tiêu đã xác nhận. |
| Baseline → mục tiêu minh họa | 15 → tối đa 6 phút mỗi lần xác định bản đúng. Dùng link đã chốt làm đối chứng và đếm lần mở nhầm bản. |
| Phương án không dùng AI | Dùng một link bản chính được ghim, có người cập nhật khi đổi bản. |
| Giả thuyết về AI | Có thể đọc tiêu đề và tóm tắt điểm khác nhau giữa hai bản. Link được nhóm ghim vẫn là căn cứ xác nhận. |
| Cảm nhận nhanh | No AI với một link bản chính. |
| Giả thuyết can thiệp | No AI nếu quy ước một bản chính giải quyết được việc tìm. |

**Quy trình nháp hiện tại**

```text
Mở link được gửi [2 phút minh họa] → tìm các link liên quan [4 phút minh họa]
→ đối chiếu và xác nhận bản chính [8 phút minh họa, bước nghẽn]
→ mở đúng bản để tiếp tục [1 phút minh họa]
```

**Tổng thời gian minh họa** — 15 phút.

### Problem Card #3 — Xác nhận người phụ trách sau buổi họp

| Trường | Giả thuyết cần đối chiếu |
|---|---|
| Job Story và actor | Khi buổi họp nhóm vừa kết thúc, tôi muốn biết từng đầu việc đã có người nhận hay chưa, để tránh việc bị bỏ quên. Actor là thành viên điều phối. |
| Bối cảnh | Nhóm vừa phân chia công việc cho một bài có nhiều phần. |
| Quy trình và bottleneck | Xem sơ đồ. Nghi vấn nằm ở bước xác nhận ai đã nhận các việc còn mơ hồ. |
| Impact | Một đầu việc có thể bị chậm hoặc được hai người làm cùng lúc. Ghi số lượt hỏi lại hoặc số đầu việc thiếu người nhận nếu từng xảy ra. |
| Success metric | Số đầu việc thiếu người nhận khi chốt. Ghi riêng thời gian xác nhận. Chưa có baseline và mục tiêu đã xác nhận. |
| Baseline → mục tiêu minh họa | 2 → 0 việc chưa có người nhận trong 6 việc. Đối chiếu với bảng phân công và ghi số phút xác nhận. |
| Phương án không dùng AI | Đọc lại bảng đầu việc và xác nhận người nhận trước khi kết thúc họp. |
| Giả thuyết về AI | AI có thể gợi ý đầu việc từ ghi chú họp. Người điều phối hỏi lại và xác nhận người nhận. |
| Cảm nhận nhanh | No AI với bảng phân công. |
| Giả thuyết can thiệp | No AI nếu nhóm có thể xác nhận trực tiếp trong buổi họp. |

**Quy trình nháp hiện tại**

```text
Đọc ghi chú họp [2 phút minh họa] → liệt kê đầu việc [3 phút minh họa]
→ xác nhận người nhận [7 phút minh họa, bước nghẽn] → chia sẻ phân công [2 phút minh họa]
```

**Tổng thời gian minh họa** — 14 phút.

### Nội dung chuẩn bị pitch

Card 1 là đề xuất ưu tiên trong bản chuẩn bị. Câu hỏi đã soạn — Trong lần gần nhất, phần mất công là tìm đủ nguồn, hiểu góp ý, hay xác nhận góp ý đã được xử lý? Hồ sơ chưa có ghi nhận buổi pitch hoặc chỉnh sửa sau phản biện của thành viên.

**Phản biện AI trong lúc chuẩn bị** — Đổi tiêu chí gộp từ cùng đoạn sang cùng hành động cần sửa và giữ cả hai mã nguồn.

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

Theo [TEAM.md](../../TEAM.md#tranvanquang-2a202604032), Trần Văn Quang (TV01) phụ trách chính CP5 và hỗ trợ CP4 Research, CP6. Đây là phân công dự kiến. Hồ sơ chưa có ghi nhận đóng góp thực tế hoặc bằng chứng được thành viên xác nhận.

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch và phản biện (CP3) | Phân công chung là mỗi người trình bày 3 card. | Chưa có biên bản pitch hoặc phản biện của TV01. |
| Research (CP4) | Dự kiến hỗ trợ TV04 kiểm tra 2–3 nguồn, tính năng và giới hạn của từng phương án. | Chưa có ghi nhận kết quả phần hỗ trợ của TV01. |
| Quy trình nhóm và Problem Statement v0 (CP5) | Phụ trách chính, phối hợp với TV03. Phần việc gồm rà sơ đồ, xác định số đo hiện tại, mục tiêu, cách đo và phạm vi. Nội dung chuẩn bị tách thời gian mở bản, đọc hai nguồn, đối chiếu và chốt trạng thái, có tính cả thời gian nhập và rà bảng. | Phần được phân công nằm ở mục 4–5 trong [báo cáo nhóm](../team/group_report.md). TEAM.md chưa ghi nhận đóng góp thực tế. |
| Mức can thiệp và Problem Statement v1 (CP6) | Dự kiến hỗ trợ TV04 so sánh bốn mức can thiệp, viết tiêu chí đánh giá và nêu thay đổi so với v0. | Chưa có ghi nhận kết quả phần hỗ trợ của TV01. |
| Quyết định (CP6) | Dự kiến cùng nhóm xem xét bốn rủi ro, quyết định và ngưỡng dừng. | Chưa có ghi nhận quyết định hoặc ý kiến của TV01. |

**Câu hỏi để luyện pitch** — Nếu hai ý cùng nhắc một đoạn nhưng yêu cầu khác nhau, căn cứ nào đủ để gộp?

Điều học được từ phần nhóm chưa được ghi trong TEAM.md.

---

## 5. Dùng AI

| Mục | AI hỗ trợ trong lần cập nhật | Cách rà trước khi dùng |
|---|---|---|
| CP1 | Bổ sung ví dụ định lượng theo từng Job Story. | Thay ví dụ bằng quan sát và số liệu của thành viên. |
| CP2 | Gợi ý thời lượng, chỉ số thử và câu hỏi phản biện. | Đổi tiêu chí gộp từ cùng đoạn sang cùng hành động cần sửa và giữ cả hai mã nguồn. |
| CP7 | Soạn reflection mẫu cho một kịch bản giả lập. | Tự viết lại theo sự việc và quyết định mình thực sự tham gia. |

---

## 6. Reflection (CP7)

**6.1. Điều rút ra từ các card**

Ba card giúp phân biệt việc tìm đúng phiên bản, việc đối chiếu góp ý và việc xác nhận người nhận. Từng bước có một đầu ra khác nhau. Vì thế thời gian chọn đúng bản không thể thay cho thời gian chốt danh sách còn mở.

**6.2. Lúc dễ chọn giải pháp quá sớm**

Một giải pháp tự động gom nhận xét dễ được chọn quá sớm. Câu hỏi cần đặt trước là người tổng hợp hiện dựa vào thông tin nào để biết một ý đã xử lý và ở bước nào họ phải quay lại kiểm nguồn.

**6.3. Phản biện làm đổi cách làm**

Một phản biện trong kịch bản là hai nhận xét cùng nhắc một đoạn có thể yêu cầu hai thay đổi khác nhau. Bản mẫu chỉ gộp khi yêu cầu hành động giống nhau và giữ mã của từng nguồn sau khi gộp.

**6.4. Điều CP4 cần kiểm**

CP4 cần kiểm tra xem đối chiếu có thật sự lâu hơn đọc chat hay không. Một tín hiệu phản bác đáng lưu là một nhóm đã dùng bình luận tài liệu cho mọi nhận xét và chỉ trao đổi lịch trong chat.

**6.5. Chỗ khó của Problem Statement**

Khó nhất là chọn mốc dừng đồng hồ. Dừng khi mới nhập xong bảng sẽ bỏ phần rà trạng thái và xác nhận người nhận. Mốc phù hợp hơn là lúc người phụ trách chốt danh sách việc còn mở.

**6.6. Việc sẽ đổi khi làm lại**

Nếu làm lại, ưu tiên tái hiện một vòng sửa thật rồi ghi thời gian từng bước. Cần thống nhất trước tiêu chí góp ý quan trọng và để người thứ hai kiểm danh sách trước khi kết luận cách nào tốt hơn.

**6.7. Giải thích mạch bài toán**

Trong một vòng sửa, người tổng hợp cần biết góp ý nào còn mở khi nhận xét đến từ chat và bình luận tài liệu. Quy trình bắt đầu khi xác định bản nháp và kết thúc khi chốt danh sách. Bước nghẽn dự kiến là đối chiếu ý mới, ý trùng và ý đã xử lý. Mục tiêu thử là giảm ít nhất 25% trung vị thời gian với 0 góp ý quan trọng bị sót. Người phụ trách xác nhận nguồn và chốt ý mâu thuẫn. Phương án dự kiến là bảng thủ công No AI. Quyết định là Not Yet cho tới khi có bằng chứng CP4.

---

## 7. Tài liệu tham khảo

- [Worksheet của lab](../../docs/01-worksheet.md)
- [Rubric](../../RUBRIC.md)
