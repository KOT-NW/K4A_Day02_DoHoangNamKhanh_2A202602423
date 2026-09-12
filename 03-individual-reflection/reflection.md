# 03 — Individual Reflection

## Thông tin cá nhân

- Họ và tên: Đỗ Hoàng Nam Khánh
- Mã học viên: 2A202602423
- Nhóm: C sủi
- Candidate problem nhóm chọn: FreshBox — theo dõi batch thực phẩm trong tủ lạnh để biết món nào nên dùng trước. Nhóm đã thống nhất chọn FreshBox.

## 1. Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Đưa ra các vấn đề về FreshBox, thủ tục online, giao thông, ô nhiễm, đi làm xa và gọi thợ sửa chữa. | Nhóm có thêm các candidate gắn với đời sống và có thể so sánh. |
| Pitch Problem Card | Trình bày FreshBox: batch, timestamp, FIFO và giảm food waste. | Đề xuất có tình huống sử dụng cụ thể và hướng prototype rõ hơn. |
| Challenge bài của bạn khác | Hỏi về mục đích sử dụng, đối tượng, thói quen và tâm lý tiêu dùng. | Buộc các ý tưởng nói rõ ai dùng và dùng trong hoàn cảnh nào. |
| Gom trùng / cluster | Gộp các ý tưởng quanh nhu cầu tiện lợi, tìm dịch vụ và quản lý đồ dùng. | Giúp nhóm nhìn ra pattern thay vì chỉ so sánh tên solution. |
| Chọn candidate problem | Ưu tiên FreshBox vì gần đời sống và có thể thử nghiệm thực tế; nhóm C sủi đã thống nhất chọn bài này. | Nhóm có một bài để đào sâu thay vì giữ nhiều ý tưởng quá rộng. |
| Validation / research | Tìm thêm bối cảnh về dịch vụ công, ô nhiễm và các nền tảng gọi thợ. | Có cơ sở tham khảo và nhận ra cần kiểm chứng pain bằng người dùng thật. |
| Workflow nhóm | Mô tả flow đặt thực phẩm vào rack → ghi ID/timestamp → theo dõi cân nặng → nhắc FIFO. | Làm rõ điểm sensor hỗ trợ và điểm người dùng vẫn cần xác nhận. |
| Problem Statement | Góp ý actor, batch, food waste, thao tác nhập liệu và boundary không tuyên bố an toàn tuyệt đối. | Problem được thu hẹp vào inventory awareness và batch tracking. |
| Rule / Workflow / Agent | Đề xuất MVP dùng sensor, ID, timestamp, weight và rule FIFO; chưa cần Agent. | Giảm scope và rủi ro kỹ thuật ban đầu. |
| Decision | Đặt câu hỏi về mức đầu tư, range sản phẩm và chi phí nếu sensor sai. | Nhóm cần tính cả feasibility và fallback, không chỉ nhìn vào ý tưởng. |

**Dấu tay rõ nhất của tôi:** Tôi đưa FreshBox vào nhóm và giúp chuyển ý tưởng “tủ lạnh thông minh” thành bài toán cụ thể hơn: nhận diện từng batch, ghi thời điểm và ưu tiên sử dụng.

## 2. Bảng dùng AI

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Gợi ý thêm vấn đề theo các lăng kính của worksheet. | Mở rộng từ trải nghiệm học tập sang thủ tục, giao thông và dịch vụ gia đình. | Một số gợi ý chung chung, không có actor hoặc dấu hiệu thật. | Giữ lại vấn đề có liên hệ đời sống và ghi rõ dữ liệu nào cần tự đo. |
| Problem Card | Nhờ AI hỏi ngược về actor, workflow và metric. | Giúp tách “có thực phẩm” thành các batch khác nhau. | Có lúc AI đi quá nhanh sang camera/AI nhận diện. | Hạ MVP về sensor, ID, timestamp, weight và FIFO. |
| Workflow | Chuyển mô tả thành flow ngắn. | Nhìn rõ bottleneck và fallback. | AI có xu hướng gộp bước xác nhận của người dùng. | Tách human confirmation và nêu cách sửa thủ công khi sensor sai. |
| Research | Tìm nguồn về dịch vụ công, ô nhiễm và các nền tảng gọi thợ. | Biết đã có sản phẩm giải quyết một phần bài toán. | Không phải mọi claim trên website đều là bằng chứng độc lập. | Chỉ dùng để nêu bối cảnh; không coi đó là số đo pain cá nhân. |
| Problem Statement | Phản biện câu problem và boundary. | Giúp câu chữ ngắn và cụ thể hơn. | AI có thể làm solution nghe hấp dẫn hơn problem. | Giữ trọng tâm inventory awareness, batch tracking và food waste. |
| Rule / Workflow / Agent | So sánh mức tự động hóa. | Làm rõ Agent chưa cần thiết vì flow MVP khá thẳng. | AI thường đề xuất Agent vì nghe “thông minh” hơn. | Chọn Workflow kết hợp Rule, có người kiểm tra. |
| Decision | Gợi ý câu hỏi về feasibility và rủi ro. | Bổ sung câu hỏi đầu tư, range sản phẩm, thói quen và chi phí sai. | Không thể thay nhóm quyết định Go/Not Yet/No-Go. | Tôi giữ quyền đánh giá dựa trên dữ liệu và ngữ cảnh thực tế. |

## 3. Reflection

Tôi đã đóng góp bằng cách đưa ra nhiều vấn đề có liên hệ với đời sống, trong đó FreshBox là ý tưởng tôi muốn pitch nhất. Tôi được challenge về việc giải pháp có đáng để đầu tư hay không, đối tượng sử dụng là ai và range sản phẩm nên rộng đến mức nào. Tôi cũng chủ động challenge các ý tưởng khác về mục đích sử dụng, thói quen và tâm lý tiêu dùng. Qua thảo luận, mọi người phải cụ thể hóa các tình huống dùng thực tế thay vì chỉ liệt kê một solution nghe hay. Tôi nhận ra việc khái quát đúng painpoint rồi chuyển thành hướng giải quyết khả thi khó hơn nhiều so với việc nghĩ ra một tính năng. Với FreshBox, điểm quan trọng không phải nhồi nhiều sensor mà là ghi nhận đúng từng batch mà không bắt người dùng nhập liệu nhiều. Tôi học được rằng workflow, metric và boundary phải đi cùng nhau thì mới biết AI có thực sự cần thiết hay không. Tôi cũng thấy các case chính thức trên thị trường giúp nhóm tránh suy nghĩ trong chân không, nhưng không thay thế được phỏng vấn hoặc số đo baseline. Nếu làm lại, tôi sẽ chuẩn bị dữ liệu và ngữ cảnh kỹ hơn, đặc biệt là tần suất pain, chi phí đầu tư và hậu quả khi hệ thống nhận diện sai. Tôi sẽ dành thêm thời gian để kiểm tra rủi ro và xác định rõ ai là người chịu trách nhiệm sửa khi tự động hóa không hoạt động.

## 4. Tự kiểm cuối bài

- [x] Cá nhân có 5+ problems và top 3 Problem Cards.
- [x] Đã pitch FreshBox và chuẩn bị câu hỏi challenge.
- [x] Reflection có vai trò, cách dùng AI, bài học và điều muốn làm khác.
- [x] Đã bổ sung tên nhóm và candidate FreshBox.
- [ ] Nên bổ sung thêm số đo thời gian di chuyển mỗi ngày và thời gian làm thủ tục vào phần evidence nếu muốn chi tiết hơn.
