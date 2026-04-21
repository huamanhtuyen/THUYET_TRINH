# 🌐 Nghiên Cứu: Tình Hình Triển Khai No-Code / Low-Code Trên Thế Giới
> Cập nhật: Tháng 4/2026 | Nguồn: Gartner, Forrester, OutSystems, Mendix, Appsmith, McKinsey

---

## 1. 📊 Tổng Quan Thị Trường Toàn Cầu

### Quy mô & Tốc độ tăng trưởng

| Chỉ số | Số liệu |
|---|---|
| Quy mô thị trường LCNC (2024) | ~$30–45 tỷ USD (tuỳ phạm vi định nghĩa) |
| Dự báo đến 2028 (Forrester) | $30–50 tỷ USD (bao gồm AI acceleration) |
| Dự báo dài hạn đến 2030 | $100–180 tỷ USD |
| % ứng dụng mới dùng LCNC vào 2025–2026 (Gartner) | **70–75%** |
| % ứng dụng mission-critical dùng LCNC vào 2029 | **80%** (dự báo Gartner) |
| Rút ngắn thời gian phát triển | **50–90%** so với code truyền thống |

### Xu hướng chính 2024–2025
- **AI tích hợp vào LCNC**: Copilot, AI Agents được nhúng vào các nền tảng (Power Apps Copilot, OutSystems AI Mentor…)
- **Citizen Developer bùng nổ**: ~41% nhân viên doanh nghiệp có thể xây dựng ứng dụng mà không cần IT
- **Mission-Critical dịch chuyển**: Không còn chỉ dùng cho tool nội bộ nhỏ — xu hướng dùng cho hệ thống cốt lõi

---

## 2. 🏛️ Bức Tranh Khu Vực: Đông Nam Á & Việt Nam

### Chính phủ Việt Nam và Chuyển đổi Số
- **Quyết định 749/QĐ-TTg** – Chương trình CĐS quốc gia đến 2025 (tầm nhìn 2030):
  - 80% dịch vụ công trực tuyến cấp độ 4
  - 100% hồ sơ quản lý nhà nước được số hóa
- **Luật Chuyển đổi số** (dự kiến thông qua cuối 2025) — mở đường pháp lý cho các công nghệ tiên tiến
- **Nhu cầu thực tế**: Cần triển khai nhanh ở cấp bộ, tỉnh, huyện với ngân sách hạn chế → LCNC là lựa chọn phù hợp

### Case Study Khu vực Đông Nam Á
| Quốc gia | Đơn vị | Nền tảng | Kết quả |
|---|---|---|---|
| Malaysia | MDEC | OutSystems | Hợp nhất 50+ hệ thống legacy → 2 nền tảng agile; giảm 50% technical debt |
| Nhiều nước ASEAN | Chính phủ | Microsoft Power Apps | Quản lý nông nghiệp, giấy phép, hạ tầng giao thông |
| Toàn cầu | Khu vực công | Mendix | Cổng dịch vụ công dân, đăng ký hộ tịch, hệ thống cứu hỏa |

---

## 3. 🔑 Phân Tích Nền Tảng: Có License vs. Không Có License

> **Bối cảnh quan trọng**: Khi bán cho nhà nước Việt Nam, cần xem xét:
> 1. Quy định mua sắm công (Luật Đấu thầu, Nghị định 13/2023...)
> 2. Yêu cầu tài liệu pháp lý (license key, chứng chỉ xuất xứ)
> 3. Yêu cầu bảo mật và chủ quyền dữ liệu (data sovereignty)
> 4. Khả năng tự host trên hạ tầng nội bộ

---

### 🟢 NHÓM 1: Open Source / Có thể tự host (Không cần mua license nước ngoài)

Đây là nhóm **phù hợp nhất để bán cho nhà nước Việt Nam** — có thể đóng gói, deploy on-premise, bán dịch vụ triển khai + tùy biến.

| Nền tảng | License | Điểm mạnh | Điểm yếu | Phù hợp nhà nước? |
|---|---|---|---|---|
| **Appsmith** | Apache 2.0 (Community) | Self-host, internal tools, admin panel; customize JS; 10,000+ GitHub stars | Chủ yếu internal-facing, UI còn hạn chế | ✅ Tốt |
| **Budibase** | GPL v3 (Community) | Self-host, RBAC mạnh, kết nối DB/API linh hoạt | Enterprise tính phí; UI builder còn cơ bản | ✅ Tốt |
| **NocoDB** | AGPL v3 | Thay thế Airtable, giao diện bảng tính, REST API auto-gen | Không build app phức tạp | ✅ Cho nghiệp vụ đơn giản |
| **ToolJet** | AGPL v3 | Self-host, workflow, internal apps, kết nối 50+ data source | Enterprise tính phí | ✅ Tốt |
| **n8n** | Fair Code (self-host free) | Tự động hóa workflow mạnh mẽ, 400+ integration | Chủ yếu automation, không phải app builder | ✅ Cho tự động hóa |
| **Directus** | BSL (self-host free) | Headless CMS + No-code data platform; API-first | Cần dev backend vận hành | ⚠️ Cần kỹ thuật |
| **Convertigo** | AGPL | Mobile + Web low-code, self-host | Ít phổ biến | ✅ Có hướng enterprise |

> **Mô hình kinh doanh gợi ý**: Mua/sử dụng bản community miễn phí → **Đóng gói thành sản phẩm riêng** → Bán dịch vụ **triển khai, tùy biến, hỗ trợ** cho nhà nước (doanh thu từ dịch vụ, không phải license phần mềm gốc)

---

### 🔴 NHÓM 2: Commercial / Cần mua license (Phù hợp nếu có ngân sách lớn)

| Nền tảng | Vendor | Pricing | Điểm mạnh | Rủi ro với nhà nước |
|---|---|---|---|---|
| **Microsoft Power Apps** | Microsoft | $5–20/user/tháng | Tích hợp M365, quen thuộc, Power BI, Teams | Phụ thuộc cloud MS; dữ liệu có thể nằm ngoài VN |
| **OutSystems** | OutSystems Inc. | ~$75k+ / năm (enterprise) | Mission-critical, scalable, AI-powered | Chi phí rất cao; vendor lock-in nặng |
| **Mendix** | Siemens | Subscription theo app | Enterprise-grade; visual collaborative dev | Đắt; cần chứng minh ROI |
| **ServiceNow** | ServiceNow Inc. | Rất cao | ITSM + Low-code; mạnh khu vực công US | Không phổ biến ở VN; giá quá cao |
| **Salesforce Platform** | Salesforce | $25–300/user/tháng | CRM + App Builder; đa dạng | Phức tạp; chủ yếu CRM |
| **Zoho Creator** | Zoho | $8–20/user/tháng | Giá hợp lý; data residency tuỳ chọn | Ít brand recognition ở nhà nước VN |
| **Appian** | Appian Corp | Enterprise pricing | BPM + Low-code; mạnh khu vực công | Ít hiện diện ở VN |

---

### 🟡 NHÓM 3: "Freemium" — Free tier nhưng có enterprise plans

| Nền tảng | Free Tier | Giới hạn | Ghi chú |
|---|---|---|---|
| **OutSystems** | Community (1 app) | Không production-scale | Bẫy: sau commun thì rất đắt |
| **Retool** | Free (self-host) | Phức tạp setup | Internal tools; có self-host option |
| **Glide** | Free (5 apps) | Chỉ mobile app từ Google Sheets | Không phù hợp nhà nước |
| **Bubble** | Free plan | Data stored trên Bubble cloud | Không self-host → không phù hợp nhà nước |

---

### 🟣 NHÓM 4: Chuyên biệt theo Domain — AI, Workflow Orchestration, Game/Simulation

Đây là nhóm **không được nhắc đến trong định nghĩa LCNC truyền thống** nhưng thực sự là no-code/low-code theo nghĩa rộng — phù hợp cho các bài toán chuyên sâu.

---

#### 🔵 Temporal.io — Workflow Orchestration (Durable Execution)

| Tiêu chí | Chi tiết |
|---|---|
| **Bản chất** | Không phải low-code thuần — là nền tảng **lập trình bền vững** (durable execution) cho microservices, job scheduling, long-running process |
| **Open Source** | ✅ **MIT License** — hoàn toàn miễn phí, self-host |
| **Self-host** | ✅ Có thể deploy on-premise (Docker, K8s) |
| **Phù hợp với** | Dev team xây hệ thống **tự động hóa phức tạp**: duyệt văn bản nhiều bước, retry logic, saga pattern |
| **Không phù hợp** | Citizen developer — cần viết code (Go/Java/Python/TypeScript) |
| **Cạnh tranh** | n8n, Camunda, Apache Airflow, Kestra |
| **Nhà nước VN** | ⚠️ Cần IT team mạnh; không thể self-service; nhưng rất mạnh cho hệ thống critical |

> **Kết luận**: Temporal là *infrastructure*, không phải LCNC tool cho người dùng cuối. Tuy nhiên có thể **dùng làm backend engine** cho một sản phẩm LCNC workflow bán cho nhà nước. Tốt hơn dùng **n8n** hoặc **Camunda** nếu muốn có UI no-code.

---

#### 🟠 LangChain / LangFlow — AI Application Builder (No-Code for AI)

| Tiêu chí | Chi tiết |
|---|---|
| **LangChain** | Framework code Python/JS để xây LLM apps — **không phải no-code** |
| **LangFlow** | ✅ **UI no-code trực quan** trên nền LangChain — kéo thả node để build AI pipeline |
| **License** | ✅ **MIT License** — miễn phí hoàn toàn |
| **Self-host** | ✅ Deploy bằng Docker hoặc Python, không cần cloud nước ngoài |
| **Tính năng** | Xây chatbot, RAG (Retrieval-Augmented Generation), AI agent, xử lý tài liệu — bằng kéo thả |
| **Export** | Workflow xuất JSON, deploy thành REST API endpoint |
| **Mở rộng** | Viết custom component bằng Python nếu cần |
| **Nhà nước VN** | ✅ Rất tiềm năng — build **chatbot hỏi đáp chính sách**, **xử lý văn bản hành chính tự động** |

> **Kết luận**: Đưa vào danh sách open source ✅ — đặc biệt phù hợp cho bài toán **AI + chính phủ số**: chatbot cổng dịch vụ công, tóm tắt văn bản tự động, tìm kiếm ngữ nghĩa trong kho tài liệu nhà nước.

**So sánh các tool AI no-code khác:**
| Tool | License | Self-host | Đặc điểm |
|---|---|---|---|
| **LangFlow** | MIT | ✅ | Kéo thả, LangChain-based, AI pipeline |
| **Flowise** | MIT | ✅ | Tương tự LangFlow, nhẹ hơn, dễ setup hơn |
| **Dify.ai** | Apache 2.0 | ✅ | LLM app platform, có UI quản lý prompt/RAG đẹp hơn |
| **n8n + AI nodes** | Fair Code | ✅ | Kết hợp workflow automation + AI |

---

#### 🟤 Unreal Engine Blueprint — Visual Scripting (Game/Simulation/VR)

| Tiêu chí | Chi tiết |
|---|---|
| **Bản chất** | Hệ thống **lập trình trực quan dạng node** trong Unreal Engine — thay thế C++ cho logic game/app |
| **License** | ⚠️ **KHÔNG phải open source** — EULA của Epic Games |
| **Dùng miễn phí?** | ✅ Miễn phí download và sử dụng |
| **Royalty** | Game: **5% royalty** sau $1M doanh thu đầu tiên |
| **Non-game (enterprise/gov)** | ⚠️ Yêu cầu **per-seat subscription** nếu công ty >$1M/năm doanh thu |
| **Chính phủ** | Phải tuân theo EULA như doanh nghiệp — liên hệ Epic Games để custom enterprise agreement |
| **Phù hợp với** | Mô phỏng, đào tạo thực tế ảo (VR training), digital twin, visualization 3D |
| **Nhà nước VN** | ⚠️ Tiềm năng cho **đào tạo VR quân sự, y tế, cứu hỏa** nhưng cần license Enterprise |

> **Kết luận**: Blueprint **KHÔNG vào được danh sách open source**. Là công cụ visual scripting rất mạnh cho simulation/VR, nhưng cần thương lượng license với Epic Games trong dự án nhà nước. Nguồn mở thay thế gần nhất: **Godot Engine** (MIT License) với GDScript visual scripting.

**So sánh với các visual scripting engine khác:**
| Engine | License | Blueprint/Visual | Phù hợp nhà nước |
|---|---|---|---|
| **Unreal Engine Blueprint** | EULA (có phí enterprise) | ✅ Rất mạnh | ⚠️ Cần license |
| **Godot Engine** | MIT | ✅ VisualScript/GDScript | ✅ Free, open source |
| **Unity (Visual Scripting)** | Unity ToS (subscription) | ✅ Shader Graph, Bolt | ⚠️ Phí từ $2k/năm |

---

## 4. ⚠️ Rủi Ro & Thách Thức Cần Biết

### Rủi ro kỹ thuật
- **Shadow IT**: Người dùng tự build app ngoài tầm kiểm soát IT → bảo mật lỗ hổng
- **Scalability ceiling**: LCNC tools chạy chậm khi load lớn hoặc data phức tạp
- **Technical debt**: App của "citizen developer" không có tài liệu, khó maintain
- **Tích hợp hệ thống legacy**: Kết nối với ERP, CSDL cũ của nhà nước rất phức tạp

### Rủi ro pháp lý / thương mại (quan trọng với nhà nước VN)
| Vấn đề | Chi tiết |
|---|---|
| **Chủ quyền dữ liệu** | Nhiều SaaS lưu data trên server nước ngoài → vi phạm quy định Luật An ninh mạng 2018 |
| **Vendor lock-in** | OutSystems/Mendix dùng ngôn ngữ riêng → không thể chuyển nền tảng dễ dàng |
| **License nước ngoài** | Nhà nước VN có thể yêu cầu phần mềm phải có bản quyền hợp lệ và hỗ trợ nội địa |
| **Điều khoản sử dụng thương mại** | Một số open source (AGPL) yêu cầu open-source toàn bộ code nếu phân phối → cần đọc kỹ |
| **Mua sắm công** | Cần hồ sơ năng lực, giấy đăng ký kinh doanh CNTT, chứng nhận an toàn thông tin (ISO 27001...) |

---

## 5. 💡 Chiến Lược Gợi Ý Cho Việc Bán Cho Nhà Nước VN

### Lộ trình A – Dùng nền tảng Open Source + Bán dịch vụ
```
Open Source Platform (Budibase / Appsmith / ToolJet)
    ↓ Tùy biến giao diện tiếng Việt
    ↓ Triển khai on-premise (server của bộ/ngành)
    ↓ Tích hợp với hệ thống hiện có
    ↓ Đào tạo + hỗ trợ kỹ thuật
    ↓ Bán hợp đồng DỊCH VỤ (không phải license phần mềm)
```
**Ưu điểm**: Không vi phạm IP; dữ liệu nằm trong nước; dễ thuyết phục nhà nước về chủ quyền

### Lộ trình B – Đại lý / Reseller nền tảng thương mại
```
Trở thành Đối tác / Reseller của Zoho, Mendix, Power Apps
    ↓ Mua license bulk → bán lại cho nhà nước
    ↓ Cộng thêm dịch vụ triển khai, tích hợp
    ↓ Cần: Hợp đồng đại lý chính thức
              Hóa đơn VAT + chứng nhận bản quyền
              Hỗ trợ kỹ thuật nội địa
```
**Rủi ro**: Chi phí license cao; phụ thuộc vendor nước ngoài

### Lộ trình C – Tự xây dựng sản phẩm riêng (MADE IN VIETNAM)
- Dùng LCNC engine mã nguồn mở làm nền → xây thêm tầng tùy biến
- Đăng ký bản quyền phần mềm Việt Nam (NAIP)
- Tham gia Chương trình Make in Vietnam của Bộ TT&TT
- Lợi thế: Ưu tiên mua sắm sản phẩm "nội địa" theo các chính sách hiện hành

---

## 6. 🎯 Khuyến Nghị Theo Từng Tình Huống

| Tình huống | Gợi ý nền tảng | Mô hình doanh thu |
|---|---|---|
| Nhà nước cần tool nội bộ đơn giản (quản lý danh sách, form báo cáo) | NocoDB / Budibase | Phí triển khai + bảo trì |
| Nhà nước cần workflow tự động hóa (duyệt văn bản, routing) | n8n + ToolJet | Dịch vụ tích hợp |
| Nhà nước cần app phức tạp (quản lý nhân sự, tài chính) | Appsmith Enterprise / Convertigo | License + dịch vụ |
| Nhà nước có ngân sách lớn, cần hệ thống chuẩn quốc tế | OutSystems / Mendix (qua đại lý) | Bán license + triển khai |
| SME / doanh nghiệp vừa và nhỏ | Zoho Creator / Power Apps | Subscription theo tháng |

---

## 7. 📋 Checklist Khi Tiếp Cận Nhà Nước

- [ ] Kiểm tra: phần mềm có **self-host** được không? (bắt buộc với nhiều cơ quan nhà nước)
- [ ] Kiểm tra: có điều khoản **data residency** — dữ liệu lưu trong nước không?
- [ ] Chuẩn bị: **Hồ sơ pháp lý** — đăng ký kinh doanh CNTT, thẩm định ATTT
- [ ] Chuẩn bị: **Demo on-premise** trong môi trường mạng nội bộ (không cần internet)
- [ ] Chuẩn bị: **Phương án đào tạo** cho "citizen developer" trong cơ quan
- [ ] Xác minh: **Điều khoản của open source license** có cho phép sử dụng thương mại không
- [ ] Tham khảo: Chương trình **Make in Vietnam** và danh sách phần mềm ưu tiên của Bộ TT&TT

---

*Nguồn tham khảo: Gartner LCAP Magic Quadrant 2024, Forrester Low-Code Platform Forecast 2024-2028, OutSystems Case Studies, McKinsey Digital Transformation Report, Quyết định 749/QĐ-TTg, Luật An ninh mạng 2018 (VN), Temporal.io Docs (MIT License), LangFlow GitHub (MIT License), Unreal Engine EULA 2024, Epic Games Licensing FAQ*
