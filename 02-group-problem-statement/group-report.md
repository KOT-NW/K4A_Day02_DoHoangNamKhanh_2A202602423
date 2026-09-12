# 02 — Group Problem Statement (Bản nộp nhóm)

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm |
|---|---|---:|---|
| 1 | Phạm Minh Cương | 2825 | Facilitator / tổng hợp candidate |
| 2 | Nguyễn Anh Trí | 2730 | Workflow / kỹ thuật |
| 3 | Đỗ Hoàng Nam Khánh | 2423 | Research / validation FreshBox |
| 4 | Võ Đức Trí | 2603 | Research / validation đô thị |
| 5 | Lê Châu Trần Phát | 2545 | Writer / Problem Statement |

> Vai trò trên là bản phân công dự kiến để hoàn thiện artifact; nhóm có thể chỉnh lại theo phân công thực tế.

**Candidate problem nhóm chọn:** FreshBox — giúp gia đình biết trong tủ lạnh đang có gì, từng batch được cất từ khi nào và món nào nên dùng trước.

---

## Phase 3 — Group Convergence

### 3.1. Các candidate được trình bày

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn |
|---:|---|---|---|---|
| 1 | Phạm Minh Cương | Quên thực phẩm và nhầm batch trong tủ lạnh | Hộ gia đình | Không có timestamp/ID, đồ cũ bị che |
| 2 | Phạm Minh Cương | Hỗ trợ khai báo thủ tục thuế | Cá nhân, hộ kinh doanh nhỏ | Không biết bắt đầu và sợ khai sai |
| 3 | Phạm Minh Cương | Miss thông tin sinh viên trên nhiều nền tảng | Sinh viên | Thông báo, deadline, tài liệu bị phân tán |
| 4 | Nguyễn Anh Trí | Check file code trước khi push cho senior | Intern/developer | Lỗi format, test hoặc thiếu checklist |
| 5 | Nguyễn Anh Trí | FreshBox theo dõi tồn kho thực phẩm | Gia đình | Nhập liệu thủ công và không biết FIFO |
| 6 | Nguyễn Anh Trí | App hỗ trợ khai thuế theo checklist | Người mới làm thủ tục | Thuật ngữ và giấy tờ khó hiểu |
| 7 | Võ Đức Trí | Xe điện xanh SM khó tìm khách tối ưu | Tài xế SM | Phân bổ cuốc và vị trí chờ chưa tối ưu |
| 8 | Võ Đức Trí | Tracking dữ liệu xe khách trong thành phố | Đơn vị vận hành/đô thị | Dữ liệu vị trí phân tán, khó xem tổng thể |
| 9 | Võ Đức Trí | Trung tâm nhắc thông tin sinh viên | Sinh viên | Bỏ sót thông báo quan trọng |
| 10 | Lê Châu Trần Phát | Tìm thợ sửa điện/nước uy tín | Người thuê trọ/hộ gia đình | Thiếu hồ sơ, review và bảo hành đáng tin |
| 11 | Lê Châu Trần Phát | So sánh báo giá sửa chữa | Khách hàng sửa đồ | Báo giá miệng, dễ phát sinh |
| 12 | Lê Châu Trần Phát | FreshBox giảm food waste | Gia đình | Không biết món nào cũ hơn |
| 13 | Đỗ Hoàng Nam Khánh | Đăng ký tạm trú online mất nhiều thời gian | Sinh viên/người thuê trọ | Hồ sơ, bước nộp và trạng thái khó theo dõi; trải nghiệm gần nhất mất khoảng 3 tuần |
| 14 | Đỗ Hoàng Nam Khánh | Di chuyển xa đi làm ảnh hưởng thời gian học/nghỉ | Intern, sinh viên năm cuối | Di chuyển khoảng 28 km mỗi ngày |
| 15 | Đỗ Hoàng Nam Khánh | FreshBox ghi nhận batch thực phẩm tự động | Gia đình | Không có timestamp và FIFO, đồ cũ dễ bị quên |

### 3.2. Gom trùng / cluster

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| A — Quản lý đồ dùng gia đình | 1, 5, 12, 15, 10, 11 | Người dùng thiếu thông tin đáng tin để quyết định trong đời sống | FreshBox có actor và workflow dễ quan sát nhất |
| B — Thủ tục và thông tin cá nhân | 2, 3, 6, 9, 13 | Thông tin/biểu mẫu phân tán, người dùng sợ bỏ sót hoặc làm sai | Cần dữ liệu quy định và quyền truy cập |
| C — Chất lượng đầu ra kỹ thuật | 4 | Cần checklist trước khi bàn giao code | Workflow khá thẳng, có thể giải bằng rule |
| D — Di chuyển và dữ liệu đô thị | 7, 8, 14 | Thiếu dữ liệu thời gian thực hoặc lộ trình tối ưu để ghép nhu cầu và phương tiện | Phụ thuộc API, dữ liệu thành phố và quyền riêng tư |

### 3.3. Shortlist

| Candidate | Vì sao vào shortlist | Rủi ro / điều chưa rõ |
|---|---|---|
| FreshBox | Gần đời sống; batch/FIFO tạo pain cụ thể; có thể prototype bằng rack, ID, timestamp và weight. | Cần kiểm chứng food waste và mức chấp nhận thao tác của người dùng. |
| Trung tâm thông tin sinh viên | Pain “miss thông tin” lặp lại; có thể gom thông báo, deadline và tài liệu vào một nơi. | Phải tích hợp nhiều nền tảng; khó xác định nguồn chính thức và quyền truy cập. |
| Hỗ trợ khai báo thuế theo checklist | Pain có hậu quả rõ nếu sai; có thể làm hướng dẫn theo ngữ cảnh. | Quy định thay đổi; không được để hệ thống tự kết luận nghĩa vụ thuế. |

### 3.4. Score để đồng thuận (1–5)

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| FreshBox | 5 | 5 | 4 | 5 | 5 | 5 | 5 | **34/35** |
| Trung tâm thông tin sinh viên | 5 | 4 | 4 | 4 | 4 | 5 | 4 | **30/35** |
| Hỗ trợ khai báo thuế | 4 | 4 | 3 | 5 | 3 | 4 | 3 | **26/35** |

**Candidate nhóm chọn:** FreshBox.

**Vì sao chọn:** FreshBox có actor cụ thể là hộ gia đình và workflow đặt thực phẩm vào tủ có thể vẽ rõ. Pain không chỉ là “không biết còn gì” mà là không phân biệt được các batch giống nhau và không thực hiện FIFO. Prototype có thể bắt đầu nhỏ bằng container ID, timestamp, cân nặng và rule FIFO. Nhóm cũng có thể đo forgotten-item rate, food waste và thời gian thêm item mà không cần xây Agent ngay.

**Vì sao không chọn các candidate còn lại:** Trung tâm thông tin sinh viên có pain rộng nhưng chưa đủ sâu về một workflow duy nhất; nhóm chưa có log thông báo bị bỏ sót để làm baseline. Hỗ trợ khai báo thuế có hậu quả và rủi ro pháp lý cao, đồng thời đã có eTax Mobile; cần nghiên cứu quy định sâu hơn trước khi quyết định build. Các bài toán tracking xe đô thị/SM phụ thuộc dữ liệu nền tảng, API và quyền riêng tư nên chưa phù hợp thời lượng lab.

**Disagreement:** Một số thành viên muốn chọn bài toán thông tin sinh viên hoặc xe SM vì có vẻ dễ làm app. Nhóm chốt FreshBox vì pain gần đời sống hơn, có boundary rõ và có thể thử prototype không cần dữ liệu bên thứ ba.

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation

Nhóm đã phỏng vấn **2 nhóm** về các candidate khác: (1) hỗ trợ khai báo thủ tục thuế và (2) app tracking dữ liệu xe khách di chuyển trong thành phố.

| Nguồn | Số người / mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Phỏng vấn nhóm 1 — thủ tục thuế | 1 nhóm người thường tự làm thủ tục | **Tóm tắt/paraphrase từ ghi chú:** người mới thường không biết bắt đầu từ bước nào, sợ thiếu giấy tờ hoặc khai sai. **Chưa có câu quote nguyên văn trong dữ liệu được cung cấp; cần thay bằng quote thật trước khi nộp.** | eTax Mobile và cổng thuế điện tử đã có tra cứu/nộp thuế, nên không nên xây lại toàn bộ hệ thống. | Thu hẹp thành checklist/hướng dẫn theo ngữ cảnh, có link về nguồn chính thức; không tự quyết định số thuế. |
| Phỏng vấn nhóm 2 — tracking xe | 1 nhóm quan tâm vận hành/di chuyển | **Tóm tắt/paraphrase:** cần xem vị trí, lộ trình và tình trạng xe trên một màn hình để phát hiện chậm trễ. **Chưa có câu quote nguyên văn; cần thay bằng quote thật trước khi nộp.** | Dữ liệu phương tiện có thể nhạy cảm; thành phố đã có cổng giao thông và các hệ thống giám sát riêng. | Thu hẹp thành dashboard tổng hợp dữ liệu đã được phép chia sẻ, không theo dõi cá nhân ngoài mục đích vận hành. |

**Insight sau validation:** Hai candidate đều có pain, nhưng nguồn dữ liệu/quyền truy cập và rủi ro pháp lý làm scope lớn. Với FreshBox, nhóm vẫn cần phỏng vấn hộ gia đình để xác nhận forgotten-item rate; research hiện tại chỉ hỗ trợ hình thành giả thuyết.

### 4.2. Research giải pháp đã có

| Nguồn / tool / case | Link | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| eTax Mobile — Cục Thuế | [Cục Thuế](https://gdt.gov.vn/) | Đăng ký tài khoản, tra cứu nghĩa vụ, nộp thuế. | Nguồn chính thức, chức năng rõ. | Không thay người dùng hiểu hoàn cảnh riêng; quy định thay đổi. | FreshBox cũng nên hỗ trợ workflow cụ thể, không tuyên bố quyết định thay người dùng. |
| Cổng giao thông TP.HCM | [Cổng giao thông](https://giaothong.hochiminhcity.gov.vn/Userguide/) | Hiển thị tình hình giao thông và tìm đường. | Có bản đồ, tuyến và tình trạng giao thông. | Phụ thuộc dữ liệu thành phố; không phải dashboard vận hành xe riêng. | Cần xác định rõ data owner và chỉ dùng dữ liệu được phép. |
| V-Tracking / giám sát phương tiện | [VNTT](https://vntt.com.vn/giam-sat-phuong-tien/) | Tập trung dữ liệu phương tiện trên bản đồ số để giám sát. | Có hướng tiếp cận ITS, bản đồ và dữ liệu lớn. | Không giải quyết trực tiếp bài toán FreshBox; dữ liệu thiết bị và quyền riêng tư là rào cản. | Không chọn bài toán đòi hỏi tích hợp dữ liệu bên ngoài trong MVP FreshBox. |
| Rada / Fixago — nền tảng gọi thợ | [Rada](https://apps.apple.com/vn/app/rada-service-around/id1064891644), [Fixago](https://www.fixago.vn/en/about) | Tìm thợ gần, xem review và đặt dịch vụ. | Cho thấy pattern hồ sơ, rating và kết nối theo vị trí. | Chất lượng review và giá vẫn cần kiểm chứng. | Với mỗi solution cần chứng minh bước workflow, không chỉ liệt kê tính năng. |

**Research takeaway:** Những hệ thống hiện có thường tập trung vào một workflow rõ và dữ liệu cụ thể. Với FreshBox, nên build MVP cho inventory awareness, batch tracking, timestamp, weight và FIFO; chưa nên build camera AI, gas sensor hay freshness estimation ngay.

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow

~~~text
[Mua/nhận thực phẩm: 10–30'] → [Chia vào túi/hộp: 5–15']
→ [Đặt vào ngăn bất kỳ: 1–3'] → [Tự nhớ ngày/batch: không có bước ghi]
→ [Đồ mới che đồ cũ] → [Kiểm tra muộn / bỏ đi]
~~~

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---|---|---|---|---|---|
| 1 | Người mua | Thực phẩm mới | Đồ mang về | 10–30 phút, mỗi lần mua | Có thể nhận thêm ngoài kế hoạch |
| 2 | Người trong nhà | Thực phẩm, túi/hộp | Các phần thực phẩm | 5–15 phút | Thường không có ID/batch |
| 3 | Người trong nhà | Hộp/túi | Đồ đặt trong tủ | 1–3 phút | Vị trí không cố định |
| 4 | Người trong nhà | Trí nhớ | Ước lượng inventory | Không ổn định | **Bottleneck:** mất timestamp và batch |
| 5 | Người trong nhà | Đồ mới | Tủ nhiều lớp | Mỗi lần thêm đồ | Đồ cũ bị che |
| 6 | Người nấu ăn | Inventory thực tế | Món được lấy | Mỗi bữa | Có thể lấy batch mới trước |
| 7 | Người trong nhà | Đồ quá lâu/không rõ ngày | Bỏ hoặc kiểm tra lại | Hàng tuần | Food waste và mua trùng |

### 5.2. Future workflow

~~~text
[Đặt hộp vào Smart Rack: <5'] → [Sensor đọc ID + timestamp: tự động]
→ [Load cell theo dõi khối lượng: tự động] → [Rule xếp FIFO]
→ [LED/App nhắc batch cũ] → [Người dùng xác nhận loại thực phẩm: ≤1 action]
→ [Lấy ra/đặt lại, hệ thống cập nhật trạng thái]
Fallback: nếu sensor/ID sai, người dùng sửa bằng app hoặc nhãn ngày thủ công.
~~~

**Before/after impact:**

| Metric | Trước | Sau kỳ vọng | Cách đo |
|---|---:|---:|---|
| Forgotten item rate | Chưa có baseline; giả định xảy ra hầu như mỗi tuần | Giảm ≥50% | Kiểm kê trước/sau pilot |
| Thời gian ghi nhận item | Không ghi hoặc nhớ thủ công | <5 giây/item, ≤1 xác nhận | Bấm giờ |
| Batch tracking accuracy | Không phân biệt ổn định | ≥90% | Đối chiếu log rack với kiểm kê |
| Food waste | Chưa có baseline | Giảm ≥30% | Cân/ghi món bỏ mỗi tuần |
| Risk mới | Quên, nhầm batch | Sensor/ID sai, lỗi kết nối | Ghi lỗi và tỷ lệ false alert |

### 5.3. Problem Statement v0

| Field | Nội dung |
|---|---|
| Actor | Hộ gia đình 2–5 người, người mua và cất thực phẩm. |
| Workflow | Mua/nhận → chia vào hộp/túi → đặt vào tủ → dựa vào trí nhớ → lấy món bất kỳ → có thể bỏ quên. |
| Bottleneck | Không có thông tin batch, timestamp và trạng thái khối lượng tại thời điểm cất. |
| Impact | Đồ cũ bị che, khó thực hiện FIFO, mua trùng và tăng food waste. |
| Success Metric | Giảm forgotten-item rate và food waste; giảm thời gian ghi nhận item. |
| Boundary | Tập trung inventory awareness, batch tracking, storage history và consumption priority; không xác định an toàn tuyệt đối. |

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp

- Độ mơ hồ: **Trung bình/thấp** — thứ tự batch và cảnh báo FIFO có tiêu chí tương đối rõ.
- Độ phức tạp: **Cao vừa phải** — có sensor, ID, weight, app và bước xác nhận người dùng nhưng flow chính vẫn tuyến tính.
- **Bài toán nằm ở ô:** Workflow có Rule hỗ trợ, chưa cần Agent.

### 6.1. So sánh Rule / Workflow / Agent

| Mức | Phương án | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| Rule | Nếu batch cũ hơn hoặc khối lượng gần 0 thì bật LED/cập nhật trạng thái. | Đủ cho FIFO, empty và cảnh báo cơ bản. | Không hiểu mô tả tự nhiên, không xử lý ngoại lệ tốt. | Có, cho logic FIFO/trạng thái. |
| Workflow | Sensor → ghi log → app → rule ưu tiên → người dùng xác nhận. | Đủ cho MVP vì các bước đi theo một flow. | Lỗi sensor/kết nối, cần human review. | **Chọn cho MVP.** |
| Agent | Tự lập kế hoạch, nhận diện món, gọi nhiều tool và đề xuất thực đơn. | Chỉ đáng cân nhắc khi đã có dữ liệu lớn và nhiều ngoại lệ. | Scope lớn, khó kiểm chứng, AI nhận diện sai. | Chưa chọn. |

1. **Rule có giải được 70–80% case không?** Có, với timestamp, FIFO, cảnh báo khối lượng và trạng thái hộp.
2. **Các bước có đi thẳng không?** Có; ngoại lệ chính là sensor sai hoặc hộp không có ID.
3. **Có thật sự cần Agent không?** Chưa; MVP chưa cần tự lập kế hoạch nhiều bước.
4. **Nếu AI/sensor sai, ai phát hiện?** Người dùng kiểm tra trên app/rack và sửa bằng nhãn ngày hoặc chỉnh log.
5. **Có hạ từ Agent → Workflow → Rule được không?** Có; bản đầu có thể chạy bằng workflow bán thủ công và rule.

**Mức chọn:** Workflow + Rule

**Vì sao chọn:** Bài toán có flow khá ổn định và cần kết nối sensor, log, app, LED với một số rule. Workflow giúp kiểm soát handoff và human boundary; Rule xử lý FIFO minh bạch, dễ kiểm thử. Agent chưa tạo thêm giá trị tương xứng với rủi ro và chi phí ở MVP.

**Vì sao không chọn mức đơn giản hơn:** Chỉ dùng Rule không đủ để kết nối phát hiện vật, container ID, cân nặng, app và xác nhận của người dùng. Tuy nhiên nhóm vẫn giữ Rule làm lõi để có thể hạ scope nếu phần cứng chưa ổn định.

### 6.2. Problem Statement v1

| Field | Nội dung |
|---|---|
| Actor | Hộ gia đình 2–5 người; người mua, chia và cất thực phẩm. |
| Workflow | Khi hộp được đặt vào Smart Rack, hệ thống nhận ID và timestamp, theo dõi khối lượng, xếp batch theo FIFO và nhắc người dùng dùng batch cũ trước. |
| Bottleneck | Ghi nhận thủ công không bền vững và không phân biệt được các batch cùng loại thực phẩm. |
| Impact | Quên đồ, mua trùng, lấy batch mới trước và phải bỏ thực phẩm cũ. |
| Success Metric | Sau pilot, forgotten-item rate giảm ≥50%, food waste giảm ≥30%, add/remove detection ≥95%, batch accuracy ≥90%, thao tác thêm item <5 giây. |
| Boundary (làm / không làm) | Làm: ID hộp, timestamp, weight, temperature cơ bản, FIFO, LED/app reminder. Không làm trong MVP: khẳng định thực phẩm an toàn, phát hiện pathogen, camera AI phức tạp, gas sensor, freshness AI. |
| AI intervention point | Nếu có AI, chỉ hỗ trợ sau khi log/sensor ghi nhận và trước bước người dùng xác nhận loại thực phẩm; không tự quyết định thực phẩm an toàn. |
| Mức chọn | Workflow + Rule vì flow tuyến tính, có thể kiểm thử và có human review. |
| Rủi ro & người thật kiểm tra | Sensor/ID sai hoặc cảnh báo sai; người dùng kiểm tra hộp trên rack/app, sửa log thủ công và nhóm theo dõi false-alert rate. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú |
|---|---|---|
| Actor + workflow rõ chưa? | Yes | Hộ gia đình và flow batch đã xác định. |
| Baseline + metric đo được chưa? | Not Yet | Cần baseline 7 ngày trước pilot về forgotten item và food waste. |
| Data/input đủ dùng chưa? | Not Yet | Có thể bắt đầu bằng dữ liệu mẫu và log bán thủ công; chưa có sensor thật. |
| AI sai, hậu quả chấp nhận được không? | Yes, có điều kiện | Không dùng AI để kết luận an toàn; người dùng luôn xác nhận. |
| Có người review/owner không? | Yes | Người dùng sửa batch; nhóm theo dõi log và lỗi. |
| Có cách non-AI đơn giản hơn không? | Yes | Nhãn ngày + bảng FIFO là fallback; vẫn cần workflow để kiểm chứng giá trị tự động hóa. |

**Decision: Go với scope nhỏ.**

**Lý do:** FreshBox có actor, workflow và painpoint cụ thể; prototype có thể chạy bán thủ công trước khi đầu tư phần cứng đầy đủ. Nhóm chọn Go để kiểm chứng giả thuyết tự động ghi nhận inventory có giảm quên đồ hay không. Quyết định này có điều kiện: phải đo baseline và không tuyên bố freshness/safety vượt quá dữ liệu.

**Pilot nhỏ nhất:** Chọn 2–3 hộ gia đình trong 7 ngày baseline và 14 ngày prototype. Dùng 3–5 hộp có QR/ID, một cân/load cell mẫu và bảng log timestamp/weight; có thể nhập thủ công thay sensor ở vòng đầu. Đo ba số: forgotten-item rate, food waste gram/tuần và thời gian thêm item.

**Exit / rollback:** Nếu người dùng phải sửa hơn 20% log, false alert cao hoặc registration vượt 5 giây/item, quay về nhãn ngày + bảng FIFO. Nếu hệ thống đưa ra claim an toàn thực phẩm hoặc mất dữ liệu batch, dừng tính năng đó và chỉ giữ inventory log thủ công.

### Self-check nộp phần 02

- [x] Có nhật ký hội tụ 15 candidate → 1, cluster, shortlist và score.
- [ ] Validation có paraphrase nhưng cần bổ sung quote nguyên văn từ 2 nhóm phỏng vấn.
- [x] Có research và link kiểm được.
- [x] Có workflow trước/sau, thời gian, bottleneck, boundary và fallback.
- [x] Có PS v0 → v1, metric trước/sau và cách đo.
- [x] Có so sánh Rule/Workflow/Agent và quyết định Go có pilot/rollback.

