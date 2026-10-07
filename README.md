# Lab 21 — Phân tích rủi ro AI qua case study thực tế

- Họ và tên: Nguyễn Thị Phương Duyên
- MSSV / mã học viên: 2A202603001
- Lớp: Track1_H201
- Ngành đã chọn: Social Media

### 1. Industry Risk Snapshot

| Nội dung | Đánh giá của tôi và lý do |
| --- | --- |
| Những tác hại chính có thể xảy ra | **Thông tin sai lệch và nội dung độc hại:** thuật toán đề xuất có thể khuếch đại nội dung gây hại, đặc biệt với trẻ em và người dùng dễ tổn thương. **Lừa đảo tài chính:** Deepfake/DeepVoice có thể giả danh người thân hoặc người quen để tạo lòng tin và yêu cầu chuyển tiền. **Xâm phạm quyền riêng tư, danh dự và nhân phẩm:** hình ảnh, khuôn mặt hoặc giọng nói của một người có thể bị AI sử dụng để tạo nội dung giả, kể cả hình ảnh/video nhạy cảm, nhằm bôi nhọ hoặc tống tiền. Người bị ảnh hưởng gồm người dùng mạng xã hội, trẻ vị thành niên, nạn nhân bị giả mạo, gia đình và các tổ chức có liên quan. |
| Mức độ high-stakes | **Cao.** Rủi ro không chỉ dừng ở việc người dùng nhìn thấy nội dung không chính xác mà có thể dẫn đến hậu quả thực tế như mất tiền, tổn hại sức khỏe tinh thần, bị đe dọa, ảnh hưởng danh dự và quyền riêng tư. Đặc biệt, với Deepfake, người dùng có thể khó nhận biết nội dung giả trước khi đưa ra quyết định hoặc trước khi nội dung đã lan truyền rộng. |
| Dữ liệu nhạy cảm có thể được sử dụng | Hình ảnh khuôn mặt, video cá nhân, mẫu giọng nói, thông tin nhận dạng, tài khoản mạng xã hội, danh sách bạn bè/người thân, lịch sử tương tác và hành vi xem nội dung. Trong các trường hợp nghiêm trọng còn có thể liên quan đến hình ảnh riêng tư hoặc dữ liệu sinh trắc học dùng để giả mạo danh tính. |
| Nhu cầu human review | **Cao.** Cần con người kiểm tra ở các điểm có khả năng gây hậu quả nghiêm trọng: nội dung bị hệ thống phát hiện là Deepfake hoặc giả mạo; nội dung nhạy cảm liên quan đến người thật; báo cáo về lừa đảo, tống tiền hoặc self-harm; và trước các quyết định khóa tài khoản/gỡ nội dung có ảnh hưởng lớn. Human reviewer cần xem xét ngữ cảnh, bằng chứng và mức độ nguy hiểm vì AI moderation có thể bỏ sót nội dung tinh vi hoặc gắn nhãn sai nội dung hợp pháp. |

### 2. Case study 1 — TikTok Việt Nam: thuật toán đề xuất và nội dung độc hại

#### Brief Case

- **Tổ chức / sản phẩm AI:** TikTok Pte. Ltd. (TikTok Singapore) — nền tảng TikTok, đặc biệt là hệ thống **recommendation / For You** và hệ thống kiểm duyệt nội dung tự động.

- **Thời gian, địa điểm / bối cảnh:** Việt Nam, tập trung vào giai đoạn **quý IV/2022 đến năm 2023**. Từ ngày **22/05/2023**, Bộ Thông tin và Truyền thông phối hợp với các bộ, ngành liên quan kiểm tra toàn diện hoạt động của TikTok tại Việt Nam; ngày **29/09/2023**, Bộ ban hành Kết luận kiểm tra số 08/KL-BTTTT.

- **AI được dùng để làm gì:** TikTok sử dụng thuật toán để phân phối và đề xuất video dựa trên **tương tác, sở thích và sự quan tâm của người dùng**. Nền tảng cũng sử dụng công nghệ tự động để kiểm tra nội dung dựa trên các yếu tố như hình ảnh, âm thanh, từ khóa, tiêu đề và mô tả.

- **Vấn đề hoặc sự kiện đáng chú ý:** Kết quả kiểm tra của Bộ TT&TT xác định quy trình kiểm duyệt của TikTok **chưa hiệu quả, để lọt nhiều nội dung vi phạm pháp luật Việt Nam**. Cơ quan quản lý cũng chỉ ra rằng cơ chế phân phối và đề xuất dựa trên tương tác, sở thích và sự quan tâm có thể khiến nội dung vi phạm lan truyền nhanh nếu nhận được nhiều tương tác. Ngoài ra còn tồn tại nội dung giả mạo, kích động bạo lực, gây hại cho trẻ em và vấn đề trẻ dưới 13 tuổi vẫn có thể mở tài khoản.

- **Số liệu có nguồn:** Trong **quý IV/2022**, TikTok đã xóa hơn **1,7 triệu video vi phạm tại Việt Nam**, trong đó **94,9% được nền tảng chủ động phát hiện và xóa**. Một khảo sát của VnExpress ngày 04/04/2023 có gần **9.500 người tham gia**; trong gần 6.000 người cho biết có sử dụng TikTok, **hơn 80% phản ánh thường xuyên tiếp xúc với nội dung độc hại**. Đây là khảo sát độc giả của VnExpress, không phải điều tra đại diện cho toàn bộ người dùng TikTok Việt Nam.

- **Nguồn:**
  - *TikTok kiểm duyệt nội dung tại Việt Nam thế nào* — VnExpress — 10/04/2023. [Mở bài VnExpress](https://vnexpress.net/tiktok-thue-hang-tram-nguoi-viet-kiem-duyet-noi-dung-4591509.html?utm_source=chatgpt.com)
  - *Bộ Thông tin và Truyền thông thông báo kết quả kiểm tra toàn diện hoạt động của TikTok tại Việt Nam* — cơ quan quản lý nhà nước — 05/10/2023. [Mở kết quả kiểm tra TikTok](https://www.abei.gov.vn/thong-tin-dien-tu/bo-thong-tin-va-truyen-thong-thong-bao-ket-qua-kiem-tra-toan-dien-hoat-dong-cua-tiktok-tai-viet-nam-/108209?utm_source=chatgpt.com)
  - *Kết quả kiểm tra toàn diện hoạt động của TikTok tại Việt Nam* — Báo Chính phủ. [Mở Báo Chính phủ](https://baochinhphu.vn/ket-qua-kiem-tra-toan-dien-hoat-dong-cua-tiktok-tai-viet-nam-102231005164335301.htm?utm_source=chatgpt.com)

- **Phân biệt bằng chứng và nhận định:** **Bằng chứng:** TikTok đã xóa hơn 1,7 triệu video vi phạm trong một quý; Bộ TT&TT kết luận cơ chế kiểm duyệt chưa hiệu quả và cơ chế đề xuất có khả năng làm nội dung vi phạm lan truyền nhanh. **Nhận định của tôi:** recommendation algorithm tạo ra một “feedback loop”, trong đó nội dung độc hại có tương tác cao có thể tiếp tục được phân phối tới nhiều người hơn. Tuy nhiên, các nguồn trên **không đủ để kết luận rằng thuật toán TikTok trực tiếp gây ra một hậu quả sức khỏe cụ thể đối với từng người dùng Việt Nam**.

#### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| **High-risk moment** | Khi người dùng, đặc biệt là trẻ em hoặc người dùng dễ bị tổn thương, xem hoặc tương tác với nội dung độc hại và hệ thống tiếp tục dùng tín hiệu tương tác đó để đề xuất thêm nội dung tương tự. |
| **Stakeholder bị ảnh hưởng** | Người dùng TikTok; trẻ em và thanh thiếu niên; phụ huynh; người sáng tạo nội dung; TikTok; cơ quan quản lý và cộng đồng xã hội. |
| **Failure mode** | **Harmful-content amplification / recommendation feedback loop:** nội dung vi phạm hoặc gây hại không được phát hiện kịp thời và có thể tiếp tục được thuật toán phân phối dựa trên tương tác. |
| **Layer bắt đầu lỗi** | **Safety**, có liên hệ với **Model/Recommendation**. Bằng chứng mạnh nhất là cơ chế kiểm duyệt chưa hiệu quả và kiểm soát đề xuất chưa ngăn được nội dung vi phạm lan truyền. Không đủ thông tin kỹ thuật để quy lỗi cho một mô hình ML cụ thể. |
| **Harm xảy ra là gì?** | **Đã xác nhận:** người dùng Việt Nam đã tiếp xúc với lượng lớn nội dung vi phạm/độc hại; cơ quan quản lý phát hiện các vấn đề liên quan đến nội dung gây hại cho trẻ em. **Nguy cơ:** tiếp xúc lặp lại có thể làm tăng misinformation, hành vi bắt chước nguy hiểm hoặc ảnh hưởng tâm lý của nhóm dễ tổn thương. |
| **Harm lens** | Information harm; child safety; psychological/social harm; misinformation amplification. |
| **Severity** | **High.** Không phải mọi video đều gây hậu quả nghiêm trọng, nhưng nền tảng có quy mô lớn và harm có thể liên quan trực tiếp tới trẻ em, misinformation và nội dung nguy hiểm. |
| **Scale** | **Large.** Chỉ trong Q4/2022 đã có hơn **1,7 triệu video vi phạm bị xóa tại Việt Nam**. Đây là số video bị xử lý, không phải số người bị hại. |
| **Probability** | **Medium–High.** Khảo sát VnExpress cho thấy hơn 80% trong gần 6.000 người dùng tham gia khảo sát nói thường xuyên gặp nội dung độc hại; tuy nhiên đây là khảo sát tự chọn nên không thể coi là tỷ lệ của toàn bộ dân số người dùng. |
| **Frequency** | **High.** Số lượng 1,7 triệu video bị xóa trong một quý và phản ánh “thường xuyên” gặp nội dung độc hại cho thấy vấn đề không phải sự kiện đơn lẻ. |
| **Vì sao?** | Đây là rủi ro ở quy mô nền tảng: một lỗi moderation chỉ tác động một video, nhưng recommendation có thể khuếch đại nó cho nhiều người. Tuy nhiên cần tránh kết luận rằng mọi nội dung bị xóa đều được thuật toán đề xuất hoặc rằng 1,7 triệu video tương đương 1,7 triệu nạn nhân. |

---

### 3. Case study 2 — Deepfake giả người thân qua video call khiến nạn nhân mất 30 triệu đồng

#### Brief Case

- **Tổ chức / sản phẩm AI:** Không xác định được nhà cung cấp công cụ Deepfake cụ thể. Công nghệ được sử dụng là **AI Deepfake tạo video/hình ảnh giả mạo khuôn mặt người thật**, kết hợp với tài khoản Facebook bị chiếm quyền sử dụng.

- **Thời gian, địa điểm / bối cảnh:** Tháng **8/2023**, nạn nhân là chị N.T.K., cư trú tại huyện Châu Thành, tỉnh Long An.

- **AI được dùng để làm gì:** Kẻ gian sử dụng Deepfake để thực hiện **cuộc gọi video giả danh một người bà con của nạn nhân ở nước ngoài**, sau khi đã chiếm quyền sử dụng tài khoản Facebook của người này. Mục tiêu là làm nạn nhân tin rằng mình đang giao tiếp với người thân thật.

- **Vấn đề hoặc sự kiện đáng chú ý:** Kẻ gian gọi video Deepfake giả người bà con và yêu cầu nạn nhân chuyển tiền. Để tăng độ tin cậy, đối tượng còn gửi thông báo giả rằng đã chuyển trả cho nạn nhân gần **100 triệu đồng**, nhưng tiền từ nước ngoài sẽ mất hai ngày mới đến. Nạn nhân tin lời và chuyển tiền.

- **Số liệu có nguồn:** Nạn nhân đã chuyển **30 triệu đồng** cho đối tượng. Một ngày sau, khi nhận được thông tin tài khoản Facebook của người bà con đã bị hack, nạn nhân mới biết mình bị lừa. Thông tin được đăng trên trang Công an địa phương.

- **Nguồn:**
  - *Lừa đảo cuộc gọi video Deepfake* — Công an địa phương — 27/08/2023. [Mở nguồn Công an](https://congan.tayninh.gov.vn/vi/chi-tiet-tin-tuc?Id=92698&utm_source=chatgpt.com)
  - *Cuộc gọi video Deepfake để lừa đảo ra sao?* — Bộ Thông tin và Truyền thông — 19/05/2023. [Mở nguồn Bộ TT&TT](https://mic.gov.vn/cuoc-goi-video-deepfake-de-lua-dao-ra-sao-197159128.htm?utm_source=chatgpt.com)
  - *Cẩm nang nhận diện và phòng tránh lừa đảo trực tuyến* — nguồn thuộc Bộ Công an, trong đó Deepfake video call được liệt kê là một hình thức lừa đảo trực tuyến.

- **Pháp lý liên quan:** Tại thời điểm hiện nay, **Luật An ninh mạng số 116/2025/QH15**, có hiệu lực từ 01/07/2026, đã quy định cấm sử dụng AI hoặc công nghệ mới để giả mạo video, hình ảnh, giọng nói của người khác trái pháp luật. Đây là quy định **hiện hành**, không nên dùng để nói rằng nó là căn cứ pháp lý đã áp dụng cho sự kiện năm 2023.

- **Phân biệt bằng chứng và nhận định:** **Bằng chứng:** cơ quan Công an ghi nhận nạn nhân mất 30 triệu đồng sau cuộc gọi video Deepfake giả người thân. **Nhận định:** Deepfake đóng vai trò như một “trust amplifier” — tăng độ thuyết phục của kịch bản social engineering. Không có thông tin công khai xác định công cụ AI cụ thể, mô hình nào được sử dụng hoặc dữ liệu huấn luyện của công cụ đó.

#### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| **High-risk moment** | Khi nạn nhân nhận cuộc gọi video có khuôn mặt giống người thân và ngay sau đó nhận yêu cầu chuyển tiền khẩn cấp. Hình ảnh quen thuộc khiến nạn nhân giảm mức độ nghi ngờ. |
| **Stakeholder bị ảnh hưởng** | Nạn nhân chuyển tiền; người có tài khoản/hình ảnh bị giả mạo; gia đình và người quen của chủ tài khoản; ngân hàng; nền tảng mạng xã hội. |
| **Failure mode** | **Identity impersonation bằng Deepfake + social engineering.** AI tạo tín hiệu nhận dạng giả đủ thuyết phục để kẻ xấu mạo danh người thật. |
| **Layer bắt đầu lỗi** | **Safety.** Đây không phải lỗi “AI trả lời sai” mà là công nghệ AI bị lạm dụng để giả danh. Ngoài ra có yếu tố **UX/authenticity** vì người nhận không có tín hiệu đáng tin cậy để biết video là synthetic. |
| **Harm xảy ra là gì?** | **Harm đã xảy ra:** một nạn nhân mất **30 triệu đồng**. Người thân cũng bị mạo danh sau khi tài khoản Facebook bị chiếm quyền. |
| **Harm lens** | Financial harm; identity/privacy harm; fraud; trust and information integrity. |
| **Severity** | **High.** Harm trực tiếp là mất tài sản và việc giả danh người thật có thể tiếp tục được sử dụng với nhiều người trong mạng lưới quan hệ của nạn nhân. |
| **Scale** | **Confirmed scale của case: 1 nạn nhân, 30 triệu đồng.** Không suy rộng con số này thành quy mô toàn quốc. Cơ quan chức năng xác nhận đây là một loại thủ đoạn đang được sử dụng rộng hơn, nhưng nguồn case không cung cấp tổng số nạn nhân toàn quốc. |
| **Probability** | **Medium.** Case cho thấy thủ đoạn có thể thành công trong thực tế, nhưng một case đơn lẻ không đủ để tính xác suất người dùng Việt Nam bị lừa. |
| **Frequency** | **Chưa đủ bằng chứng định lượng để chấm High.** Cơ quan chức năng đã nhiều lần cảnh báo về video Deepfake, nhưng nguồn không cung cấp số vụ Deepfake video-call toàn quốc trong một khoảng thời gian chuẩn hóa. |
| **Vì sao?** | Điểm nguy hiểm là AI làm giả một tín hiệu mà người dùng vốn xem là bằng chứng mạnh về danh tính: **khuôn mặt/video trực tiếp**. Tuy nhiên, cần phân biệt Deepfake với các vụ chỉ hack tài khoản hoặc giả danh bằng tin nhắn; không nên gộp toàn bộ lừa đảo online thành thiệt hại do Deepfake. |

---

### 4. Case study 3 — AI/Deepfake ghép ảnh nhạy cảm để tống tiền gần 1.000 người

#### Brief Case

- **Tổ chức / sản phẩm AI:** Không xác định một sản phẩm AI thương mại cụ thể. Các đối tượng sử dụng **AI/Deepfake** và công nghệ chỉnh sửa hình ảnh/video để tạo nội dung nhạy cảm giả từ hình ảnh của người thật.

- **Thời gian, địa điểm / bối cảnh:** Hoạt động được ghi nhận tại nhiều tỉnh, thành ở Việt Nam. Một nhánh điều tra tại Bắc Giang xác định dòng tiền trong giai đoạn **tháng 8–10/2024**; đến tháng **4/2025**, cơ quan Công an công bố việc điều tra, bắt giữ và mở rộng vụ án.

- **AI được dùng để làm gì:** Các đối tượng thu thập hình ảnh và thông tin cá nhân, đặc biệt của doanh nhân, cán bộ, người có địa vị xã hội; sau đó sử dụng **AI/Deepfake để ghép khuôn mặt vào hình ảnh hoặc video nhạy cảm**, gửi cho nạn nhân và đe dọa sẽ phát tán cho gia đình, cơ quan hoặc mạng xã hội nếu không chuyển tiền.

- **Vấn đề hoặc sự kiện đáng chú ý:** Ngày 25/04/2025, thông tin từ Bộ Công an được báo chí dẫn cho biết Cục Cảnh sát hình sự đã phát hiện và điều tra đường dây có yếu tố nước ngoài sử dụng AI/Deepfake tạo hình ảnh nhạy cảm để đe dọa doanh nhân, cán bộ và người có điều kiện kinh tế. Vụ án liên quan đến hành vi **cưỡng đoạt tài sản và rửa tiền**.

- **Số liệu có nguồn:** Theo thông tin điều tra được công bố, **gần 1.000 bị hại trên cả nước** có liên quan; tại nhánh điều tra Bắc Giang, ba đối tượng đã đứng tên lập **71 tài khoản ngân hàng**, thực hiện việc quét sinh trắc học khuôn mặt và luân chuyển tổng số tiền chiếm đoạt của gần 1.000 bị hại khoảng **200 tỷ đồng** trong giai đoạn tháng 8–10/2024. Mỗi trong ba đối tượng này được xác định hưởng lợi bất chính khoảng **80 triệu đồng**.

- **Nguồn:**
  - *Dùng AI ghép ảnh nhạy cảm tống tiền doanh nhân, công chức: Gần 1.000 người sập bẫy* — VTV — 25/04/2025, dẫn thông tin Bộ Công an. [Mở bài VTV](https://vtv.vn/phap-luat/dung-ai-ghep-anh-nhay-cam-tong-tien-doanh-nhan-cong-chuc-gan-1000-nguoi-sap-bay-20250425210351993.htm?utm_source=chatgpt.com)
  - *Doanh nhân, công chức bị cắt ghép hình ảnh, video nhạy cảm để tống tiền* — Tuổi Trẻ — 25/04/2025, dẫn thông tin Bộ Công an. [Mở bài Tuổi Trẻ](https://tuoitre.vn/doanh-nhan-cong-chuc-bi-cat-ghep-hinh-anh-video-nhay-cam-de-tong-tien-20250425205756996.htm?utm_source=chatgpt.com)
  - *Bắc Giang: Bắt nhóm đối tượng trong đường dây cắt, ghép tạo hình ảnh nhạy cảm để lừa đảo chiếm đoạt tài sản* — Báo Bắc Giang, nguồn Công an tỉnh. [Mở Báo Bắc Giang](https://baobacgiang.vn/bac-giang-bat-nhom-doi-tuong-trong-duong-day-cat-ghep-tao-hinh-anh-nhay-cam-de-lua-dao-chiem-doat-tai-san-postid416912.bbg?utm_source=chatgpt.com)
  - *Dùng AI ghép hình ảnh nhạy cảm để tống tiền* — Tuổi Trẻ — 17/03/2025, mô tả trường hợp thực tế và cách Deepfake được sử dụng. [Mở bài Tuổi Trẻ về Deepfake nhạy cảm](https://tuoitre.vn/dung-ai-ghep-hinh-anh-nhay-cam-de-tong-tien-20250317075948373.htm?utm_source=chatgpt.com)

- **Pháp lý liên quan:**
  - Vụ án được cơ quan chức năng điều tra theo các hành vi liên quan **cưỡng đoạt tài sản/rửa tiền**; tại một nhánh khác, ba bị can bị điều tra về **lừa đảo chiếm đoạt tài sản**.
  - **Luật Bảo vệ dữ liệu cá nhân số 91/2025/QH15** được ban hành ngày 26/06/2025 và có hiệu lực từ **01/01/2026**, thiết lập khung pháp luật hiện hành về bảo vệ dữ liệu cá nhân.
  - Trước đó, Nghị định **13/2023/NĐ-CP** xác định dữ liệu cá nhân gồm **hình ảnh của cá nhân**, thông tin tài khoản số và lịch sử hoạt động trên không gian mạng; dữ liệu về đặc điểm sinh học riêng có thể thuộc dữ liệu nhạy cảm.
  - Luật An ninh mạng hiện hành số **116/2025/QH15** bổ sung quy định cấm sử dụng AI/công nghệ mới để làm giả video, hình ảnh, giọng nói người khác trái pháp luật.

- **Phân biệt bằng chứng và nhận định:** **Bằng chứng:** cơ quan chức năng xác nhận tồn tại đường dây sử dụng AI/Deepfake tạo nội dung nhạy cảm để đe dọa, chiếm đoạt tài sản; gần 1.000 bị hại và khoảng 200 tỷ đồng xuất hiện trong kết quả điều tra được công bố. **Nhận định:** AI đã làm giảm mạnh chi phí và kỹ năng cần thiết để tạo synthetic sexual content đủ thuyết phục để đe dọa nạn nhân. Không có bằng chứng công khai xác định một model AI hay nhà cung cấp AI cụ thể chịu trách nhiệm cho toàn bộ nội dung của đường dây.

#### Harm Map Worksheet

| Trường | Phân tích của tôi |
| --- | --- |
| **High-risk moment** | Khi kẻ xấu lấy hình ảnh thật của nạn nhân trên mạng xã hội, tạo ảnh/video nhạy cảm giả bằng AI rồi gửi trực tiếp cho nạn nhân kèm lời đe dọa sẽ phát tán cho gia đình, đồng nghiệp hoặc công chúng nếu không chuyển tiền. |
| **Stakeholder bị ảnh hưởng** | Nạn nhân bị ghép mặt; gia đình; đồng nghiệp/cơ quan; doanh nghiệp; ngân hàng; nền tảng mạng xã hội; cơ quan thực thi pháp luật. |
| **Failure mode** | **Non-consensual synthetic sexual content + identity impersonation + extortion.** AI tạo nội dung giả mang danh tính của người thật mà không có sự đồng ý. |
| **Layer bắt đầu lỗi** | **Safety.** Đây chủ yếu là AI misuse: công nghệ tạo/chỉnh sửa nội dung có thể bị sử dụng để tạo nội dung tình dục giả về người thật. **UX** cũng góp phần khi người nhận nội dung không có cơ chế dễ dàng xác thực thật/giả. Không đủ dữ liệu để quy lỗi cho một model cụ thể. |
| **Harm xảy ra là gì?** | **Đã xảy ra:** nạn nhân bị đe dọa, tống tiền và có người đã mất tiền; điều tra ghi nhận gần 1.000 bị hại và khoảng 200 tỷ đồng liên quan đến số tiền bị chiếm đoạt/luân chuyển. Ngoài thiệt hại tài chính còn có nguy cơ tổn hại danh dự, đời tư, tâm lý và nghề nghiệp. |
| **Harm lens** | Financial harm; privacy violation; dignity/reputational harm; non-consensual sexual imagery; psychological harm; identity abuse. |
| **Severity** | **Critical.** Harm đồng thời tác động đến tiền bạc, danh dự, đời tư và sức khỏe tâm lý; quy mô đã vượt khỏi một sự cố cá nhân và trở thành hoạt động có tổ chức. |
| **Scale** | **Very large:** gần **1.000 bị hại trên cả nước** và khoảng **200 tỷ đồng** được cơ quan điều tra ghi nhận trong dòng tiền liên quan. |
| **Probability** | **Medium–High đối với nhóm mục tiêu.** Cơ quan chức năng ghi nhận các đối tượng chủ động thu thập thông tin, hình ảnh của doanh nhân, cán bộ và người có địa vị/điều kiện kinh tế để lựa chọn nạn nhân. Không có đủ dữ liệu để tính xác suất cho toàn bộ người dùng mạng xã hội Việt Nam. |
| **Frequency** | **High trong phạm vi đường dây.** Gần 1.000 bị hại trong hoạt động có tổ chức cho thấy hành vi được lặp lại có hệ thống chứ không phải một sự cố đơn lẻ. |
| **Vì sao?** | AI không chỉ tạo misinformation mà trở thành **công cụ tạo bằng chứng giả để cưỡng ép hành vi thực tế**. Người bị hại thậm chí không cần tin video là thật: chỉ cần lo rằng gia đình, đồng nghiệp hoặc công chúng có thể tin nội dung giả, kẻ xấu đã có đòn bẩy để tống tiền. |

