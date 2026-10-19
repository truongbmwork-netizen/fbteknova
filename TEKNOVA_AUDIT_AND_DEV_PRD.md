# BÁO CÁO ĐỐI SOÁT TOÀN DIỆN & KẾ HOẠCH HÀNH ĐỘNG DEV (PRD) — NÂNG CẤP PORTAL TEKNOVA 2026

- **Mã văn kiện kỹ thuật**: `TEKNOVA-MASTER-AUDIT-PRD-2026`
- **Cơ quan ban hành**: Ban Thẩm định Kỹ thuật & Kiến trúc Hệ thống TEKNOVA
- **Phiên bản tài liệu**: `v3.0.0-RELEASE-CANDIDATE` (Bản đặc tả kỹ thuật và đối soát toàn diện)
- **Tài liệu nguồn chân lý pháp lý (SSOT)**: `audit_teknova/ho_so_nang_luc_extracted.txt` (Hồ Sơ Năng Lực TEKNOVA 2026)
- **Hệ thống đối soát hiện trường**:
  * **Bản Dev Demo**: `https://teknova-demo.netlify.app/` (Codebase Vue 3 / Next.js tại `teknova-portal/`, ảnh chụp `screenshots/demo_fullpage.png`)
  * **Bản Design Tham chiếu**: `https://teknova-topaz.vercel.app/` (Codebase React Vite tại `teknova_redesign/`, ảnh chụp `screenshots/design_fullpage.png`)
- **Tài liệu đầu vào tổng hợp**: Báo cáo Explorer Survey 1 (Dữ liệu), Survey 2 (Thị giác & Layout), Survey 3 (Showcase UX & Kiến trúc 5 Tính năng)
- **Ngày hoàn tất ban hành**: 15/10/2026
- **Trạng thái phê duyệt**: **CHÍNH THỨC — SẴN SÀNG TRIỂN KHAI DEV ACTION SPRINT**

---

## 1. TỔNG QUAN ĐIỀU HÀNH & BẢNG ĐIỂM SẴN SÀNG SHOWCASE (EXECUTIVE SUMMARY & SCORECARD)

### 1.1 Mục Đích Văn Bản & Tinh Thần Phối Hợp Kỹ Thuật (Marketing to Engineering Note)

Văn bản này được biên soạn từ góc nhìn của **Bộ phận Marketing & Truyền thông Doanh nghiệp**, đóng vai trò là một bản đối soát hiện trường và cầu nối thông tin chuyển tiếp tới **Bộ phận Kỹ thuật & Lập trình (Dev Team)**.

Trong các buổi tiếp cận thực tế, đi thuyết trình và chào thầu giải pháp trước Hội đồng Giám đốc Bệnh viện, Lãnh đạo Sở Y tế, Sở TT&TT/KH&CN cùng các Tổng thầu viễn thông quốc gia, Cổng thông tin điện tử TEKNOVA Portal chính là **bộ mặt thương hiệu đầu tiên** mà đối tác mở ra kiểm tra. Bộ phận Marketing nhận thấy đội ngũ Dev đã nỗ lực xây dựng hạ tầng trang web vận hành mượt mà, ổn định trên cả Netlify và Vercel. 

Tuy nhiên, để phục vụ mục tiêu showcase thực tế, tạo dựng niềm tin pháp lý vững chắc và hỗ trợ tối đa cho quá trình chốt thầu/bảo vệ dự án, Bộ phận Marketing xin phép gửi đến các anh em Dev:
* **Bản tổng hợp dữ liệu chuẩn xác nhất** từ tài liệu pháp lý gốc *Hồ Sơ Năng Lực TEKNOVA 2026* (về nhân sự, 22 hợp đồng thực tế, MST và văn bằng).
* **Bản đối soát chi tiết về mặt thị giác, trải nghiệm thao tác, hiệu ứng cuộn/hover** giữa bản Dev demo hiện tại và bản thiết kế tham chiếu.
* **Đề xuất bổ sung các tính năng tương tác thực chiến** nhằm giúp trang web không chỉ "đẹp" mà còn trở thành công cụ thuyết trình giải pháp trực quan, sống động cho đội ngũ đi thị trường.

Rất mong nhận được sự đồng hành, góp ý và hỗ trợ kỹ thuật từ đội ngũ Dev để cùng hoàn thiện sản phẩm một cách chỉn chu, chuyên nghiệp nhất.


---

### 1.2 Bảng Tổng Hợp Đóng Góp & Giá Trị Bổ Trợ Giữa 2 Bản (Cross-Platform Synthesis)

Thay vì đánh giá thắng - thua, mục tiêu của bảng này là chỉ ra **ưu điểm của mỗi bên để chắt lọc sang nhau**, hướng tới một phiên bản production hoàn thiện nhất:

| STT | Trụ Cột Năng Lực | Ưu Điểm Đáng Học Hỏi Ở Bản Demo (Netlify) | Điểm Sáng Gợi Ý Ở Bản Thiết Kế (Topaz) | Giải Pháp Kết Hợp Tối Ưu (Synthesis Action) |
|:---:|---|---|---|---|
| **1** | **Nhận Diện Pháp Lý & Thương Hiệu** | Trình bày slogan *"Thực Người • Thực Việc • Thực Giá Trị"* rất mạch lạc, danh mục dịch vụ rõ ràng. | Gợi ý bổ sung MST `0402300331`, văn phòng làm việc 456 Nguyễn Hữu Thọ và khối chân dung lãnh đạo đại diện. | **Kết hợp**: Giữ nguyên thông điệp của Demo, bổ sung thêm ảnh chân dung lãnh đạo và chuẩn hóa tên **Trần Bình Sơn** theo giấy ĐKKD. |
| **2** | **Bằng Chứng Dự Án Thực Tế** | Bố cục thẻ text (Tên dự án, tỷ lệ hoàn thành, đối tác) rất chuẩn mực và ngay ngắn. | Gợi ý bố trí ảnh chụp hiện trường 16:9 sắc nét, giúp tăng tính sinh động khi thuyết trình. | **Kết hợp**: Giữ cấu trúc thẻ của Demo, nạp thêm ảnh thumbnail 16:9 lưu trữ cục bộ từ gói assets để hiển thị đầy đủ, không lo lỗi link. |
| **3** | **Bố Cục & Phân Cấp Thị Giác** | Tốc độ tải trang nhanh, font chữ tiếng Việt hiển thị rõ ràng, không bị giật lag. | Bố cục căn giữa (Centered Monumental 1200px) giúp bảng điều phối EMR mở rộng nhìn rất bề thế. | **Kết hợp**: Kế thừa độ mượt của Demo, áp dụng bố cục căn giữa và màu xanh Cobalt điểm nhấn cho Card 4 như bản Thiết kế. |
| **4** | **Hiệu Ứng Cuộn & Chuyển Động** | Cuộn trang dứt khoát theo cơ chế trình duyệt, nhẹ máy, không kén thiết bị. | Tích hợp Lenis Smooth Scroll tạo cảm giác lướt đầm tay, có tính năng dừng dải logo khi rê chuột. | **Kết hợp**: Cấu hình Lenis mức độ vừa phải (`duration: 1.1`), giữ nguyên tính năng dừng dải đối tác khi hover để người thuyết trình kịp chỉ vào logo. |
| **5** | **Khung Pháp Lý & Tiêu Chuẩn Y Tế** | Nêu bật các thông tư cốt lõi (TT 26, QĐ 3176, liên thông BHYT). | Gắn các huy hiệu (badges) trực quan ngay trên đầu thẻ dự án. | **Kết hợp**: Chuẩn hóa 8 căn cứ pháp lý thành các huy hiệu nhỏ gọn, chuyên nghiệp. |
| **6** | **Chuyển Đổi Khách Hàng (Lead Funnel)** | Nút gọi hotline `0935 722 579` trên topbar rất thuận tiện. | Bổ sung thêm nút phụ *"Tải Profile PDF"* cạnh nút *"Khám phá dự án"*. | **Kết hợp**: Giữ nút hotline của Demo, thêm nút Tải Profile PDF của bản Thiết kế để hỗ trợ khách tải tài liệu nhanh. |

---

### 1.3 Hai Điểm Cần Sự Hỗ Trợ Ưu Tiên Từ Đội Ngũ Dev (Priority Focus)

Để website sẵn sàng trở thành công cụ trình chiếu thực tế trước các cơ sở y tế và đối tác, Bộ phận Marketing xin phép đề xuất 2 nội dung ưu tiên cần anh em Dev hỗ trợ hoàn thiện sớm:

```text
┌────────────────────────────────────────────────────────────────────────────────────────────────┐
│                         2 NỘI DUNG ƯU TIÊN PHỐI HỢP KỸ THUẬT                                   │
├────────────────────────────────────────────────────────────────────────────────────────────────┤
│ 1. BỔ SUNG KHỐI THÔNG ĐIỆP LÃNH ĐẠO & CHÂN DUNG ĐẠI DIỆN:                                      │
│    • Hiện trạng Demo: Đã có phần cam kết chữ Tín và hỗ trợ 24/7 rất đanh thép.                 │
│    • Đề xuất bổ trợ: Ghép thêm ảnh chân dung cắt nền của lãnh đạo (đã chuẩn bị sẵn tại         │
│      public/ceo-cutout.png) vào cạnh khối cam kết; đồng thời lưu ý cập nhật đúng tên Chủ tịch  │
│      kiêm Tổng Giám đốc là Ông TRẦN BÌNH SƠN (MBA, Kỹ sư Điện tử) theo hồ sơ năng lực 2026.     │
├────────────────────────────────────────────────────────────────────────────────────────────────┤
│ 2. NẠP TƯ LIỆU ẢNH THỰC TẾ CHO KHỐI DỰ ÁN TIÊU BIỂU:                                           │
│    • Hiện trạng Demo: Khung text dự án rất gọn gàng nhưng phần hình ảnh chưa hiển thị được.    │
│    • Đề xuất bổ trợ: Sử dụng bộ ảnh chụp hiện trường 16:9 (bác sĩ kê đơn EMR, phòng khám TTYT, │
│      màn hình Zalo OA) đã lưu trữ cục bộ trong thư mục assets để đưa lên đầu mỗi thẻ dự án.   │
└────────────────────────────────────────────────────────────────────────────────────────────────┘
```


---

### 1.4 Tuyên Ngôn Giá Trị Cốt Lõi (Value Proposition Statement)
> **"Chuyển đổi TEKNOVA Portal từ một 'Trang web tin tức tĩnh với các hình ảnh mockup tượng trưng' trở thành một 'Cỗ máy trình diễn giải pháp Y tế số & Chính quyền số tương tác thực chiến' — Nơi mỗi dòng mã, mỗi con số, mỗi quy trình đều được bảo chứng 100% bằng chứng cứ pháp lý, văn bản nghiệm thu thực tế và chiều sâu công nghệ lâm sàng."**

---

## 2. ĐỐI SOÁT DỮ LIỆU XÁC THỰC TỪ HỒ SƠ NĂNG LỰC TEKNOVA 2026 (AUTHORITATIVE DATA RECONCILIATION)

Dữ liệu dưới đây là **Chân lý Đơn nhất (Single Source of Truth - SSOT)**, được trích xuất trực tiếp và có tính pháp lý ràng buộc từ tài liệu gốc *HỒ SƠ NĂNG LỰC TEKNOVA 2026* (`audit_teknova/ho_so_nang_luc_extracted.txt`) và Giấy chứng nhận Đăng ký Doanh nghiệp số 0402300331. Mọi thành phần mã nguồn, cơ sở dữ liệu (`teknova-data.ts`, `projects.ts`, `services.ts`) phải tuân thủ tuyệt đối các tham số này.

### 2.1 Thông Tin Pháp Nhân, Mã Số Thuế & Trụ Sở Doanh Nghiệp

* **Tên tiếng Việt có dấu đầy đủ**: CÔNG TY CỔ PHẦN ĐỔI MỚI SÁNG TẠO TEKNOVA
* **Tên giao dịch quốc tế**: TEKNOVA INNOVATION JOINT STOCK COMPANY
* **Tên viết tắt doanh nghiệp**: TEKNOVA .,JSC
* **Mã số doanh nghiệp / Mã số thuế (MST)**: **`0402300331`**
* **Ngày cấp giấy phép kinh doanh**: **23/09/2025** (Giải thích nguồn gốc hậu tố nghiệp vụ `0925` trong email chính thức)
* **Cơ quan cấp phép**: Phòng Đăng ký Kinh doanh – Sở Kế hoạch và Đầu tư Thành phố Đà Nẵng
* **Người đại diện theo pháp luật**: Ông **TRẦN BÌNH SƠN** (Chức vụ: Chủ tịch Hội đồng Quản trị kiêm Tổng Giám đốc)
* **Trụ sở làm việc & Giao dịch chính thức (HSNL 2026)**:
  * **Địa chỉ**: **Tầng 3, 456 Nguyễn Hữu Thọ, Phường Cẩm Lệ, Thành phố Đà Nẵng, Việt Nam**
  * *Ý nghĩa chiến lược*: Tuyến phố trung tâm công nghệ và dịch vụ y tế của Đà Nẵng; địa điểm đặt văn phòng điều hành, phòng Lab R&D và tiếp đón đối tác.
* **Địa chỉ đăng ký kinh doanh theo giấy phép (ĐKKD)**:
  * **Địa chỉ**: **K131/18 Lý Thái Tổ, Phường Thanh Khê, Quận Thanh Khê, Thành phố Đà Nẵng, Việt Nam**
* **Số điện thoại Hotline hỗ trợ 24/7**: **`0935 722 579`** (Cấu hình `tel:0935722579` trên toàn bộ nút gọi)
* **Hệ thống thư điện tử nghiệp vụ & chính thức**:
  * Email nghiệp vụ hồ sơ năng lực: `teknova0925@gmail.com`
  * Email định danh tên miền: `contact@teknova.com.vn`
* **Cổng thông tin điện tử chính thức**: `https://www.teknova.com.vn/`
* **Khẩu hiệu hành động (Slogan / Brand Motto)**: **"NOW OR NEVER"** & **"Thực Người • Thực Việc • Thực Giá Trị"**

---

### 2.1.1 Hồ Sơ Pháp Lý & Giấy Chứng Nhận Đăng Ký Doanh Nghiệp & Bản Quyền Tác Giả (Legal Certificates)

Tài liệu pháp lý gốc được trích xuất trực tiếp từ Phần A (Trang 7-9) của Hồ Sơ Năng Lực 2026. Đây là các "bằng chứng thép" (Steel Evidence) cần được tích hợp vào khối Showcase / Modal xem hồ sơ pháp lý trên web:

```text
┌────────────────────────────────────────────────────────────────────────────────────────────────┐
│                   DANH MỤC TÀI LIỆU PHÁP LÝ & BẢN QUYỀN TÁC GIẢ ĐÃ CHỨNG THỰC                  │
├────────────────────────────────────────────────────────────────────────────────────────────────┤
│ 1. GIẤY CHỨNG NHẬN ĐĂNG KÝ DOANH NGHIỆP CÔNG TY CỔ PHẦN (LẦN ĐẦU)                             │
│    • Cơ quan cấp: Phòng Đăng ký Kinh doanh - Sở Kế hoạch và Đầu tư TP. Đà Nẵng                 │
│    • Mã số doanh nghiệp: 0402300331 | Ngày cấp: 23/09/2025                                     │
│    • Vốn điều lệ: 20.000.000.000 đồng (Hai mươi tỷ đồng chẵn) - 2.000.000 cổ phần              │
│    • Người đại diện pháp luật: TRẦN BÌNH SƠN (Sinh ngày 30/05/1974 - Chức danh: Giám đốc)     │
│    • Người ký: KT. Trưởng phòng - Phó Trưởng phòng Trần Anh Dũng (Dấu đỏ chứng thực)           │
│    • File tài nguyên: audit_teknova/assets/giay_dang_ky_kinh_doanh_lan1.png                    │
├────────────────────────────────────────────────────────────────────────────────────────────────┤
│ 2. GIẤY CHỨNG NHẬN ĐĂNG KÝ DOANH NGHIỆP (ĐĂNG KÝ THAY ĐỔI LẦN THỨ 1)                           │
│    • Ngày thay đổi: 17/08/2026                                                                 │
│    • Cập nhật địa chỉ trụ sở chính: Tầng 3, 456 Nguyễn Hữu Thọ, P. Cẩm Lệ, TP. Đà Nẵng        │
│    • Người ký: KT. Trưởng phòng - Phó Trưởng phòng Trần Anh Dũng                               │
│    • File tài nguyên: audit_teknova/assets/giay_dang_ky_kinh_doanh_thaydoi1.png                │
├────────────────────────────────────────────────────────────────────────────────────────────────┤
│ 3. GIẤY CHỨNG NHẬN ĐĂNG KÝ QUYỀN TÁC GIẢ PHẦN MỀM Y KHOA                                       │
│    • Cơ quan cấp: Cục Bản Quyền Tác Giả - Bộ Văn Hóa, Thể Thao và Du Lịch                      │
│    • Số giấy chứng nhận: Số 7057/2026/QTG | Ngày cấp: 07/07/2026                               │
│    • Mã hồ sơ: G16.15-260512-0059 | Cục trưởng ký: Trần Hoàng (Dấu đỏ Cục Bản quyền tác giả)   │
│    • Tên tác phẩm: PhanmemYkhoa.Teknova (Bao gồm hệ sinh thái giải pháp y tế số cốt lõi):      │
│      - Datlich24.Teknova (Phần mềm Đặt lịch khám & Tiếp đón thông minh)                        │
│      - LIS.Teknova (Hệ thống Thông tin Xét nghiệm & Trả kết quả)                               │
│      - HIS.Teknova (Hệ thống Thông tin Quản lý Bệnh viện lõi)                                  │
│      - EMR.Teknova (Hệ thống Bệnh án Điện tử chuẩn Thông tư 46/2018/TT-BYT)                    │
│    • Tác giả: Trần Bình Sơn (Đà Nẵng) & Trương Văn Voãn (Quảng Ngãi)                           │
│    • Chủ sở hữu bản quyền: CÔNG TY CỔ PHẦN ĐỔI MỚI SÁNG TẠO TEKNOVA                           │
│    • File tài nguyên: audit_teknova/assets/giay_chung_nhan_ban_quyen_tac_gia.png              │
├────────────────────────────────────────────────────────────────────────────────────────────────┤
│ 4. SƠ ĐỒ CƠ CẤU TỔ CHỨC VÀ ĐIỀU HÀNH DOANH NGHIỆP                                              │
│    • Cơ cấu phân tầng: Đại hội đồng Cổ đông -> HĐQT & Ban TGĐ -> 4 Khối Phòng Ban Chuyên Trách │
│    • File tài nguyên: audit_teknova/assets/so_do_to_chuc.png                                   │
└────────────────────────────────────────────────────────────────────────────────────────────────┘
```

> **Hướng dẫn Kỹ thuật cho Dev (Implementation Guideline)**:
> - Tích hợp các ảnh chứng nhận này vào khối **Block 7 (Leadership & Trust)** hoặc tạo modal xem chi tiết **"Xem Giấy Chứng Nhận Pháp Lý & Bản Quyền"** có hiệu ứng zoom lightbox (`v-viewer` hoặc `yet-another-react-lightbox`).
> - Khi khách hàng B2G bấm xem, hiển thị bản quét scan chất lượng cao có dấu đỏ của Sở KH&ĐT Đà Nẵng và Cục Bản Quyền Tác Giả, chứng minh năng lực sở hữu trí tuệ độc quyền đối với phân hệ lõi `EMR.Teknova`, `HIS.Teknova`, `LIS.Teknova`.


### 2.2 Bảng Đối Soát Chi Tiết 12 Nhân Sự Chủ Chốt & Đội Ngũ Chuyên Gia

Cơ cấu nhân sự trong Hồ Sơ Năng Lực 2026 (`ho_so_nang_luc_extracted.txt:26-78`) gồm đúng **12 nhân sự nòng cốt**, trong đó 9/12 nhân sự có văn bằng chứng chỉ Đại học, Thạc sĩ, Tiến sĩ được công chứng đính kèm trực tiếp tại Phần B (Trang 17-18). 

Dưới đây là bảng đối soát chi tiết, phân định rõ theo **4 Khối Phòng Ban chức năng**:

```text
                               ┌────────────────────────────────────────────────────────┐
                               │     HỘI ĐỒNG QUẢN TRỊ & TỔNG GIÁM ĐỐC                  │
                               │     • Trần Bình Sơn (MBA, KS. Điện tử - >20 năm KN)    │
                               │     • TS. Lê Trọng Nhân (Tiến sĩ Xử lý TH & VT)        │
                               └──────────────────────────┬─────────────────────────────┘
                                                          │
          ┌───────────────────────────────────────────────┼───────────────────────────────────────────────┐
          │                                               │                                               │
┌─────────▼──────────────────────────┐  ┌─────────────────▼──────────────────┐  ┌─────────────────────────▼─────────────────────┐
│ KHỐI KỸ THUẬT & R&D PHẦN MỀM LÕI   │  │ KHỐI TRIỂN KHAI & HẠ TẦNG THỰC ĐỊA │  │ KHỐI VẬN HÀNH, TÀI CHÍNH & KINH DOANH       │
│ • KS. Võ Quang Hòa (13 năm KN)     │  │ • KS. Nguyễn Hoài Nhân (12 năm KN) │  │ • CN. Nguyễn Thị Dung (Kế toán - >5 năm KN)   │
│ • ThS. Lê Hoàng Hải (>10 năm KN)   │  │ • KS. Trần Ngọc Trai (>20 năm KN)  │  │ • CN. Nguyễn Thị Thúy Vân (HR - >10 năm KN)   │
│ • CN. Dương Mạnh Quân (01 năm KN)  │  │ • KS. Trần Minh Chiến (02 năm KN)  │  │ • CN. Bùi Thị Mai (Kinh doanh - 02 năm KN)    │
│                                    │  │ • KS. Lê Thiện Nhân (01 năm KN)    │  │                                               │
└────────────────────────────────────┘  └────────────────────────────────────┘  └───────────────────────────────────────────────┘
```

#### Bảng Đối Soát 12 Nhân Sự Chuẩn:

| STT | Họ và Tên Nhân Sự | Bằng Cấp / Học Vị Chuẩn HSNL 2026 | Thâm Niên | Chức Danh & Phòng Ban | Chuyên Môn Trọng Tâm & Đóng Góp Công Nghệ | Minh Chứng Bằng Cấp (HSNL Trang 17-18) |
|:---:|---|---|:---:|---|---|:---:|
| **01** | **Trần Bình Sơn** | **MBA (Thạc sĩ Quản trị Kinh doanh), Kỹ sư Điện tử** | **Trên 20 năm** | **Chủ tịch HĐQT & Tổng Giám đốc** (Đại diện pháp luật) | Lãnh đạo điều hành toàn diện, chiến lược công nghệ y tế số, chuyên gia tư vấn mô hình thuê dịch vụ CNTT OPEX theo Quyết định 80/2014/QĐ-TTg. | **Có bản scan bằng ĐH/MBA** |
| **02** | **TS. Lê Trọng Nhân** | **Tiến sĩ (Ph.D) Xử lý tín hiệu & Viễn thông** | **Trên 15 năm** | **Giám đốc Công nghệ (CTO) & Cố vấn Cấp cao** | Xử lý tín hiệu số, kiến trúc dữ liệu y tế lớn, chuẩn kết nối HL7 FHIR / DICOM, kiến trúc bảo mật dữ liệu theo Nghị định 13/2023/NĐ-CP. | **Có bản scan bằng Tiến sĩ** |
| **03** | **KS. Võ Quang Hòa** | **Kỹ sư Công nghệ Thông tin** | **13 năm** | **Trưởng phòng Kiến trúc Phần mềm & An toàn thông tin** | Lập trình phần mềm lõi Bệnh án điện tử (EMR), phân hệ ký số Cloud CA & dấu thời gian TSA, trích xuất cấu trúc XML QĐ 3176/QĐ-BYT. | **Có bản scan bằng Kỹ sư CNTT** |
| **04** | **KS. Nguyễn Hoài Nhân** | **Kỹ sư Công nghệ Thông tin** | **12 năm** | **Trưởng bộ phận Tích hợp Hệ thống & HIS** | Tích hợp liên thông HIS bệnh viện với Cổng Đơn thuốc Quốc gia (TT 26/2025), cổng giám định BHYT (QĐ 130), chuẩn hóa dữ liệu khám chữa bệnh. | **Có bản scan bằng Kỹ sư CNTT** |
| **05** | **ThS. Lê Hoàng Hải** | **Thạc sỹ (M.Sc) Khoa học Máy tính** | **Trên 10 năm** | **Trưởng nhóm Khoa học Dữ liệu & AI** | Ứng dụng trí tuệ nhân tạo nhận diện chữ viết y khoa (OCR), Data Warehouse, Cổng cơ sở dữ liệu dân số 56 xã phường theo Đề án 06/CP. | **Có bản scan bằng Thạc sĩ KHMT** |
| **06** | **KS. Trần Minh Chiến** | **Kỹ sư Công nghệ Thông tin** | **02 năm** | **Kỹ sư Triển khai Hệ thống & Zalo OA** | Lập trình và tích hợp Zalo Official Account, Zalo Mini App chăm sóc bệnh nhân, trả kết quả xét nghiệm tự động, hỗ trợ dịch vụ công trực tuyến. | **Có bản scan bằng Kỹ sư CNTT** |
| **07** | **KS. Lê Thiện Nhân** | **Kỹ sư Kỹ thuật Máy tính** | **01 năm** | **Kỹ sư Phần cứng Y tế & Kiosk Tiếp đón** | Lắp đặt, cấu hình và bảo trì Kiosk đón tiếp người bệnh thông minh, tích hợp đầu đọc thẻ CCCD gắn chip, máy quét QR VNeID và thiết bị bảo mật. | **Có bản scan bằng Kỹ sư KTMT** |
| **08** | **CN. Dương Mạnh Quân** | **Cử nhân Công nghệ Thông tin** | **01 năm** | **Lập trình viên Web Portal & CSDL Phân tán** | Phát triển giao diện Web Portal, các dashboard theo dõi chỉ số y tế - dân số cơ sở, tối ưu hóa truy vấn cơ sở dữ liệu tốc độ cao. | **Có bản scan bằng Cử nhân CNTT** |
| **09** | **KS. Trần Ngọc Trai** | **Kỹ sư Điện** | **Trên 20 năm** | **Kỹ sư Trưởng Hạ tầng Điện nhẹ (ELV) & Data Center** | *Nhân sự kỳ cựu bị bỏ quên*. Thiết kế và thi công hệ thống mạng cáp quang, điện nhẹ ELV bệnh viện, hệ thống Camera AI giám sát và phòng máy chủ y tế. | **Có bản scan bằng Kỹ sư Điện** |
| **10** | **CN. Nguyễn Thị Dung** | **Cử nhân Kinh tế** | **Trên 05 năm** | **Kế toán trưởng & Phụ trách Quyết toán Thầu** | Quản trị tài chính doanh nghiệp, lập dự toán thầu dịch vụ CNTT y tế, thủ tục thanh quyết toán nguồn kinh phí thường xuyên và BHYT. | Có hồ sơ nghiệp vụ kế toán |
| **11** | **CN. Nguyễn Thị Thúy Vân** | **Cử nhân Quản trị** | **Trên 10 năm** | **Trưởng bộ phận Hành chính - Nhân sự** | Quản trị nguồn nhân lực, điều phối quy chế hoạt động, kiểm soát tính pháp lý và hồ sơ năng lực nhân sự khi tham gia các gói thầu. | Có hồ sơ nghiệp vụ nhân sự |
| **12** | **CN. Bùi Thị Mai** | **Cử nhân Quản trị Kinh doanh** | **02 năm** | **Chuyên viên Kinh doanh Dự án B2G & Chăm sóc Khách hàng** | *Nhân sự mới được phục hồi*. Khảo sát nhu cầu bệnh viện và UBND phường xã, điều phối lịch khảo sát hiện trường, chăm sóc đối tác B2G. | Có bằng Cử nhân QTKD |

---

### 2.3 Chuẩn Hóa & Bổ Sung Đầy Đủ Thông Tin Nhân Sự

1. **Khắc phục lỗi P0: Thay tên đổi họ Tổng Giám Đốc trên bản Design**:
   * *Sai lệch*: Bản Design Reference ghi: *"Nguyễn Hùng Sơn - CHỦ TỊCH HỘI ĐỒNG QUẢN TRỊ & TỔNG GIÁM ĐỐC"*.
   * *Phê phán*: Đây là sự sơ suất trong khâu nhập liệu mẫu (placeholder) trong quá trình thiết kế giao diện (AI placeholder distortion). TEKNOVA không có bất kỳ lãnh đạo nào tên là Nguyễn Hùng Sơn.
   * *Hành động*: Khẳng định tư cách người đứng đầu hợp pháp duy nhất là **Ông TRẦN BÌNH SƠN (MBA, Kỹ sư Điện tử)**. Thay thế toàn bộ text, thẻ alt, metadata và gắn kèm bản tóm lược quá trình hơn 20 năm công tác trong ngành Viễn thông - CNTT.
2. **Phục hồi 7 nhân sự bị cắt xén**:
   * Bản Design chỉ khai báo 5 người trong code và dồn toàn bộ thành một câu text chung chung: *"Đội ngũ kỹ sư hiện trường"*.
   * Bản Dev Demo hoàn toàn không hiển thị danh sách nhân sự trên trang chủ.
   * *Hành động*: Đưa toàn bộ 12 nhân sự vào giao diện với đầy đủ chức danh, phân loại theo 4 phòng ban chuẩn, làm nổi bật hai nhân sự trên 20 năm kinh nghiệm là **Trần Bình Sơn** và **Trần Ngọc Trai**.

---

### 2.4 Bảng Danh Mục Đầy Đủ 22 Hợp Đồng Dự Án Thực Tế (Authoritative Contract Roster)

Toàn bộ 22 dự án dưới đây được trích xuất nguyên văn từ Phần B Hồ Sơ Năng Lực 2026 (`ho_so_nang_luc_extracted.txt:80-172`). Đây là các hợp đồng đã ký kết, đang triển khai hoặc đã nghiệm thu bàn giao thành công, phân bổ theo 3 nhóm khách hàng chiến lược:

#### Nhóm 1: Khối Cơ Sở Y Tế & Bệnh Viện Công Lập (10 Hợp đồng)

| Mã HĐ | Đơn Vị Chủ Đầu Tư / Khách Hàng | Tên Gói Thầu / Hợp Đồng Triển Khai Thực Tế | Địa Điểm Triển Khai | Căn Cứ Pháp Lý & Số QĐ Trúng Thầu / E-TBMT | Giá Trị Nghiệm Thu Thực Chiến |
|:---:|---|---|---|---|---|
| **HĐ-01** | **Bệnh viện Phổi Đà Nẵng** | Cung cấp dịch vụ thuê phần mềm Bệnh án điện tử (EMR) | Tổ 53 Phước Lý, P. Hòa Minh, Q. Liên Chiểu, TP. Đà Nẵng | **Thông tư 46/2018/TT-BYT**; **QĐ 80/2014/QĐ-TTg**; **Quyết định số 142/QĐ-SYT** (Phê duyệt KQLCNT); E-TBMT: IB2400018920-00; HĐ số 08/2024/HĐ-BVP | Xóa bỏ 100% bệnh án giấy; tích hợp ký số Cloud CA cho 40+ bác sĩ; lưu trữ an toàn hồ sơ bệnh án nội trú. |
| **HĐ-02** | **Bệnh viện Phổi Đà Nẵng** | Cung cấp phần mềm quảng bá miễn phí thông tin Bệnh viện Phổi Đà Nẵng qua Zalo OA (tích hợp HIS bệnh viện) | Tổ 53 Phước Lý, P. Hòa Minh, Q. Liên Chiểu, TP. Đà Nẵng | **Nghị định 13/2023/NĐ-CP**; **Quyết định số 218/QĐ-BVP**; E-TBMT: IB2400031102-00; HĐ số 12/2024/HĐ-ZALO-BVP | Kênh tiếp đón tự động qua Zalo; tra cứu lịch khám; trả kết quả chẩn đoán hình ảnh và xét nghiệm qua liên kết mã hóa. |
| **HĐ-03** | **Bệnh viện Phổi Đà Nẵng** | Nâng cấp hệ thống phần mềm HIS để định dạng dữ liệu đầu ra phục vụ quản lý, giám định, thanh toán chi phí KCB BHYT theo Quyết định 3176/QĐ-BYT và trích xuất dữ liệu Người bệnh tử vong đẩy Cổng dữ liệu hành chính công thành phố | Số 215 Nguyễn Đình Tứ, P. Hòa Khánh, TP. Đà Nẵng | **Quyết định 3176/QĐ-BYT** (29/10/2024); **Đề án 06/CP**; **Quyết định số 356/QĐ-BVP**; E-TBMT: IB2400054210-00; HĐ số 29/2024/HĐ-XML-BVP | Tự động hóa trích xuất dữ liệu XML đầu ra chuẩn BHYT; đồng bộ dữ liệu người bệnh tử vong phục vụ thủ tục mai táng trên Cổng DVC. |
| **HĐ-04** | **Trung tâm Y tế Khu vực Liên Chiểu** | Cập nhật mẫu đơn thuốc điện tử theo Thông tư số 26/2025/TT-BYT | Số 525 Tôn Đức Thắng, P. Hòa Khánh, TP. Đà Nẵng | **Thông tư 26/2025/TT-BYT**; Cổng `donthuocquocgia.vn`; **Quyết định số 89/QĐ-TTYTLC**; E-TBMT: IB2500004512-00; HĐ số 05/2025/HĐ-TT26-LC | Liên thông 100% đơn thuốc ngoại trú; cấp mã định danh đơn thuốc quốc gia và in mã QR trong thời gian phản hồi < 0.8s. |
| **HĐ-05** | **Trung tâm Y tế Khu vực Liên Chiểu** | Triển khai nâng cấp hệ thống trích xuất dữ liệu (XML) theo Quyết định 3176/QĐ-BYT | Số 525 Tôn Đức Thắng, P. Hòa Khánh, TP. Đà Nẵng | **Quyết định 3176/QĐ-BYT** Bộ Y tế; **Quyết định số 194/QĐ-TTYTLC**; E-TBMT: IB2400038910-00; HĐ số 19/2024/HĐ-XML-LC | Cập nhật định dạng gói tin giám định BHYT mới nhất; bảo đảm tỷ lệ duyệt hồ sơ đạt 100%, không bị trả về. |
| **HĐ-06** | **Trung tâm Y tế Khu vực Liên Chiểu** | Nâng cấp phần mềm quản lý BV đáp ứng QĐ 130/QĐ-BYT, CV 1165, CV 3617 liên thông dữ liệu Giấy chứng sinh, Giấy báo tử lên cổng giám định BHYT triển khai Đề án 06/CP, liên thông GPLX lên Cổng DVCQG, gửi thanh toán và kết quả KCB qua Zalo OA | Số 525 Tôn Đức Thắng, P. Hòa Khánh, TP. Đà Nẵng | **QĐ 130/QĐ-BYT**; CV 1165 & 3617/BYT-KCB; **Đề án 06/CP**; DVC Quốc gia; **Quyết định số 312/QĐ-TTYTLC**; E-TBMT: IB2400062145-00; HĐ số 33/2024/HĐ-QD130-LC | Tích hợp toàn diện 4 phân hệ liên thông nhà nước: Giấy chứng sinh, Giấy báo tử, Khám sức khỏe lái xe và trả viện phí không tiền mặt qua Zalo OA. |
| **HĐ-07** | **Trung tâm Y tế Khu vực Ngũ Hành Sơn** | Thuê phần mềm Bệnh án điện tử (EMR) năm 2025 | Phường Ngũ Hành Sơn, TP. Đà Nẵng | **Quyết định 80/2014/QĐ-TTg**; Thông tư 46/2018/TT-BYT; **Quyết định số 45/QĐ-TTYTNHS**; E-TBMT: IB2500001290-00; HĐ số 02/2025/HĐ-EMR-NHS | Triển khai trọn gói mô hình thuê phần mềm EMR không cần vốn đầu tư công CAPEX; ký hợp đồng thường niên từ kinh phí sự nghiệp. |
| **HĐ-08** | **Trung tâm Y tế Khu vực Cẩm Lệ** | Cập nhật hệ thống HIS để đẩy dữ liệu XML theo Quyết định 3176/QĐ-BYT ngày 29/10/2024 của Bộ Y tế | Số 105 Nguyễn Nhàn, P. Cẩm Lệ, TP. Đà Nẵng | **Quyết định 3176/QĐ-BYT** Bộ Y tế; **Quyết định số 208/QĐ-TTYTCL**; E-TBMT: IB2400041280-00; HĐ số 21/2024/HĐ-HIS-CL | Chuẩn hóa cấu trúc dữ liệu XML viện phí, kết nối thông suốt với cổng tiếp nhận dữ liệu BHXH TP. Đà Nẵng. |
| **HĐ-09** | **Bệnh viện Phụ sản - Nhi Đà Nẵng** | Phần mềm trả kết quả xét nghiệm qua Zalo cho cơ sở 01 | Số 402 Lê Văn Hiến, P. Ngũ Hành Sơn, TP. Đà Nẵng | **Nghị định 13/2023/NĐ-CP**; **Quyết định số 175/QĐ-BVPSN**; E-TBMT: IB2400033100-00; HĐ số 16/2024/HĐ-PSN | Trả kết quả xét nghiệm nhanh chóng cho sản phụ và người nhà qua Zalo OA; giảm tải 60% tình trạng tập trung đông tại sảnh chờ xét nghiệm. |
| **HĐ-10** | **Bệnh viện Y học Cổ truyền TP. Đà Nẵng** | Tặng cho Website Bệnh viện Y học Cổ truyền TP. Đà Nẵng | Số 77 Đinh Gia Trinh, P. Thanh Khê, TP. Đà Nẵng | Luật Khám bệnh, chữa bệnh 2023; **Quyết định số 56/QĐ-BVYDCT**; HĐ hợp tác chuyển giao số 01/2024/HĐ-YDCT | Cổng thông tin điện tử giới thiệu dịch vụ khám chữa bệnh y học cổ truyền kết hợp hiện đại, tra cứu bảng giá và lịch bác sĩ. |

#### Nhóm 2: Khối Chính Quyền Số, Dân Số & Địa Phương (8 Hợp đồng)

| Mã HĐ | Đơn Vị Chủ Đầu Tư / Cơ Quan | Tên Gói Thầu / Hợp Đồng Triển Khai Thực Tế | Địa Điểm Triển Khai | Lĩnh Vực Chuyên Môn & Số QĐ Phê Duyệt / E-TBMT | Giá Trị Thực Tiễn |
|:---:|---|---|---|---|---|
| **HĐ-11** | **Chi cục Dân số TP. Đà Nẵng** | Xây dựng Web tổng hợp và thống kê dữ liệu báo cáo của tuyến cơ sở | Số 118 Lê Đình Lý, P. Thanh Khê, TP. Đà Nẵng | Quản lý dữ liệu chuyên ngành Dân số - KHHGĐ; Đề án 06/CP; **Quyết định số 92/QĐ-CCDS**; E-TBMT: IB2400019400-00; HĐ số 07/2024/HĐ-CCDS | Thu thập và chuẩn hóa dữ liệu biến động dân số từ toàn bộ 56 xã/phường trên địa bàn TP. Đà Nẵng về một hệ thống tập trung. |
| **HĐ-12** | **Chi cục Dân số TP. Đà Nẵng** | Xây dựng và vận hành trang thông tin điện tử (Website) Chi cục Dân số TP. Đà Nẵng | Số 118 Lê Đình Lý, P. Thanh Khê, TP. Đà Nẵng | Cổng thông tin truyền thông cơ quan nhà nước; **Quyết định số 128/QĐ-CCDS**; E-TBMT: IB2400025110-00; HĐ số 11/2024/HĐ-WEB-CCDS | Kênh truyền thông chính thức về chính sách dân số, chăm sóc sức khỏe sinh sản và dịch vụ công chuyên ngành. |
| **HĐ-13** | **Trung tâm Phục vụ Hành chính công P. Ngũ Hành Sơn** | Xây dựng, tích hợp và vận hành hệ thống gửi thông báo, tin nhắn qua nền tảng Zalo OA phục vụ công tác quản lý, điều hành và truyền thông | Phường Ngũ Hành Sơn, TP. Đà Nẵng | Chính quyền số cấp cơ sở; Tương tác công dân; **Quyết định số 164/QĐ-UBND**; E-TBMT: IB2400029800-00; HĐ số 14/2024/HĐ-UBND-NHS | Kênh thông báo tiến độ xử lý hồ sơ một cửa, tiếp nhận phản ánh hiện trường và tuyên truyền chính sách số đến người dân. |
| **HĐ-14** | **Trung Tâm CĐS Và Công Nghệ Chiến Lược Đà Nẵng** | Nâng cấp phần mềm Đánh giá các tiêu chí ứng dụng công nghệ thông tin trên địa bàn TP. Đà Nẵng | Số 02 Quang Trung, P. Hải Châu, TP. Đà Nẵng | Đánh giá xếp hạng chỉ số ICT Index / DTI thành phố; **Quyết định số 240/QĐ-STTTT**; E-TBMT: IB2400045600-00; HĐ số 22/2024/HĐ-CDS-STTTT | Nền tảng chấm điểm, đối soát và xếp hạng mức độ ứng dụng CNTT và chuyển đổi số cho các sở ban ngành, quận huyện. |
| **HĐ-15** | **UBND Xã Xuân Phú, TP. Đà Nẵng** | Tư vấn khảo sát, xây dựng đề án Chuyển đổi số giai đoạn 2026 - 2030 tầm nhìn 2035 xã Xuân Phú | Thôn Mộc Bài, Xã Xuân Phú, TP. Đà Nẵng | Tư vấn chiến lược chuyển đổi số nông thôn mới thông minh; **Quyết định số 28/QĐ-UBNDXP**; E-TBMT: IB2500000890-00; HĐ số 03/2025/HĐ-XP | Khảo sát hiện trạng, lập báo cáo tiền khả thi và đề xuất quy hoạch hạ tầng số, kinh tế số và xã hội số cấp xã. |
| **HĐ-16** | **UBND Xã Xuân Phú, TP. Đà Nẵng** | Tư vấn khảo sát, cập nhật, tạo lập dữ liệu cơ sở chuyên ngành vào Kho dữ liệu dùng chung của thành phố | Thôn Mộc Bài, Xã Xuân Phú, TP. Đà Nẵng | Chuẩn hóa dữ liệu & Tích hợp Data Warehouse thành phố; **Quyết định số 64/QĐ-UBNDXP**; E-TBMT: IB2500001940-00; HĐ số 09/2025/HĐ-DL-XP | Làm sạch và số hóa dữ liệu hộ tịch, đất đai, người có công; kết nối vào CSDL dùng chung của UBND Thành phố. |
| **HĐ-17** | **Phòng Văn Hóa – Xã Hội Xã Tiên Phước** | Tạo lập, chuẩn hoá, cập nhật dữ liệu vào phần mềm, cơ sở dữ liệu chuyên ngành | Số 81 Huỳnh Thúc Kháng, Xã Tiên Phước, TP. Đà Nẵng | Quản lý dữ liệu văn hóa - xã hội địa phương; **Quyết định số 182/QĐ-UBNDTP**; E-TBMT: IB2400034120-00; HĐ số 15/2024/HĐ-TP | Số hóa toàn bộ hồ sơ quản lý đối tượng bảo trợ xã hội và di tích văn hóa lịch sử trên địa bàn xã. |
| **HĐ-18** | **Phòng Văn Hóa Xã Hội Phường Điện Bàn Bắc** | Xây dựng điểm tổ dân phố thông minh: Hệ thống Camera AI, thiết bị xử lý lưu trữ dữ liệu và các hạng mục có liên quan | Tổ dân phố Xóm Bùng, P. Điện Bàn Bắc, TP. Đà Nẵng | Đô thị thông minh & An ninh trật tự AI; **Quyết định số 298/QĐ-UBNDDBB**; E-TBMT: IB2400051200-00; HĐ số 26/2024/HĐ-DBB | Lắp đặt cụm Camera AI giám sát an ninh trật tự, tự động nhận diện biển số và cảnh báo vi phạm truyền về trung tâm điều hành phường. |

#### Nhóm 3: Khối Doanh Nghiệp, Ngân Hàng & Viễn Thông (4 Hợp đồng)

| Mã HĐ | Đơn Vị Đối Tác / Khách Hàng | Tên Gói Thầu / Hợp Đồng Triển Khai Thực Tế | Địa Điểm Triển Khai | Phạm Vi Kỹ Thuật & Căn Cứ Hợp Đồng | Giá Trị Công Nghệ |
|:---:|---|---|---|---|---|
| **HĐ-19** | **Công ty TNHH Cloud ACE** | Nghiên cứu và phát triển phần mềm cổng thông tin quản lý khách hàng bao gồm website và ứng dụng trên thiết bị di động (Mobile App) | Số 384 Hoàng Diệu, P. Khánh Hội, TP. Hồ Chí Minh | Web Portal & Mobile App React Native / Flutter; Cloud Architecture; HĐ thương mại dịch vụ số 01/2024/TEK-CA; Đối tác Google Cloud Premier | Xây dựng hệ thống quản lý tài khoản và hóa đơn điện toán đám mây cho đối tác cấp cao (Premier Partner) của Google Cloud tại Việt Nam. |
| **HĐ-20** | **Ngân hàng TMCP Đại Chúng Việt Nam (PvcomBank)** | Nâng cấp, mở rộng phần mềm quản lý bệnh viện và tích hợp kênh giao tiếp điện tử với người bệnh thông qua Zalo OA | Số 22 Ngô Quyền, P. Cửa Nam, TP. Hà Nội | Fintech y tế; Tích hợp cổng thanh toán viện phí Napas / VietQR; HĐ hợp tác công nghệ số 04/2024/TEK-PVCOM | Hợp tác công nghệ tích hợp thanh toán viện phí không dùng tiền mặt và gửi thông báo biến động giao dịch qua Zalo OA bệnh viện. |
| **HĐ-21** | **MobiFone Đà Nẵng – CN Tổng Công ty MobiFone** | Phần mềm hỗ trợ giải đáp thủ tục hành chính công trên Zalo OA và Zalo Mini App | Số 586 Nguyễn Hữu Thọ, P. Cẩm Lệ, TP. Đà Nẵng | AI Chatbot / Trợ lý ảo; Zalo Mini App SDK; HĐ dịch vụ số 18/2024/TEK-MBF | Xây dựng trợ lý ảo hỏi đáp dịch vụ công, hướng dẫn nộp hồ sơ trực tuyến qua Zalo Mini App cho thuê bao di động. |
| **HĐ-22** | **MobiFone Đà Nẵng – CN Tổng Công ty MobiFone** | Phần mềm chuyển đổi số phường xã qua Zalo OA | Số 586 Nguyễn Hữu Thọ, P. Cẩm Lệ, TP. Đà Nẵng | Nền tảng điều hành đô thị số; Zalo Notification Service; HĐ kinh tế số 25/2024/TEK-MBF2 | Bộ công cụ số hóa điều hành phường xã, gửi thông báo khẩn cấp và tiếp nhận tin báo từ người dân qua Zalo. |

---

### 2.5 Bản Đồ Khung Pháp Lý Chuyên Ngành Bắt Buộc (Regulatory Framework Mapping)

Năng lực cốt lõi giúp TEKNOVA chiến thắng trong các buổi thẩm định hồ sơ thầu y tế công là **sự thấu hiểu và đáp ứng triệt để 8 văn bản quy phạm pháp luật sống còn**:

```text
┌────────────────────────────────────────────────────────────────────────────────────────────────┐
│                          BẢN ĐỒ KHUNG PHÁP LÝ & SẢN PHẨM TEKNOVA TƯƠNG ỨNG                    │
├─────────────────────────┬──────────────────────────────────┬───────────────────────────────────┤
│ Văn bản Quy phạm PL     │ Nội dung & Quy chuẩn Kỹ thuật    │ Sản phẩm / Hợp đồng Đối ứng       │
├─────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ 1. Quyết định           │ Chuẩn dữ liệu đầu ra phục vụ     │ • Nâng cấp HIS BV Phổi Đà Nẵng    │
│    3176/QĐ-BYT          │ quản lý, giám định, thanh toán   │ • Nâng cấp trích xuất TTYT        │
│    (29/10/2024)         │ KCB BHYT & dữ liệu tử vong DVC.  │   Liên Chiểu và TTYT Cẩm Lệ       │
├─────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ 2. Thông tư             │ Chuẩn hóa cấu trúc đơn thuốc     │ • Cập nhật đơn thuốc điện tử      │
│    26/2025/TT-BYT       │ điện tử, mã định danh quốc gia   │   TTYT Khu vực Liên Chiểu         │
│                         │ và liên thông donthuocquocgia.vn │ • Kiến trúc Async Queue (< 0.8s)  │
├─────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ 3. Quyết định           │ Chuẩn và định dạng dữ liệu gói tin│ • Nâng cấp HIS TTYT Liên Chiểu   │
│    130/QĐ-BYT           │ XML giám định BHYT; liên thông   │   (CV 1165, CV 3617 liên thông    │
│    (18/01/2023)         │ giấy chứng sinh, giấy báo tử.    │   chứng sinh, báo tử, GPLX)       │
├─────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ 4. Thông tư             │ Quy chế Hồ sơ Bệnh án điện tử    │ • Thuê phần mềm EMR BV Phổi       │
│    46/2018/TT-BYT       │ (EMR), ký số Cloud CA y lệnh,    │ • Thuê EMR TTYT Ngũ Hành Sơn      │
│                         │ dấu thời gian TSA, bỏ bệnh án giấy│ • Ký số 40+ bác sĩ, kho lưu EMR  │
├─────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ 5. Quyết định           │ Cơ chế Thuê dịch vụ CNTT trọn    │ • Hợp đồng thuê EMR BV Phổi       │
│    80/2014/QĐ-TTg &     │ gói chi từ nguồn thu viện phí    │ • Hợp đồng thuê EMR TTYT Ngũ      │
│    Nghị định 73/2019    │ (OPEX); 0đ vốn đầu tư công CAPEX │   Hành Sơn (phê duyệt trong 3 tuần│
├─────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ 6. Đề án 06/CP          │ Phát triển ứng dụng dữ liệu dân  │ • Web CSDL Dân số 56 xã phường    │
│    Thủ tướng Chính phủ  │ cư, định danh CCCD chip, VNeID,  │ • Kiosk tiếp đón tích hợp CCCD    │
│                         │ liên thông thủ tục hành chính    │ • Liên thông GPLX DVCQG           │
├─────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ 7. Nghị định            │ Bảo vệ dữ liệu cá nhân; bóc      │ • Kiến trúc Decoupled Link OTP    │
│    13/2023/NĐ-CP        │ tách dữ liệu y bạ nhạy cảm       │   BV Phổi, BV Phụ sản - Nhi       │
│                         │ khỏi máy chủ bên thứ ba (Zalo)   │ • Mã hóa dữ liệu người bệnh       │
├─────────────────────────┼──────────────────────────────────┼───────────────────────────────────┤
│ 8. Nghị định            │ Tiêu chuẩn bảo đảm an toàn hệ    │ • Hạ tầng máy chủ Cloud EMR cô lập│
│    85/2016/NĐ-CP        │ thống thông tin Cấp độ 3         │ • Tường lửa WAF, mã hóa AES-256   │
└─────────────────────────┴──────────────────────────────────┴───────────────────────────────────┘
```

---

### 2.6 Chuẩn Hóa Danh Sách Đối Tác & Khách Hàng Theo Hợp Đồng Thực Tế

Bản Dev Demo (`teknova-demo`) hiện đang vi phạm nghiêm trọng Điều 89 Luật Đấu thầu 2023 khi hiển thị các thương hiệu không có trong quan hệ hợp đồng:
1. **Xóa bỏ vĩnh viễn các logo không có hợp đồng**:
   * *Bệnh viện Đa Khoa Quốc Tế Vinmec (JCI)*
   * *Hệ thống Y tế Medlatec*
   * *Viện Khoa học Y Dược Đà Nẵng*
   * *Cisco Systems, Microsoft Solutions Partner, Fortinet Security*
   * *Logo cấp hội sở ngân hàng: Vietcombank, BIDV, VietinBank* (Chỉ giữ lại PVcomBank theo đúng HĐ-20).
2. **Xóa bỏ các case study và quote khách hàng hư cấu**:
   * Xóa bỏ case study *"Tổng Công ty Phân phối Dược & Thiết bị Y tế Miền Trung"*.
   * Xóa bỏ danh sách nhận xét của các bác sĩ giả định: *"BS. CKII Nguyễn Văn A"*, *"DSCK Trần Thị B"*, *"ThS. BS Lê Văn C"*.
   * Thay thế bằng: **Trích dẫn thực tế từ Biên bản nghiệm thu kỹ thuật của Hội đồng Khoa học Bệnh viện Phổi Đà Nẵng và TTYT Liên Chiểu**.


---

## 3. ĐỐI SOÁT CHI TIẾT GIAO DIỆN & BỐ CỤC 8 BLOCK (VISUAL & LAYOUT AUDIT ACROSS 8 BLOCKS)

Dưới đây là bảng đối soát chi tiết từng khu vực giao diện giữa Hiện trạng Bản Dev Demo (`teknova-demo`), Mục tiêu Bản Design Reference (`teknova-topaz`), kèm Đánh giá kỹ thuật và CSS Blueprints chuẩn hóa:

```text
┌─────────────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                 SƠ ĐỒ BỐ CỤC 8 KHU VỰC THỊ GIÁC TOÀN TRANG                              │
├─────────────────────────────────────────────────────────────────────────────────────────────────────────┤
│ [BLOCK 1] HEADER & NAVIGATION (Glassmorphism, Logo SVG, Dual CTA Buttons, Top Progress Bar)             │
│ [BLOCK 2] HERO SECTION & PANORAMA EMR MOCKUP (Monumental Centered 1200px, 4-step Flow, Floating Badges)│
│ [BLOCK 3] STATS & METRICS COUNTER (Dải 4 chỉ số thực: >20 Năm, 22+ Dự án, 12+ Chuyên gia, 100% Nghiệm thu) │
│ [BLOCK 4] PARTNERS & CLIENT TICKER (Infinite Marquee 12 Bệnh viện & Cơ quan thực tế, Hover Pause)      │
│ [BLOCK 5] 6 CORE SOLUTION DOMAINS (Bento Grid công nghệ, Card Hero Accent Cobalt Blue #415DA8)         │
│ [BLOCK 6] CASE STUDIES & PROJECTS (Local Image Assets, Bổ sung Badge QĐ 3176/TT 26, Click mở Drawer)   │
│ [BLOCK 7] LEADERSHIP & VISION (Chân dung Cutout CEO Trần Bình Sơn, 3 Cam kết hành động, Dấu ấn Trust) │
│ [BLOCK 8] FOOTER & CTA BANNER (Banner Chuyển đổi B2G Xanh Cobalt, Footer Đầy đủ Trụ sở & MST)           │
└─────────────────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

### BLOCK 1: HEADER & THANH ĐIỀU HƯỚNG (NAVIGATION BAR)

#### Bảng Đối Soát 3 Cột:

| Yếu Tố Cấu Thành | Hiện Trạng (Bản Dev Demo - Netlify) | Mục Tiêu (Bản Design Reference - Topaz) | Đánh Giá Kỹ Thuật & CSS Blueprint Chuẩn Hóa |
|---|---|---|---|
| **Logo Thương Hiệu** | Logo Chevron xanh đơn sắc, chữ TEKNOVA đậm, thiếu tagline phụ. | Biểu tượng khối công nghệ đa giác tinh xảo, font chữ Plus Jakarta Sans / Be Vietnam Pro, hiển thị huy hiệu nhỏ "NOW OR NEVER". | Cập nhật file SVG logo chuẩn vector, hỗ trợ `h-9 w-auto`, giữ tỉ lệ khung hình không méo trên màn hình Retina. |
| **Hiệu Ứng Nền (Styling)** | Dải màu trắng đặc `bg-white/95`, đổ bóng đơn giản `shadow-sm`, viền dưới xám mờ. | Glassmorphism cao cấp: `backdrop-blur-md bg-surface-container-lowest/85`, viền mờ `border-b border-outline-variant/20`. | Áp dụng đúng công thức Glassmorphism: `backdrop-blur-md bg-white/80 border-b border-slate-200/60 sticky top-0 z-50 transition-all duration-300`. |
| **Cấu Trúc Menu** | 5 mục: `Trang chủ`, `Giới thiệu`, `Lĩnh vực`, `Dự án`, `Đội ngũ` (Bị lệch vì trang chủ không có mục đội ngũ). | 5 mục: `Trang chủ`, `Giới thiệu`, `Lĩnh vực`, `Dự án`, `Liên hệ`. Font medium, hover đổi màu xanh cobalt `#415DA8`. | Đồng bộ 5 liên kết chuẩn SEO: `['/', '/gioi-thieu', '/giai-phap', '/du-an', '/lien-he']`. Active state có gạch chân xanh `h-0.5 bg-primary rounded-full`. |
| **Cụm Nút Hành Động (CTA)** | Chỉ có 1 nút đơn độc: `Trao đổi dự án ->` kèm số hotline đặt ở phía trước. | **Kiến trúc Dual-CTA chiến lược**: <br>1. *Nút phụ*: `Tải Profile PDF` (icon download, nền mờ).<br>2. *Nút chính*: `Tư vấn dự án` (nền xanh, hiệu ứng đổ bóng phát quang). | **Khôi phục ngay nút Tải Profile PDF** bên cạnh nút Tư vấn. Cấu trúc HTML/Tailwind: <br>`<button class="inline-flex items-center gap-2 px-3.5 py-2 rounded-lg text-xs font-semibold text-slate-700 bg-slate-100 hover:bg-slate-200 border border-slate-200/80 transition-all">Tải Profile PDF</button>` |
| **Thanh Tiến Trình (Progress)** | Hoàn toàn không có. | Có thanh chỉ báo tiến độ đọc trang mảnh 3px (`#top-progress-bar`) chạy mượt theo thanh cuộn trang. | Tích hợp thanh tiến trình trên đỉnh Header: <br>`<div id="top-progress-bar" class="fixed top-0 left-0 h-[3px] bg-gradient-to-r from-blue-600 to-cyan-500 z-50 transition-all"></div>`. |

---

### BLOCK 2: HERO SECTION & MOCK DASHBOARD EMR/HIS

#### Bảng Đối Soát 3 Cột:

| Yếu Tố Cấu Thành | Hiện Trạng (Bản Dev Demo - Netlify) | Mục Tiêu (Bản Design Reference - Topaz) | Đánh Giá Kỹ Thuật & CSS Blueprint Chuẩn Hóa |
|---|---|---|---|
| **Mô Hình Bố Cục (Layout)** | **Phân chia 2 cột lệch (Split-column grid 12 cols)**: Cột trái chứa chữ (55%), cột phải chứa mockup (45%). | **Monumental Centered Layout (Căn giữa hoành tráng)**: Tiêu đề căn giữa `max-w-4xl`, Mockup EMR Panorama trải rộng `max-w-[1200px]`. | Bố cục 2 cột ở bản Dev bóp nghẹt khung mockup còn ~500px, khiến các phân hệ EMR bị biến dạng. Bắt buộc chuyển sang cấu trúc căn giữa trải rộng chuẩn Agency. |
| **Typography Tiêu Đề** | Chữ bị bẻ dòng gượng gạo, cỡ chữ nhỏ (~42px), tương phản giữa text đen và text gradient xanh nhạt nhòa. | Cỡ chữ `56px` (Desktop), line-height `1.15`, letter-spacing `-0.03em`, font Be Vietnam Pro font-black (900), tương phản mạnh mẽ. | Cấu hình class Tailwind: <br>`text-4xl sm:text-5xl lg:text-[56px] font-black tracking-tight leading-[1.15] text-slate-900 text-center`. |
| **Huy Hiệu Chứng Nhận (Badges)** | 2 badge tĩnh nhỏ đặt dưới nút bấm, không có tương tác giải thích nghiệp vụ. | 2 badge tương tác: `Chứng nhận HIS/EMR Chuẩn BYT` và `An toàn Cấp độ 3 (NĐ 85)`, có Tooltip giải thích chi tiết khi hover. | Bổ sung Tooltip nổi giải thích cụ thể: <br>• Tooltip 1: *"Tuân thủ 100% Thông tư 46/2018/TT-BYT, Thông tư 26/2025/TT-BYT và Quyết định 130/QĐ-BYT"*. <br>• Tooltip 2: *"Hệ thống kiểm soát an toàn thông tin theo Nghị định 85/2016/NĐ-CP"*. |
| **Khung Mockup Panorama 3D** | Khung Dashboard chữ nhật đứng, chỉ hiển thị vài con số đơn giản, thiếu chiều sâu lâm sàng. | Khung Dashboard macOS 1200px: Header 3 nút tròn, nhãn `Live v4.8`, Sidebar 4 phân hệ, 3 Card KPI và **Sơ đồ 4 bước dòng chảy dữ liệu lâm sàng**. | Chuyển đổi khung mockup thành component điều khiển tương tác mô phỏng 4-5 bước quy trình khám bệnh. Độ phân giải mockup đạt tối thiểu 2400x1400px (retina scale). |
| **Thẻ Nổi 3D (Floating Badges)** | Bị co sát mép hoặc bị ẩn hoàn toàn khi màn hình thu nhỏ. | 2 thẻ nổi bay bổng 2 bên sườn mockup: <br>• Trái: *Hồ Sơ Bệnh Án EMR (Liên thông BYT 100%)*<br>• Phải: *Kiosk Y Tế CCCD (Tích hợp QR VNeID)*. | Cấu hình vị trí tuyệt đối (Absolute Positioning): <br>`class="absolute -left-6 top-1/4 p-4 rounded-xl bg-white/95 shadow-xl border border-slate-100 backdrop-blur-md hidden md:flex items-center gap-3 animate-float-slow"`. |

---

### BLOCK 3: STATS & METRICS COUNTER

#### Bảng Đối Soát 3 Cột:

| Yếu Tố Cấu Thành | Hiện Trạng (Bản Dev Demo - Netlify) | Mục Tiêu (Bản Design Reference - Topaz) | Đánh Giá Kỹ Thuật & CSS Blueprint Chuẩn Hóa |
|---|---|---|---|
| **Tính Xác Thực Của Số Liệu** | Hiển thị: `15+ Năm`, **`50+ Dự án` (Phóng đại)**, `20+ Chuyên gia`, `100% Hài lòng`. | Hiển thị: **`>20 Năm` Kinh nghiệm**, **`22+` Dự án Thực tế**, **`12` Chuyên gia Nòng cốt**, **`100%` Nghiệm thu Chuẩn BYT**. | Con số `50+` ở bản Dev là phóng đại phi thực tế, vi phạm đạo đức dữ liệu. Phải chuẩn hóa chính xác theo HSNL 2026: **`22+` Hợp đồng thực tế** và **`>20 Năm` thâm niên lãnh đạo**. |
| **Lỗi Kỹ Thuật Counter (Lỗi NaN)** | Số liệu tĩnh, không có animation. | Bản Design bị lỗi hydration kịch bản chạy số, render thành chuỗi lỗi: **`00+ Năm`, `00+ Dự án`, `00+ Chuyên gia`, `000%`**. | Khắc phục triệt để lỗi NaN bằng Intersection Observer hook an toàn với fallback số tĩnh nếu trình duyệt tắt JavaScript. |
| **Styling & Nhịp Điệu Nền** | Nền trắng trơn, không có đường phân cách, bị lẫn vào khối Hero phía trên. | Dải nền màu lam nhạt `bg-surface-container-low` (`#EFF4FF`), viền bo mềm `rounded-2xl`, tạo nhịp nghỉ thị giác tinh tế. | Áp dụng cấu trúc: <br>`<div class="py-10 bg-slate-50 border-y border-slate-200/60 my-12">...</div>` với lưới 4 cột chia đều `grid grid-cols-2 lg:grid-cols-4 gap-6`. |

---

### BLOCK 4: PARTNERS & CLIENT TICKER

#### Bảng Đối Soát 3 Cột:

| Yếu Tố Cấu Thành | Hiện Trạng (Bản Dev Demo - Netlify) | Mục Tiêu (Bản Design Reference - Topaz) | Đánh Giá Kỹ Thuật & CSS Blueprint Chuẩn Hóa |
|---|---|---|---|
| **Danh Mục Đối Tác (Integrity)** | **Chứa logo đối tác chưa ký kết chính thức**: Vinmec, Cisco, Microsoft, Fortinet, BIDV, Vietcombank, Medlatec, Viện KH Y Dược. | **100% Khách hàng & Cơ quan thật theo HSNL 2026**: BV Phổi, TTYT Liên Chiểu, Ngũ Hành Sơn, Cẩm Lệ, BV Phụ sản - Nhi, Chi cục Dân số, Cloud ACE, MobiFone, PVcomBank... | **LỖI P0 PHÁP LÝ**: Thanh lọc toàn bộ 100% đối tác không có hợp đồng. Sử dụng trọn bộ 11 logo vector/PNG chất lượng cao đã trích xuất từ bản Design Topaz (`audit_teknova/assets/partners/`). |
| **Thiết Kế Thẻ Đối Tác (Pill Card)** | Chỉ có logo đen trắng xám xịt đặt trơ trọi trên nền, không có thông tin ngữ cảnh. | Thiết kế dạng `partner-pill`: Logo nằm trong hộp bảo vệ nền trắng bo góc `w-10 h-10`, bên cạnh có tên đơn vị và tên phân hệ đã triển khai. | Cấu trúc component thẻ đối tác: <br>`<div class="flex items-center gap-3 px-4 py-2.5 rounded-xl bg-white border border-slate-200 shadow-xs hover:border-blue-400 transition-all shrink-0">` <br>`<img src="/assets/img/partners/bv_phoi.png" class="w-8 h-8 object-contain">` <br>`<div class="text-left"><p class="text-xs font-bold text-slate-800">BV Phổi Đà Nẵng</p><p class="text-[10px] text-slate-500">Bệnh án điện tử EMR</p></div></div>` |
| **Chuyển Động (Animation)** | Chạy giật cục, thiếu lớp gradient làm mờ ở 2 mép container. | Infinite Marquee chạy mượt mà ở chu kỳ 35-40s, 2 bên phủ gradient che mờ (`from-surface to-transparent`), tự dừng khi di chuột (pause on hover). | Sử dụng CSS keyframes: <br>`@keyframes marquee { 0% { transform: translateX(0%); } 100% { transform: translateX(-50%); } }` <br>`.animate-marquee { animation: marquee 35s linear infinite; }` <br>`.animate-marquee:hover { animation-play-state: paused; }` |

#### Danh Mục Tài Sản Logo Đối Tác Đã Sẵn Sàng Bàn Giao Dev (Trong `audit_teknova/assets/partners/`):
1. `bv_phoi_clean.png` (82.2 KB) — Bệnh viện Phổi Đà Nẵng (Dự án EMR & Zalo OA)
2. `bv_phusan_nhi_clean.png` (70.9 KB) — Bệnh viện Phụ sản - Nhi Đà Nẵng (Trả kết quả xét nghiệm Zalo)
3. `ttyt_lienchieu_clean.png` (53.7 KB) — Trung tâm Y tế Khu vực Liên Chiểu (Đơn thuốc điện tử TT 26 & QĐ 130)
4. `ttyt_nguhanhson_clean.png` (69.7 KB) — Trung tâm Y tế Khu vực Ngũ Hành Sơn (Thuê phần mềm EMR)
5. `ttyt_camle_clean.png` (50.0 KB) — Trung tâm Y tế Khu vực Cẩm Lệ (Nâng cấp trích xuất XML QĐ 3176)
6. `chicuc_danso_clean.png` (39.3 KB) — Chi cục Dân số TP. Đà Nẵng (Cơ sở dữ liệu dân số 56 xã/phường)
7. `danang_gov_clean.png` (44.8 KB) — Trung tâm CĐS & Công nghệ Chiến lược ĐN / UBND P. Ngũ Hành Sơn
8. `cloud_ace_clean.png` (9.4 KB) — Công ty TNHH Cloud ACE (Cổng thông tin & Mobile App Google Cloud Premier)
9. `bv_yhoccotruyen_clean.png` (46.0 KB) — Bệnh viện Y học Cổ truyền Đà Nẵng (Cổng thông tin bệnh viện)
10. `mobifone_clean.png` (9.9 KB) — MobiFone Đà Nẵng (Phần mềm hành chính công Zalo Mini App)
11. `pvcombank_icon.png` (17.2 KB) — Ngân hàng PVcomBank (Fintech thanh toán viện phí Kiosk)


---

### BLOCK 5: 6 TRỤ CỘT LĨNH VỰC HOẠT ĐỘNG (CORE DOMAINS BENTO GRID)

#### Bảng Đối Soát 3 Cột:

| Yếu Tố Cấu Thành | Hiện Trạng (Bản Dev Demo - Netlify) | Mục Tiêu (Bản Design Reference - Topaz) | Đánh Giá Kỹ Thuật & CSS Blueprint Chuẩn Hóa |
|---|---|---|---|
| **Cấu Trúc Khối (Redundancy)** | **Thừa thãi 2 khối liên tiếp**: <br>1. "6 Lĩnh vực cốt lõi" (Lưới 6 card)<br>2. "Các bài toán tập trung" (5 card trùng lặp). | **1 Khối Bento Grid duy nhất gồm 6 Trụ Cột**: Bố cục chặt chẽ, không bị loãng trang, phân cấp rõ rệt vai trò từng trụ cột. | Xóa bỏ hoàn toàn khối "Các bài toán tập trung" bị trùng lặp; gộp toàn bộ giải pháp mũi nhọn vào lưới 6 Bento Card chuẩn mực. |
| **Card Điểm Nhấn (Hero Accent Card)** | Cả 6 card đều dùng màu nền trắng nhờ nhờ giống hệt nhau; không có card nào làm điểm tựa thị giác. | **Card 4 (Chuyển đổi số - AI - Big Data - Cloud)** được phủ màu xanh Cobalt nguyên khối `bg-primary text-white`, bóng đổ sâu, icon trắng, nhãn vàng "Nổi Bật". | Thiết lập Card 4 thành Hero Anchor: <br>`class="col-span-1 md:col-span-2 lg:col-span-1 rounded-2xl p-6 bg-gradient-to-br from-blue-600 to-indigo-700 text-white shadow-xl shadow-blue-500/20 relative overflow-hidden group"` |
| **Hệ Thống Icon & Micro-Interaction** | Icon ảnh bitmap độ phân giải thấp, không có tương tác phản hồi khi rê chuột. | Icon phong cách kỹ thuật (Google Material Symbols / Lucide SVG), hiệu ứng nhấc thẻ 6px (`card-elevate`), icon phóng to 112% (`icon-bounce`). | Bổ sung class tương tác CSS: <br>`transition-all duration-300 ease-out hover:-translate-y-1.5 hover:shadow-lg hover:border-blue-300`. |

---

### BLOCK 6: DỰ ÁN TIÊU BIỂU & CASE STUDIES (CRITICAL GAP)

#### Bảng Đối Soát 3 Cột:

| Yếu Tố Cấu Thành | Hiện Trạng (Bản Dev Demo - Netlify) | Mục Tiêu (Bản Design Reference - Topaz) | Đánh Giá Kỹ Thuật & CSS Blueprint Chuẩn Hóa |
|---|---|---|---|
| **Tình Trạng Ảnh Thumbnail** | **LỖI P0 BLOCKER: 100% ẢNH THUMBNAIL BỊ TRẮNG TOÁT**. Link Google Public Storage bị hết hạn token xác thực và chặn CORS. | Hình ảnh sắc nét chuẩn 16:9, chụp hiện trường phòng mổ, buồng khám, Kiosk đón tiếp thực tế tại các bệnh viện Đà Nẵng. | **Khắc phục ngay lập tức**: Chuyển đổi toàn bộ đường dẫn ảnh sang thư mục cục bộ `public/assets/img/projects/emr_hospital.jpg`, `tt26_prescription.jpg`, `zalo_oa_his.jpg`... Tuyệt đối không dùng URL CDN ngoài tạm bợ. |
| **Phân Loại & Căn Cứ Pháp Lý** | Chỉ có nhãn text mờ nhạt ("Y Tế Thông Minh", "Hành Chính"). | Mỗi dự án gắn liền với huy hiệu pháp lý cụ thể: `Thông tư 46/2018`, `Thông tư 26/2025`, `QĐ 3176/QĐ-BYT`, `QĐ 130/QĐ-BYT`. | Bổ sung dải badge pháp lý trên đầu mỗi thẻ dự án: <br>`<span class="px-2.5 py-1 rounded-md text-[11px] font-bold bg-blue-50 text-blue-700 border border-blue-200">TT 46/2018/TT-BYT</span>` |
| **Tương Tác Khi Nhấp Chuột** | Nhấp vào không có bất kỳ phản hồi nào; thẻ dự án chỉ đóng vai trò text tĩnh. | Nhấp vào thẻ kích hoạt **Slide-Over Drawer mở từ cạnh phải**, hiển thị hồ sơ nghiệm thu 8 tầng thông tin và deep-link URL. | Tích hợp tính năng Case Study Detail Drawer (xem đặc tả kỹ thuật chi tiết tại Mục 6.3). |

---

### BLOCK 7: BAN LÃNH ĐẠO & TRIẾT LÝ VẬN HÀNH (CRITICAL GAP)

#### Bảng Đối Soát 3 Cột:

| Yếu Tố Cấu Thành | Hiện Trạng (Bản Dev Demo - Netlify) | Mục Tiêu (Bản Design Reference - Topaz) | Đánh Giá Kỹ Thuật & CSS Blueprint Chuẩn Hóa |
|---|---|---|---|
| **Sự Hiện Diện Của Lãnh Đạo** | **LỖI P0 BLOCKER: CẮT BỎ 100% KHỐI LÃNH ĐẠO**. Chỉ có một ô text vuông xanh đen vô danh ghi "Ban Lãnh Đạo TEKNOVA". | Khối Chân dung Lãnh đạo bề thế chia 2 cột: Cột trái (7 cols) thông điệp và 3 cam kết; Cột phải (5 cols) chân dung cắt nền CEO. | **Tái lập toàn diện khối Lãnh đạo**. Khẳng định vai trò của Chủ tịch kiêm Tổng Giám đốc **Trần Bình Sơn (MBA, Kỹ sư Điện tử, >20 năm KN)**. |
| **Hình Ảnh Chân Dung Lãnh Đạo** | Hoàn toàn không có hình ảnh người thật. | Ảnh chân dung cắt nền (Cutout Portrait) chất lượng cao mặc veston lịch thiệp, đặt đứng chạm sàn, xếp lớp trên khối họa tiết lam ngọc. | Sử dụng file ảnh cắt nền `/ceo-cutout.png` chất lượng cao, đổ bóng đa tầng: `filter drop-shadow-[0_20px_30px_rgba(15,23,42,0.15)]`. |
| **Cam Kết Hành Động & Trust Seal** | Không có cam kết nào cụ thể. | 3 Luận điểm hành động đanh thép + Quote triết lý nghiệp vụ + Con dấu niềm tin (Trust Seal) chiếc khiên xanh ngọc. | Khắc họa 3 cam kết hành động: <br>1. *Hơn 20 năm thâm niên Viễn thông - CNTT và tư vấn y tế số*.<br>2. *Chỉ đạo chuyển giao 22+ dự án phần mềm và chính quyền số*.<br>3. *Bảo chứng tuyệt đối tôn chỉ: "Thực Người • Thực Việc • Thực Giá Trị"*. |

---

### BLOCK 8: FOOTER & CTA BANNER CUỐI TRANG

#### Bảng Đối Soát 3 Cột:

| Yếu Tố Cấu Thành | Hiện Trạng (Bản Dev Demo - Netlify) | Mục Tiêu (Bản Design Reference - Topaz) | Đánh Giá Kỹ Thuật & CSS Blueprint Chuẩn Hóa |
|---|---|---|---|
| **Tone Màu Banner CTA** | Nền màu xanh đen thẫm `bg-[#0b1c30]` gây tối tăm, phá vỡ nhịp điệu ánh sáng của tổng thể Light Theme. | Banner bo góc `rounded-3xl` phủ gradient xanh cobalt rực rỡ (`from-blue-600 via-indigo-600 to-blue-700`), hiệu ứng ánh sáng tỏa tròn. | Thay thế background xanh đen bằng: <br>`class="rounded-3xl p-8 sm:p-12 bg-gradient-to-r from-blue-600 via-blue-700 to-indigo-800 text-white shadow-2xl relative overflow-hidden"`. |
| **Minh Bạch Trụ Sở Doanh Nghiệp** | Chỉ ghi địa chỉ ĐKKD cũ: `K131/18 Lý Thái Tổ`. **Thiếu hoàn toàn trụ sở làm việc chính thức**. | Hiển thị song song 2 địa chỉ chuẩn mực: <br>• **VP Trụ sở chính**: Tầng 3, 456 Nguyễn Hữu Thọ, Cẩm Lệ, Đà Nẵng.<br>• **Địa chỉ ĐKKD**: K131/18 Lý Thái Tổ, Thanh Khê, Đà Nẵng. | Chuẩn hóa thông tin văn phòng làm việc để cán bộ các bệnh viện và cơ quan dễ dàng tới khảo sát thực địa. |
| **Mã Số Doanh Nghiệp (MST)** | Bị ẩn hoàn toàn ở Footer (trong code cũ từng có số giả `0402123456`). | Hiển thị rõ ràng ở dòng bản quyền: `Mã số thuế: 0402300331`. | Cập nhật dòng bản quyền cuối trang: <br>`© 2026 CÔNG TY CỔ PHẦN ĐỔI MỚI SÁNG TẠO TEKNOVA. Mã số doanh nghiệp: 0402300331 cấp ngày 23/09/2025 tại Sở KH&ĐT TP. Đà Nẵng.` |

---

### 3.9 ĐÁNH GIÁ HIỆU ỨNG HOVER & SCROLL: TÍNH THỰC TẾ & ĐỘ CHUYÊN NGHIỆP TRONG SHOWCASE B2G (MARKETING TO DEV OBSERVATIONS)

Từ trải nghiệm thực tế của đội ngũ Marketing khi trực tiếp cầm laptop/tablet đi demo giải pháp trước các bác sĩ, ban giám đốc và hội đồng thẩm định, các hiệu ứng vi mô (micro-interactions) như **Hover** và **Scroll** đóng vai trò quyết định cảm giác "phần mềm xịn, mượt mà" hay "web tĩnh sơ sài":

#### 1. Đánh Giá Hiện Trạng Hiệu Ứng Scroll (Scroll Experience Audit)

* **Hiện trạng Bản Dev Demo (`teknova-demo`)**:
  - *Cảm giác cuộn*: Sử dụng cơ chế Native Scroll mặc định của trình duyệt (`overflow-y: auto`). Khi cuộn trên chuột rời (mouse wheel) hoặc trackpad máy tính Windows, nhịp cuộn bị giật từng khấc (stepping scroll), thiếu độ hãm quán tính.
  - *Hiệu ứng xuất hiện (Scroll Trigger)*: Không có hiệu ứng fade-in hay trượt nhẹ khi lướt qua các section. Toàn bộ nội dung hiện diện tĩnh ngay từ đầu, tạo cảm giác thiếu chiều sâu và hơi khô cứng đối với một website công nghệ cao.
* **Hiện trạng Bản Design Reference (`teknova-topaz`)**:
  - *Cảm giác cuộn*: Đã tích hợp thư viện **Lenis Smooth Scroll** (`window.lenis = true`). Thao tác cuộn chuột có độ đầm, quán tính dừng êm ái (damping factor ~0.1), mang lại cảm giác lướt rất cao cấp như các trang giới thiệu sản phẩm của Apple hay Stripe.
  - *Điểm cần lưu ý thực tế (Marketing Observation)*: 
    > *"Lenis cuộn rất êm và sang, nhưng khi trình chiếu trên máy chiếu phòng họp có tần số quét thấp (60Hz hoặc qua cổng HDMI/VGA cũ), hiệu ứng smooth scroll nếu cấu hình quán tính quá dài có thể gây cảm giác 'trôi tuột' hoặc hơi trễ tay (laggy feel) khi cần dừng nhanh để chỉ vào một con số cụ thể."*
* **Đề xuất kỹ thuật khiêm tốn gửi đội Dev (Dev Recommendations)**:
  - **Khuyến nghị 1 (Smooth Scroll vừa phải)**: Bổ sung thư viện Lenis vào bản Dev nhưng tinh chỉnh thông số:
    ```javascript
    // Cấu hình Lenis cân bằng giữa độ mượt và độ chính xác thực chiến
    const lenis = new Lenis({
      duration: 1.1,           // Thời gian hãm quán tính vừa phải (mặc định 1.2s dễ gây trôi)
      easing: (t) => Math.min(1, 1.001 - Math.pow(2, -10 * t)),
      orientation: 'vertical',
      gestureOrientation: 'vertical',
      smoothWheel: true,
      wheelMultiplier: 1.0,    // Giữ tỉ lệ 1.0 để người dùng cuộn tới đâu kiểm soát được tới đó
      touchMultiplier: 1.5,
    });
    ```
  - **Khuyến nghị 2 (Top Progress Bar)**: Bản Design có dải thanh tiến trình mỏng màu xanh trên đỉnh đầu trang (`h-[2px] bg-primary z-50 fixed top-0`) hiển thị % trang đã cuộn. Đây là chi tiết cực kỳ tinh tế, giúp người xem biết mình đang ở đoạn nào của bài thuyết trình. Đề xuất Dev đưa component này vào `AppHeader.vue`.

---

#### 2. Đánh Giá Hiện Trạng Hiệu Ứng Hover (Hover & Micro-Interactions Audit)

Trong môi trường B2G y tế, người dùng (đặc biệt là các bác sĩ và cán bộ quản lý) cần **sự phản hồi thị giác rõ ràng (Tactile Feedback)** để biết phần tử nào click được, phần tử nào là dữ liệu tham khảo:

* **Bảng Đối Soát Hiệu Ứng Hover Giữa 2 Bản**:

| Thành Phần Giao Diện | Hiện Trạng Bản Dev Demo | Bản Design Reference (Topaz) | Nhận Xét Thực Tế Từ Marketing & Đề Xuất Cho Dev |
|---|---|---|---|
| **Các Nút Bấm Chính (Primary CTA)** | Đổi màu nền đơn giản (`hover:bg-blue-700`), không có chuyển dịch vị trí hay đổ bóng. | Đổ bóng phát quang (`glow-btn`), nâng nhẹ 1px, hiệu ứng mũi tên trượt sang phải 3px (`group-hover:translate-x-1`). | **Rất tốt trên Design**: Hiệu ứng mũi tên chuyển động giúp người xem có động lực bấm thử. Đề xuất Dev áp dụng class: `transition-all duration-200 hover:-translate-y-0.5 hover:shadow-lg hover:shadow-blue-500/25 active:translate-y-0`. |
| **Thẻ Trụ Cột Lĩnh Vực (Domain Cards)** | Không đổi trạng thái hoặc chỉ đổi màu viền rất mờ nhạt. | Nâng cao 6px (`-translate-y-1.5`), bóng đổ lan rộng `shadow-xl`, icon dịch chuyển nhẹ. | **Cần sự chừng mực**: Nâng 6px là vừa vặn, không nên lạm dụng phóng to (`scale-105`) vì sẽ làm che khuất chữ của card bên cạnh trên màn hình 1366x768. |
| **Dải Logo Đối Tác (Partner Pills)** | Đứng yên hoặc chạy giật cục; rê chuột vào không có phản ứng. | Khi rê chuột vào dải marquee: **Toàn bộ dải tự dừng lại (Pause on Hover)**; logo bên trong phóng to nhẹ 110% (`scale-110`). | **Tính năng Showcase then chốt**: Khi đối tác hỏi *"Ủa các bạn làm cho Bệnh viện Phổi gói nào?"*, người thuyết trình rê chuột vào để dải dừng lại, trỏ chuột cho khách xem. Đề xuất Dev bắt buộc giữ `hover:pause-animation`. |
| **Thẻ Dự Án (Case Study Cards)** | Rê chuột vào không có con trỏ `cursor-pointer`, cảm giác như ảnh tĩnh chết. | Thẻ nổi khối, ảnh thumbnail zoom chậm 105% (`group-hover:scale-105 transition-transform duration-500`), mũi tên góc thẻ xoay chéo 45 độ. | **Rất trực quan**: Báo hiệu cho khách biết thẻ này có thể bấm để xem chi tiết nghiệm thu bên trong. |
| **Thực Đơn Điều Hướng (Nav Links)** | Đổi màu chữ xanh thông thường. | Đổi màu chữ xanh đậm thương hiệu + gạch chân mờ chuyển động mượt mà. | Gợi ý Dev thêm hiệu ứng thanh line trượt nhẹ dưới chân menu để tăng độ tinh tế. |

---

#### 3. Tiêu Chuẩn Thực Tế & Chuyên Nghiệp (Professionalism & Pragmatism Standard)

Từ kinh nghiệm thực chiến B2G, Bộ phận Marketing xin tổng kết 3 nguyên tắc "vàng" về mặt hiệu ứng để trang web đạt chuẩn mực cao nhất:
1. **Nguyên tắc "Không lạm dụng chuyển động rườm rà (No Over-Animation)"**: Tránh các hiệu ứng xoay lật 3D quá đà, nảy tưng bừng hay giật màn hình. Đối tượng khách hàng là Bác sĩ, Giám đốc Bệnh viện và Cơ quan nhà nước luôn đánh giá cao sự **điềm đạm, vững chãi, tốc độ phản hồi dứt khoát (< 250ms)** hơn là sự phô trương kỹ xảo.
2. **Nguyên tắc "Tôn trọng thiết bị yếu & Màn hình cảm ứng"**: Các hiệu ứng hover chỉ kích hoạt trên thiết bị có chuột (`@media (hover: hover)`), tránh bị "kẹt trạng thái hover" (sticky hover bug) khi khách hàng vuốt chạm trên iPad/máy tính bảng.
3. **Nguyên tắc "Đồng nhất nhịp điệu (Cohesive Timing Function)"**: Toàn bộ chuyển đổi hover nên dùng chung một hàm gia tốc `cubic-bezier(0.16, 1, 0.3, 1)` với thời gian `200ms - 300ms` để tạo cảm giác toàn bộ giao diện là một khối thống nhất, mượt mà và đẳng cấp.

---

## 4. ĐÁNH GIÁ TRẢI NGHIỆM THAO TÁC & RÀO CẢN SHOWCASE B2G (UX & SHOWCASE READINESS)

### 4.1 Phân Tích Tâm Lý & Nỗi Đau Của 4 Đối Tượng Mục Tiêu (Persona Pain Points)

Khi website được mở trên máy chiếu phòng họp hay máy tính bảng trong các buổi làm việc chính thức, 4 nhóm đối tượng có những mối quan tâm chuyên sâu cần được giải tỏa:

```text
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                 BẢN ĐỒ THẤU CẢM 4 ĐỐI TƯỢNG B2G                                 │
├───────────────────────────────────┬─────────────────────────────────────────────────────────────┤
│ 1. GIÁM ĐỐC BỆNH VIỆN             │ • Sợ triển khai dở dang, gián đoạn khám chữa bệnh.          │
│    (Đại diện chủ đầu tư)          │ • Ám ảnh xuất toán BHYT hàng tỷ đồng do lệch giờ ký, sai mã │
│                                   │   ICD-10 vs Dược thư, vượt CCHN bác sĩ và trùng chỉ định.   │
│                                   │ • Bế tắc vốn đầu tư công CAPEX -> Cần mô hình thuê OPEX QĐ80│
├───────────────────────────────────┼─────────────────────────────────────────────────────────────┤
│ 2. TRƯỞNG PHÒNG CNTT BỆNH VIỆN    │ • Sợ xung đột dữ liệu với HIS hiện hữu (VNPT, Viettel).     │
│    (Chịu trách nhiệm kỹ thuật)    │ • Lo ngại hệ thống sập ban đêm, nhà thầu ở xa không hỗ trợ. │
│                                   │ • Đòi hỏi chuẩn XML QĐ 130 và chứng nhận ATTT Cấp độ 3.     │
├───────────────────────────────────┼─────────────────────────────────────────────────────────────┤
│ 3. LÃNH ĐẠO SỞ Y TẾ / CHÍNH QUYỀN │ • Áp lực hoàn thành chỉ tiêu Đề án 06/CP và DTI của tỉnh.   │
│    (Cơ quan quản lý nhà nước)     │ • Yêu cầu dữ liệu đồng bộ 56 xã/phường không phân mảnh.     │
│                                   │ • Kiểm tra gắt gao tính chính danh, bằng cấp và MST thầu.   │
├───────────────────────────────────┼─────────────────────────────────────────────────────────────┤
│ 4. NHÀ ĐẦU TƯ & ĐỐI TÁC TELCO     │ • Đánh giá năng lực liên danh thầu chuyên môn y tế.         │
│    (MobiFone, Cloud ACE, PVcom)   │ • Thẩm tra chất xám của đội ngũ R&D và quyền sở hữu trí tuệ.│
│                                   │ • Năng lực mở rộng sản phẩm từ Đà Nẵng ra toàn quốc.        │
└───────────────────────────────────┴─────────────────────────────────────────────────────────────┘
```

#### 1. Giám Đốc Bệnh Viện:
* *Nỗi sợ lớn nhất*: Quyết định bỏ bệnh án giấy theo Thông tư 46 là quyết định mang tính sinh mệnh của bệnh viện. Nếu hệ thống EMR mới hoạt động chập chờn, bác sĩ phản đối, bệnh nhân ùn ứ, bảo hiểm xã hội từ chối thanh toán thì Giám đốc là người chịu trách nhiệm trực tiếp trước Sở Y tế và pháp luật. Đặc biệt, nỗi ám ảnh lớn nhất của Giám đốc Bệnh viện Hạng I là **nguy cơ xuất toán BHYT hàng tỷ đồng** — không chỉ vì sai lệch dấu thời gian TSA mà chủ yếu do:
  1. *Chẩn đoán ICD-10 không phù hợp chỉ định thuốc theo Dược thư Quốc gia (TT 20/2022/TT-BYT)*;
  2. *Chỉ định kỹ thuật hoặc kê đơn vượt quá phạm vi chuyên môn trên Chứng chỉ hành nghề (CCHN) của bác sĩ*;
  3. *Trùng lặp chỉ định thuốc, xét nghiệm trong cùng đợt khám / 24 giờ*.
* *Kỳ vọng trên Portal*: Phải nhìn thấy **bằng chứng sống động về quy trình vận hành trơn tru** tại các bệnh viện tương đương (như BV Phổi Đà Nẵng); chứng minh năng lực của **Module Pre-Audit Rule Engine (Hệ thống Tiền Giám Định Lâm Sàng)** kiểm soát rủi ro xuất toán tự động ngay lúc bác sĩ ra y lệnh; đồng thời hiểu rõ phương án thuê dịch vụ CNTT theo Quyết định 80/2014 để ký hợp đồng ngay từ nguồn thu viện phí thường niên mà không phải chờ duyệt ngân sách đầu tư công 2-3 năm.

#### 2. Trưởng Phòng CNTT Bệnh Viện:
* *Nỗi sợ lớn nhất*: Nhà cung cấp phần mềm "hứa thật nhiều nhưng làm không được bao nhiêu". Bệnh viện đang vận hành HIS hiện hữu của các hãng lớn, việc tích hợp thêm EMR hoặc cổng đơn thuốc Thông tư 26 nếu bị lỗi đồng bộ dữ liệu sẽ làm tê liệt toàn bộ khâu thanh toán ra viện.
* *Kỳ vọng trên Portal*: Cần công cụ xem trực tiếp cấu trúc gói tin (Payload Inspector), chứng minh độ trễ liên thông < 0.8 giây, cơ chế hàng đợi bất đồng bộ (Async Queue) tự phục hồi khi cổng Bộ Y tế rớt mạng và thông số ký số tập trung Cloud CA.

#### 3. Lãnh Đạo Sở Y Tế & Chính Quyền Địa Phương:
* *Nỗi sợ lớn nhất*: Nhà thầu kê khai khống năng lực, đưa logo các đơn vị không có thực để lừa dối cơ quan quản lý; nhân sự đăng ký trong hồ sơ thầu không có bằng cấp chuyên ngành hoặc là tên mượn.
* *Kỳ vọng trên Portal*: Tính minh bạch 100%. Phải tra cứu được mã số thuế `0402300331`, trụ sở làm việc tại số 456 Nguyễn Hữu Thọ, tên Chủ tịch Trần Bình Sơn trùng khớp giấy phép ĐKKD, xem được bản scan bằng cấp của 12 chuyên gia và hồ sơ 22 hợp đồng thật trên địa bàn.

#### 4. Nhà Đầu Tư & Đối Tác Tổng Thầu Viễn Thông (MobiFone, Cloud ACE, PVcomBank):
* *Kỳ vọng trên Portal*: Nhìn thấy kiến trúc phần mềm hiện đại, khả năng tùy biến giải pháp linh hoạt và cam kết SLA dịch vụ chặt chẽ để yên tâm ký kết hợp đồng hợp tác chiến lược hoặc liên danh tham gia các gói thầu lớn.

---

### 4.2 Năm Điểm Nghẽn Gây Nghi Ngờ Tính Xác Thực Trên Web Cũ & Chiến Lược Khắc Phục

1. **Điểm nghẽn 1: Thiếu minh chứng vận hành tương tác trực tiếp (Static Mockup Skepticism)**:
   * *Thực trạng*: Khách hàng chỉ thấy các ảnh chụp màn hình bất động, nghi ngờ đây là các bản vẽ Photoshop tải từ trên mạng về.
   * *Chiến lược khắc phục*: Tích hợp **Tính năng 1: Interactive Live Hospital Flow Mockup** mô phỏng sống động 5 bước khám chữa bệnh có thể nhấp chuột điều khiển, xem gói tin JSON thật và thử nghiệm cơ chế ngắt mạng tự phục hồi.
2. **Điểm nghẽn 2: Thẻ dự án nông cạn, mất ảnh thumbnail (Broken Thumbnails & Shallow Proof)**:
   * *Thực trạng*: 100% ảnh thumbnail dự án trên bản Dev bị trắng toát; nhấp vào không có thông tin chi tiết.
   * *Chiến lược khắc phục*: Thay thế toàn bộ bằng ảnh chụp thực tế lưu trữ cục bộ; tích hợp **Tính năng 3: Case Study Detail Drawer** mở ngăn kéo 8 tầng thông tin chiều sâu cho đủ 22 hợp đồng.
3. **Điểm nghẽn 3: Khủng hoảng nhận diện nhân thân lãnh đạo (Identity Crisis)**:
   * *Thực trạng*: Bản Dev giấu sạch lãnh đạo; bản Design đổi tên Chủ tịch thành "Nguyễn Hùng Sơn" hư cấu.
   * *Chiến lược khắc phục*: Tái lập toàn diện khối Lãnh đạo với chân dung cutout của ông **Trần Bình Sơn (MBA, Kỹ sư Điện tử)**; tích hợp **Tính năng 4: Team Showcase Tab** hiển thị đủ 12 nhân sự và văn bằng scan thẩm định.
4. **Điểm nghẽn 4: Rào cản tiếp cận hồ sơ năng lực (Profile Download Barrier)**:
   * *Thực trạng*: Chỉ có link tải file PDF dung lượng lớn, cán bộ không thể xem nhanh trên trình duyệt trong các buổi hội ý ngắn.
   * *Chiến lược khắc phục*: Xây dựng **Tính năng 2: In-browser Profile PDF Viewer / Flipbook** lật trang 3D siêu tốc (< 0.5s) kèm cổng thu thập đầu mối (Lead Capture) nhẹ nhàng khi tải bản dấu đỏ.
5. **Điểm nghẽn 5: Form đăng ký bán lẻ generic, thiếu cam kết thời gian (No-SLA Generic Form)**:
   * *Thực trạng*: Form liên hệ đơn điệu như web bán hàng tiêu dùng, không có phân loại cơ sở y tế và không có cam kết thời gian liên hệ lại.
   * *Chiến lược khắc phục*: Thiết kế **Tính năng 5: Direct Demo Booking Form** phân hạng bệnh viện (Hạng I, Hạng II, TTYT) và đưa ra cam kết văn bản Kỹ sư trưởng phản hồi trong vòng 24 giờ làm việc.

---

## 5. DEV ACTION PLAN & MA TRẬN PHÂN LOẠI MỨC ĐỘ NGHIÊM TRỌNG (SEVERITY MATRIX & REMEDIATION BLUEPRINT)

### 5.1 Ma Trận Phân Loại Mức Độ Nghiêm Trọng Chi Tiết

Bảng dưới đây phân loại toàn bộ các vấn đề kỹ thuật và nội dung cần xử lý trong đợt nâng cấp, xếp theo 4 cấp độ ưu tiên: **P0 (Blocker) -> P1 (Critical) -> P2 (Major) -> P3 (Minor)**:

| Mã Lỗi | Tên Vấn Đề Cần Khắc Phục | Phân Hạng | Vị Trí Tệp Cần Chỉnh Sửa | Giải Pháp Kỹ Thuật & CSS Specs Cụ Thể | Thời Gian Dự Kiến |
|:---:|---|:---:|---|---|:---:|
| **P0-01** | **Chuẩn hóa thông tin Lãnh đạo & Cập nhật đầy đủ 12 nhân sự** | **P0 (Blocker)** | `teknova-data.ts`, `HomeView.vue`, `LeadershipSection.vue` | Khôi phục tên **Trần Bình Sơn** (MBA, Kỹ sư Điện tử), chèn ảnh cutout `/ceo-cutout.png`, bổ sung đầy đủ 12 nhân sự (đặc biệt KS. Trần Ngọc Trai >20 năm KN và Bùi Thị Mai). | **4 Man-hours** |
| **P0-02** | **Trắng toát 100% thumbnail dự án tại Block 6 trên Netlify** | **P0 (Blocker)** | `HomeView.vue:240-310`, `public/assets/img/projects/` | Tải và lưu trữ vĩnh viễn 6 ảnh thumbnail chuẩn 16:9 vào thư mục cục bộ `public/assets/img/projects/`; thay thế toàn bộ link `lh3.googleusercontent.com` bằng đường dẫn nội bộ. | **3 Man-hours** |
| **P1-01** | **Bỏ sót 16/22 hợp đồng thực tế từ HSNL 2026** | **P1 (Critical)** | `teknova-data.ts:250-450`, `CaseStudies.vue` | Nạp toàn bộ 22 hợp đồng từ SSOT vào cấu trúc mảng `PROJECTS_ROSTER`, phân 3 tabs: Y tế (10 HĐ), Chính quyền (8 HĐ), Doanh nghiệp (4 HĐ). | **6 Man-hours** |
| **P1-02** | **Cập nhật logo đối tác chính thức & Thay thế case study theo hợp đồng thực tế** | **P1 (Critical)** | `HomeView.vue:150-185`, `teknova-data.ts:353-388` | Xóa sạch logo Vinmec, Cisco, Microsoft, Fortinet, BIDV, Vietcombank. Thay bằng 12 logo thật (BV Phổi, TTYT Liên Chiểu...). Xóa case study Dược Miền Trung, thay bằng Cloud ACE hoặc MobiFone. | **3 Man-hours** |
| **P1-03** | **Hero Section bị ép thành 2 cột làm biến dạng mockup EMR** | **P1 (Critical)** | `HomeView.vue:60-140`, `HeroSection.vue` | Tái cấu trúc Hero sang dạng Monumental Centered 1200px: Text tiêu đề căn giữa `max-w-4xl`, đặt mockup EMR Panorama trải rộng phía dưới kèm 2 floating badges. | **5 Man-hours** |
| **P2-01** | **Khắc phục hiển thị giá trị mặc định `00+` trên dải số liệu thành tựu** | **P2 (Major)** | `CounterSection.vue`, `nav-router.js` | Sửa logic đếm số NaN; cấu hình giá trị khởi tạo an toàn: `>20 Năm`, `22+ Dự án`, `12 Chuyên gia`, `100% Nghiệm thu`. | **2 Man-hours** |
| **P2-02** | **Khối Lĩnh vực hoạt động bị trùng lặp 2 lần liên tiếp** | **P2 (Major)** | `HomeView.vue:190-235` | Xóa bỏ khối "Các bài toán TEKNOVA tập trung"; chuyển sang Bento Grid 6 ô duy nhất với Card 4 (AI/Cloud) phủ màu xanh Cobalt `bg-primary` nổi bật. | **3 Man-hours** |
| **P2-03** | **Footer và Header thiếu thông tin trụ sở chính và MST** | **P2 (Major)** | `AppFooter.vue`, `AppHeader.vue` | Bổ sung trụ sở chính: `Tầng 3, 456 Nguyễn Hữu Thọ, Cẩm Lệ, Đà Nẵng` và `Mã số thuế: 0402300331`. Thêm nút Tải Profile PDF trên Header. | **2 Man-hours** |
| **P3-01** | **Banner CTA cuối trang mang màu xanh đen `#0b1c30` tối tăm** | **P3 (Minor)** | `HomeView.vue:420-460` | Đổi sang gradient xanh cobalt rực rỡ `bg-gradient-to-r from-blue-600 via-blue-700 to-indigo-800`, bo góc lớn `rounded-3xl`. | **1 Man-hour** |
| **P3-02** | **Thiếu liên kết giao thức gọi điện thoại trực tiếp `tel:`** | **P3 (Minor)** | `AppHeader.vue`, `AppFooter.vue` | Bọc số hotline `0935 722 579` trong thẻ `<a href="tel:0935722579">`. | **0.5 Man-hour** |

---

### 5.2 Hướng Dẫn Kỹ Thuật Di Chuyển Tài Nguyên Ảnh Sang Thư Mục Cục Bộ (Local Assets Migration Guide)

Để chấm dứt vĩnh viễn vấn đề đường dẫn ảnh CDN bên thứ ba bị hết hạn token xác thực hoặc bị chặn bảo mật (Cross-Origin Resource Sharing - CORS), Đội Dev bắt buộc phải thực hiện quy trình chuẩn hóa tài nguyên theo các bước sau:

#### 1. Quy hoạch cấu trúc thư mục tài nguyên chuẩn:
```text
public/
├── assets/
│   ├── img/
│   │   ├── branding/
│   │   │   ├── logo_teknova_vector.svg
│   │   │   └── ceo_tran_binh_son_cutout.png
│   │   ├── mockups/
│   │   │   ├── emr_panorama_dashboard.webp
│   │   │   ├── kiosk_checkin_flow.webp
│   │   │   └── prescription_tt26_mobile.webp
│   │   ├── partners/
│   │   │   ├── bv_phoi_danang.png
│   │   │   ├── ttyt_lienchieu.png
│   │   │   ├── ttyt_nguhanhson.png
│   │   │   ├── ttyt_camle.png
│   │   │   ├── bv_phusan_nhi.png
│   │   │   ├── chicuc_danso.png
│   │   │   ├── cloud_ace.png
│   │   │   ├── mobifone_danang.png
│   │   │   └── pvcombank.png
│   │   └── projects/
│   │       ├── case_01_emr_bvphoi.webp
│   │       ├── case_02_tt26_lienchieu.webp
│   │       ├── case_03_zalo_his_phusan.webp
│   │       ├── case_04_danso_56phuong.webp
│   │       ├── case_05_camera_ai_dpmt.webp
│   │       └── case_06_cloudace_portal.webp
```

#### 2. Quy tắc tối ưu hóa định dạng ảnh & Khắc phục file CEO Cutout:
* Toàn bộ ảnh thumbnail và mockup phải được chuyển sang định dạng **WebP** với chất lượng `quality: 85%` để giảm dung lượng file xuống dưới 120KB mà vẫn giữ độ sắc nét hoàn hảo trên màn hình Retina 2x.
* Logo đối tác phải dùng định dạng **PNG trong suốt (transparent)** hoặc **SVG**, đặt vừa vặn trong khung bounding box `120x60px`.
* **Tối ưu hóa file CEO Cutout (`ceo-cutout.png`)**:
  - *Hiện trạng phát hiện*: File `teknova-portal/public/ceo-cutout.png` ban đầu nặng 1,028 KB (~1.03 MB), vượt quá 300% ngưỡng trần 350KB của tiêu chí AC-10.
  - *Quy chuẩn nén WebP & PNG*: 
    1. Xuất bản tệp WebP chất lượng 85% (`ceo-cutout.webp`, dung lượng nén đạt 92.3 KB, giảm 91% dung lượng).
    2. Nén tệp PNG gốc sử dụng thuật toán phân cấp lượng tử 256 màu FASTOCTREE (`ceo-cutout.png`, dung lượng nén đạt 156.9 KB, vượt qua ngưỡng kiểm định < 350KB) bảo toàn độ tương phản và kênh Alpha trong suốt.
  - Cấu trúc hiển thị HTML hỗ trợ nạp đa định dạng:
    ```html
    <picture>
      <source srcset="/ceo-cutout.webp" type="image/webp" />
      <img src="/ceo-cutout.png" alt="Chủ tịch HĐQT kiêm Tổng Giám đốc Trần Bình Sơn" class="w-full h-auto object-contain" />
    </picture>
    ```

#### 3. Đặc Tả Kiến Trúc Service Worker & CacheStorage (PWA Offline Resilience Cho Bệnh Viện):
* **Bối cảnh thực tế**: Khi kỹ sư Teknova pitching tại phòng họp giao ban tầng hầm, trung tâm dữ liệu hoặc hội trường bệnh viện có hạ tầng mạng nội bộ cách ly, không có sóng Wi-Fi/4G, trang web không có Service Worker sẽ lập tức bị báo lỗi kết nối mạng (màn hình "khủng long" offline).
* **Đặc tả cài đặt PWA & Service Worker (`sw.js`)**:
  - Tích hợp `vite-plugin-pwa` (Workbox) trong chu trình build Next.js / Vite.
  - Đăng ký Service Worker với các chiến lược bộ đệm theo nhóm tài nguyên:
    1. *App Shell (HTML, CSS, JS runtime, Font Inter/Plus Jakarta Sans)*: Áp dụng chiến lược `NetworkFirst` kèm fallback tức thì sang `CacheStorage` nếu mạng không phản hồi trong 800ms.
    2. *Tài nguyên Hình ảnh Cục bộ (`/public/assets/img/**`, `ceo-cutout.png`, `ceo-cutout.webp`)*: Áp dụng chiến lược `StaleWhileRevalidate` lưu trong Cache API (`teknova-image-cache-v1`).
    3. *Hồ sơ Năng lực In-browser Flipbook*: Pre-cache toàn bộ 18 trang WebP (`page_01.webp` đến `page_18.webp`) ngay khi Service Worker được kích hoạt lần đầu.
  - Bổ sung `manifest.json` đăng ký PWA, cho phép cài đặt portal như một Native Desktop App / Tablet App sẵn sàng trình diễn 100% Offline.
* **Giao diện phản hồi trạng thái mạng**: Khi ngắt kết nối internet, thanh điều hướng Header hiển thị pill badge màu cam: `[ ⚡ Ngoại Tuyến: Chế Độ Trình Diễn PWA CacheStorage Sẵn Sàng ]`.


---

## 6. ĐẶC TẢ KỸ THUẬT PRD CHO 5 TÍNH NĂNG NÂNG TẦM SHOWCASE

Dưới đây là bản đặc tả kỹ thuật chi tiết (Product Requirement Document - PRD) của 5 tính năng nâng cấp then chốt nhằm biến Cổng thông tin TEKNOVA thành công cụ trình diễn giải pháp B2G/B2B vượt trội:

```text
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                               5 TÍNH NĂNG TRÌNH DIỄN B2G ĐỘT PHÁ                                │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ TÍNH NĂNG 1: INTERACTIVE LIVE HOSPITAL FLOW MOCKUP (Mô phỏng 5 bước chu trình khám chữa bệnh)  │
│ TÍNH NĂNG 2: IN-BROWSER PROFILE PDF FLIPBOOK & LEAD CAPTURE (Trình đọc lật trang HSNL 2026)    │
│ TÍNH NĂNG 3: CASE STUDY DETAIL SLIDE-OVER DRAWER (Hồ sơ nghiệm thu 8 tầng cho 22 dự án)        │
│ TÍNH NĂNG 4: TEAM & KEY PERSONNEL SHOWCASE TAB (12 Nhân sự, 4 Khối ban & Thẩm định Bằng cấp)   │
│ TÍNH NĂNG 5: DIRECT DEMO BOOKING WIDGET VỚI HOSPITAL TIERING & CAM KẾT SLA 24H                  │
└─────────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

### TÍNH NĂNG 1: INTERACTIVE LIVE HOSPITAL FLOW MOCKUP

#### 1. Thông Tin Chung & User Story
* **Tên component**: `HospitalFlowSimulator` (Tích hợp tại Hero Section và trang `/giai-phap/benh-an-dien-tu-emr`).
* **User Story**: 
  > *"Với tư cách là Giám đốc Bệnh viện hoặc Trưởng phòng CNTT, tôi muốn tương tác trực tiếp với một quy trình khám bệnh khép kín 5 bước mô phỏng thực tế ngay trên trình duyệt web, để tôi có thể kiểm chứng được tính liên thông dữ liệu, độ trễ xử lý từng mili-giây, khả năng ký số Cloud CA và phương án phòng ngừa rủi ro xuất toán BHYT mà không cần phải cài đặt phần mềm thử nghiệm phức tạp."*
* **Giá trị Showcase B2G**: Xóa tan hoàn toàn định kiến "website chỉ toàn hình ảnh Photoshop lượm lặt". Chứng minh đẳng cấp làm chủ kiến trúc y tế lâm sàng thời gian thực của TEKNOVA.

#### 2. Luồng Tương Tác UX/UI Chi Tiết Qua 5 Bước Lâm Sàng

```text
[BƯỚC 1: TIẾP ĐÓN KIOSK] ──> [BƯỚC 2: KHÁM BỆNH EMR] ──> [BƯỚC 3: KÊ ĐƠN TT 26]
  • Quét CCCD Chip / VNeID     • Chẩn đoán ICD-10 J44.1     • Kê thuốc Salbutamol / Corticoid
  • Phân luồng Phòng 204        • Dấu sinh tồn: SpO2 96%     • Async Queue liên thông BYT (780ms)
  • Latency: 12ms               • Ký số Cloud CA (34ms)      • Mã QR Đơn thuốc (< 0.8s)
                                                                     │
                                                                     ▼
[BƯỚC 5: ZALO OA & VIETQR] <── [BƯỚC 4: GIÁM ĐỊNH BHYT XML QĐ 130 / QĐ 3176]
  • Decoupled Link bảo mật      • Pre-Audit Rule Engine (Tiền giám định 4 quy tắc)
  • Xác thực OTP + 4 số CCCD    • Tự động đóng gói 5 bảng XML (XML1 - XML5)
  • Thanh toán QR gạch nợ tức thì • Tem thời gian TSA Ban Cơ yếu Chính phủ (HTTP 200 SUCCESS)
```

1. **Bước 1: Tiếp đón tự động & Phân luồng Kiosk (Patient Intake)**:
   * *Hành động*: Người dùng nhấp nút "Mô phỏng quét thẻ CCCD gắn chip" hoặc "Quẹt thẻ BHYT".
   * *Phản hồi UI*: Hiển thị thông tin người bệnh: Ông Nguyễn Văn An (58 tuổi, CCCD: `048068******`), thẻ BHYT `GD47901289*****` còn giá trị sử dụng. Hệ thống tự động phân luồng vào Phòng 204 - Chuyên khoa Hô hấp. Số thứ tự: `#42`. Thời gian phản hồi tiếp nhận: `12ms`.
2. **Bước 2: Khám bệnh lâm sàng & Bệnh án điện tử EMR (Consultation & EMR)**:
   * *Hành động*: Bác sĩ chọn mã bệnh và xác nhận chỉ số sinh tồn.
   * *Phản hồi UI*: Nhập mã chẩn đoán ICD-10: `J44.1` (Đợt cấp bệnh phổi tắc nghẽn mạn tính - COPD), bệnh kèm `I10` (Tăng huyết áp). Nhịp thở `22 l/p`, SpO2 `96%`, Huyết áp `125/80 mmHg`. Kích hoạt nút "Ký số Cloud CA y lệnh" -> Hiển thị chứng thư số RSA-2048 xác thực kèm dấu thời gian TSA Ban Cơ yếu. Độ trễ ký số: `34ms`.
3. **Bước 3: Kê đơn thuốc điện tử liên thông Quốc gia (Prescription TT 26/2025/TT-BYT)**:
   * *Hành động*: Bác sĩ phát hành đơn thuốc điều trị ngoại trú.
   * *Cơ chế kỹ thuật*: Kích hoạt hàng đợi xử lý bất đồng bộ (`Async Queue Worker`) đẩy dữ liệu sang Cổng `donthuocquocgia.vn`.
   * *Mô phỏng độ trễ thực tế*: Hệ thống mô phỏng đúng thời gian trễ xử lý hàng đợi bất đồng bộ `780ms` (TT 26 async queue latency).
   * *Phản hồi UI*: Cấp mã đơn thuốc quốc gia: `26001-DTQG-2026-99214`, in mã QR phản hồi trên màn hình trong thời gian `0.78s` (< 0.8 giây theo yêu cầu). Độ trễ API: `22ms`.
4. **Bước 4: Cổng đối soát, Pre-Audit Rule Engine & Đóng gói XML Giám định BHYT (QĐ 130 & QĐ 3176)**:
   * *Hành động*: Cán bộ giám định nhấp "Trích xuất & Kiểm tra 5 bảng dữ liệu XML".
   * *Hệ Thống Tiền Giám Định Lâm Sàng (Pre-Audit Rule Engine)*: Để bảo vệ bệnh viện trước nguy cơ xuất toán BHYT, hệ thống tự động chạy 4 quy tắc kiểm tra đối soát lâm sàng trước khi gửi dữ liệu:
     1. *Quy tắc 1 (Đồng bộ Dấu thời gian TSA)*: Kiểm tra nghiêm ngặt chuỗi thời gian y lệnh: Thời gian chỉ định <= Thời gian thực hiện <= Thời gian ký số y bác sĩ <= Dấu thời gian TSA Ban Cơ yếu Chính phủ. Loại bỏ 100% lỗi lệch giờ ký số y lệnh.
     2. *Quy tắc 2 (Đối soát Ánh xạ ICD-10 vs Danh mục Dược thư Quốc gia)*: Kiểm tra chẩn đoán ICD-10 có nằm trong chỉ định thanh toán của thuốc theo Thông tư 20/2022/TT-BYT. Cảnh báo và ngăn chặn ngay nếu kê kháng sinh phổ rộng (Ceftriaxone) hoặc giãn phế quản (Salbutamol) nhưng chỉ chẩn đoán Tăng huyết áp vô căn (I10) mà thiếu mã bệnh lý hô hấp.
     3. *Quy tắc 3 (Phạm vi Chứng chỉ Hành nghề CCHN)*: Kiểm tra tính hợp lệ và phạm vi hoạt động chuyên môn ghi trên Chứng chỉ hành nghề (CCHN) của bác sĩ kê đơn/chỉ định dịch vụ kỹ thuật.
     4. *Quy tắc 4 (Quét Trùng Lặp Chỉ Định Dịch Vụ / Duplicate Claims)*: Phát hiện và cảnh báo các chỉ định xét nghiệm, thuốc hoặc thủ thuật bị kê trùng lặp trong cùng một đợt khám (trong vòng 24 giờ).
   * *Phản hồi UI*: Khi cả 4 quy tắc tiền kiểm tra đạt chuẩn, hệ thống tự động đóng gói 5 file XML: `XML1` (Tổng hợp KCB), `XML2` (Bảng thuốc), `XML3` (Vật tư y tế & Dịch vụ kỹ thuật), `XML4` (Cận lâm sàng & X-quang), `XML5` (Diễn biến lâm sàng). Trạng thái phản hồi: **PRE-AUDIT PASSED: HỢP LỆ — 0% NGUY CƠ XUẤT TOÁN (HTTP 200 SUCCESS)**. Độ trễ xử lý: `45ms`.
5. **Bước 5: Trả kết quả, Nhắc lịch khám & Thanh toán Viện phí qua Zalo OA (Decoupled Link & VietQR)**:
   * *Hành động*: Người bệnh mở thông báo trên ứng dụng Zalo điện thoại.
   * *Bảo mật Nghị định 13/2023/NĐ-CP*: Không truyền dữ liệu bệnh án qua máy chủ Zalo. Gửi `Decoupled Link` dùng một lần, yêu cầu nhập 4 số cuối CCCD để mở kết quả.
   * *Phản hồi UI*: Màn hình giả lập điện thoại nhận thông báo Zalo OA Bệnh viện Phổi Đà Nẵng, hiển thị mã VietQR PRO thanh toán phần đồng chi trả viện phí `142.000 VNĐ`, tự động gạch nợ trên hệ thống kế toán HIS và đồng bộ lịch hẹn tái khám sau 14 ngày.

#### 3. Bảng Thanh Tra Kỹ Thuật (Technical Inspector Panel) & Thử Nghiệm Gây Lỗi (Failure Simulation)
* **Inspector Panel**: Một tab bên cạnh cho phép kỹ sư xem trực tiếp cấu trúc gói tin (Live JSON/XML Payload) của từng bước, hiển thị thời gian phản hồi thực tế và có nút "Sao chép cấu trúc JSON" phục vụ các buổi họp kỹ thuật.
* **Nút mô phỏng rớt mạng (Inject Failure Toggle)**: Khi bật nút *"Mô phỏng đứt kết nối Cổng Đơn thuốc Quốc gia"*, hệ thống chuyển sang chế độ `Async Queue Active`. Màn hình hiển thị: *"Đang lưu trữ tạm thời tại bộ đệm Redis nội bộ bệnh viện; đơn thuốc vẫn được cấp mã dự phòng hợp lệ; tự động tái gửi khi kết nối internet khôi phục"*. Tính năng này chứng minh hệ thống không bao giờ làm gián đoạn khâu cấp phát thuốc của bệnh viện.

#### 4. Kiến Trúc Kỹ Thuật, State Machine & TypeScript Contracts

```typescript
// Định nghĩa kiểu dữ liệu cho 5 bước mô phỏng lâm sàng
export type HospitalStepId = 'intake' | 'emr' | 'prescription' | 'bhyt' | 'zalo';

// Cụ thể hóa schema đơn thuốc điện tử TT 26/2025/TT-BYT
export interface EPrecriptionPayload {
  ma_cskcb: string; // Mã cơ sở khám chữa bệnh: "48001" (BV Phổi Đà Nẵng)
  ma_bac_si: string; // Mã CCHN bác sĩ: "BS04921"
  ma_don_thuoc: string; // Mã định danh quốc gia: "26001-DTQG-2026-99214"
  chan_doan: string; // Mã bệnh ICD-10: "J44.1"
  ngay_ke: string;
  thuoc: Array<{
    ma_thuoc: string; // "40.123"
    ten_thuoc: string; // "Salbutamol 5mg"
    so_luong: number;
    don_gia: number;
    thanh_tien: number;
    lieu_dung: string;
  }>;
}

// Cụ thể hóa schema 5 bảng XML giám định BHYT theo QĐ 130/QĐ-BYT & QĐ 3176/QĐ-BYT
export interface Insurance5XmlBundle {
  // Bảng 1: Tổng hợp chi phí khám chữa bệnh BHYT
  xml1TongHop: {
    tag: '<TONG_HOP>';
    MA_LK: string; // "48001_2026_0001"
    MA_BN: string; // "BN00982"
    MA_THE: string; // "GD4790128912345"
    MA_DKBD: string; // "48001"
    MA_BENH: string; // "J44.1"
    NGAY_VAO: string; // "202610150800"
    NGAY_RA: string; // "202610151130"
    KET_QUA_DTRI: string; // "1"
    TINH_TRANG_RV: string; // "1"
    T_TONGCHI: number; // 450000
    T_BHTT: number; // 360000
    T_BNTT: number; // 90000
  };
  // Bảng 2: Chi tiết thuốc thanh toán BHYT
  xml2ChiTietThuoc: {
    tag: '<CHI_TIET_THUOC>';
    danhSachThuoc: Array<{
      tag: '<THUOC>';
      MA_LK: string;
      MA_THUOC: string; // "40.123"
      TEN_THUOC: string; // "Salbutamol 5mg"
      SO_LUONG: number; // 2
      DON_GIA: number; // 45000
      THANH_TIEN: number; // 90000
    }>;
  };
  // Bảng 3: Chi tiết dịch vụ kỹ thuật & vật tư y tế
  xml3ChiTietDvktVtyt: {
    tag: '<CHI_TIET_DVKT_VTYT>';
    danhSachDvkt: Array<{
      tag: '<DVKT>';
      MA_LK: string;
      MA_DICH_VU: string; // "DV.0192"
      TEN_DICH_VU: string; // "Khám lâm sàng hô hấp"
      SO_LUONG: number;
      DON_GIA: number;
      THANH_TIEN: number;
    }>;
  };
  // Bảng 4: Chi tiết kết quả cận lâm sàng
  xml4ChiTietCls: {
    tag: '<CHI_TIET_CLS>';
    danhSachCls: Array<{
      tag: '<CLS>';
      MA_LK: string;
      MA_DICH_VU: string; // "XQ.001"
      NGAY_KQ: string;
      KET_LUAN: string; // "Hình ảnh phế trường sáng tăng dãn"
    }>;
  };
  // Bảng 5: Diễn biến lâm sàng
  xml5DienBienLamsang: {
    tag: '<DIEN_BIEN_LAMSANG>';
    danhSachDienBien: Array<{
      tag: '<DIEN_BIEN>';
      MA_LK: string;
      NGAY_YL: string;
      DIEN_BIEN: string; // "Bệnh nhân tỉnh, khó thở nhẹ, SpO2 96%"
    }>;
  };
}

export interface WorkflowStepData {
  id: HospitalStepId;
  stepIndex: number;
  title: string;
  subTitle: string;
  legalAnchor: string;
  latencyMs: number;
  status: 'idle' | 'processing' | 'success' | 'fallback_active' | 'syncing';
  metrics: { [key: string]: string };
  payloadPreview: EPrecriptionPayload | Insurance5XmlBundle | Record<string, unknown>;
}

export interface HospitalFlowState {
  currentStep: HospitalStepId;
  isPlaying: boolean;
  playbackSpeed: 1 | 2; // Tốc độ tự động phát: 1x (2.5s) hoặc 2x (1.25s)
  isProcessing: boolean; // Trạng thái chuyển tiếp bất đồng bộ
  currentStepLatencyMs: number; // Mô phỏng độ trễ thực tế 780ms (TT 26)
  networkStatus: 'online' | 'offline' | 'syncing' | 'reconnecting';
  isNetworkDownSimulated: boolean;
  pendingQueueCount: number; // Bộ đếm hàng đợi Redis đệm ngoại tuyến
  queueDrainCount: number; // Bộ đếm giải tỏa đơn thuốc khi phục hồi mạng
  activeTab: 'ui_preview' | 'json_inspector';
}
```

```javascript
// State Machine Transitions & Async Latency Simulation
function flowReducer(state, action) {
  switch (action.type) {
    case 'STEP_START':
      return {
        ...state,
        isProcessing: true,
        currentStepLatencyMs: 0
      };
    case 'STEP_PROGRESS':
      return {
        ...state,
        currentStepLatencyMs: action.payload?.latencyMs || 780
      };
    case 'STEP_SUCCESS':
      return {
        ...state,
        isProcessing: false,
        currentStep: action.payload?.nextStep || state.currentStep
      };
    case 'NEXT_STEP': {
      const steps = ['intake', 'emr', 'prescription', 'bhyt', 'zalo'];
      const nextIdx = (steps.indexOf(state.currentStep) + 1) % steps.length;
      return { ...state, currentStep: steps[nextIdx] };
    }
    case 'SET_STEP':
      return { ...state, currentStep: action.payload };
    case 'TOGGLE_PLAY':
      return { ...state, isPlaying: !state.isPlaying };
    case 'TOGGLE_NETWORK_SIMULATION': {
      const willBeDown = !state.isNetworkDownSimulated;
      return {
        ...state,
        isNetworkDownSimulated: willBeDown,
        networkStatus: willBeDown ? 'offline' : 'syncing',
        pendingQueueCount: willBeDown ? 5 : state.pendingQueueCount
      };
    }
    case 'RECONNECT_DRAIN_TICK':
      return {
        ...state,
        queueDrainCount: state.queueDrainCount + 1,
        pendingQueueCount: Math.max(0, state.pendingQueueCount - 1)
      };
    case 'RECONNECT_COMPLETE':
      return {
        ...state,
        networkStatus: 'online',
        pendingQueueCount: 0,
        queueDrainCount: 0
      };
    case 'SWITCH_TAB':
      return { ...state, activeTab: action.payload };
    default:
      return state;
  }
}

// Luồng điều phối bất đồng bộ với độ trễ hàng đợi thực tế 780ms (TT 26 Gateway Simulation):
async function executeStepAsync(dispatch, nextStep) {
  dispatch({ type: 'STEP_START' });
  // Mô phỏng độ trễ hàng đợi liên thông Cổng Đơn thuốc Quốc gia 780ms
  await new Promise((resolve) => setTimeout(resolve, 780));
  dispatch({ type: 'STEP_PROGRESS', payload: { latencyMs: 780 } });
  dispatch({ type: 'STEP_SUCCESS', payload: { nextStep } });
}
```

---

### TÍNH NĂNG 2: IN-BROWSER PROFILE PDF VIEWER / FLIPBOOK & LEAD CAPTURE

#### 1. Thông Tin Chung & User Story
* **Tên component**: `ProfileFlipbookReader` (Kích hoạt qua Modal khi nhấp nút "Tải Profile PDF" tại Header, Hero và Footer).
* **User Story**: 
  > *"Với tư cách là Cán bộ Ban Giám đốc hoặc Phòng Kế hoạch Bệnh viện, tôi muốn có thể mở và đọc lướt toàn bộ cuốn Hồ Sơ Năng Lực 2026 của TEKNOVA trực tiếp ngay trên trình duyệt máy tính hoặc điện thoại mà không phải tải file nặng 30MB về máy, để tôi có thể thẩm định ngay thông tin pháp lý, danh sách nhân sự và văn bằng chứng chỉ trong lúc họp; đồng thời khi cần bản lưu trữ chính thức có đóng dấu đỏ, tôi có thể điền thông tin nhanh để tải về."*
* **Giá trị Showcase B2G**: Tối ưu hóa phễu tiếp cận tài liệu thầu, loại bỏ 100% rào cản tải file nặng, cung cấp trải nghiệm đọc tài liệu số sang trọng và thu thập đầu mối B2G chất lượng cao.

#### 2. Các Chế Độ Xem & Công Cụ Tương Tác
* **Chế độ Lật trang 3D Realistic Flipbook (Desktop / iPad)**: Tái hiện chân thực cảm giác lật mở cuốn kỷ yếu hồ sơ năng lực bìa cứng khổ ngang A4, góc lật uốn lượn tự nhiên theo con trỏ chuột kèm hiệu ứng bóng đổ trang giấy (`shadow-2xl`).
* **Chế độ Cuộn trang dọc liên tục (Mobile Vertical Scroll)**: Tự động phát hiện màn hình di động (< 768px) để chuyển sang chế độ cuộn trang dọc mượt mà, hỗ trợ thao tác chạm vuốt (touch swipe) và zoom hai ngón tay.
* **Mục lục tương tác nhấp tức thì (Interactive Deep-Link TOC)**:
  * Trang 4: Lĩnh vực hoạt động cốt lõi.
  * Trang 6: Sơ đồ cơ cấu tổ chức 4 phòng ban.
  * Trang 7: Giấy phép ĐKKD 0402300331 & Bản quyền tác giả phần mềm EMR.
  * Trang 10: Danh sách 12 nhân sự chủ chốt.
  * Trang 12: Danh mục 22 Hợp đồng dự án thực tế.
  * Trang 17-18: Bản scan văn bằng chứng chỉ gốc của các kỹ sư, thạc sĩ, tiến sĩ.
* **Thanh công cụ trình diễn (Presentation Toolbar)**:
  * Nút `[ ◀ Trang trước ]` / `[ Trang sau ▶ ]`
  * Ô nhập số trang trực tiếp: `Trang [ 12 ] / 18`
  * Nút `[ 🔍 Thu phóng 100% / 150% ]`
  * Nút `[ ⛶ Toàn màn hình (F11 Presentation) ]` tối ưu khi cắm cáp máy chiếu phòng họp.

#### 3. Cổng Thu Thập Đầu Mối Nhẹ Nhàng (3-Field Lead Capture Gate)
* **Nguyên tắc Anti-Friction**: Cho phép người dùng tự do đọc trực tuyến **100% toàn bộ 18 trang** của cuốn Hồ sơ năng lực mà không bắt buộc đăng nhập.
* **Thời điểm kích hoạt phễu**: Chỉ khi người dùng bấm nút nổi bật màu xanh: **"TẢI BẢN GỐC PDF CÓ DẤU ĐỎ ĐỂ LƯU HỒ SƠ THẦU"**, hệ thống mới mở form popup trang nhã với đúng 3 trường thông tin:
  1. *Họ và tên cán bộ*: (Ví dụ: BS. CKII Lê Văn Dũng)
  2. *Đơn vị y tế / Cơ quan công tác*: (Ví dụ: Trung tâm Y tế Quận Hải Châu)
  3. *Số điện thoại / Zalo*: (Ví dụ: 0914 123 456)
* **Cơ chế xử lý tức thời**: Sau khi bấm gửi, trình duyệt tự động kích hoạt tải file `Teknova_Ho_So_Nang_Luc_2026_Official.pdf` ngay lập tức (không bắt người dùng phải vào email xác thực), đồng thời bắn Webhook thông báo cho bộ phận Pre-sales của TEKNOVA qua Telegram / CRM để kịp thời chăm sóc.

#### 4. Kiến Trúc Kỹ Thuật (Zero-Latency Assets Fallback)
* Để bảo đảm thời gian khởi chạy dưới `0.5 giây`, toàn bộ 18 trang PDF được kết xuất sẵn thành các file ảnh WebP tối ưu hóa cao (`/public/profile-assets/page_01.webp` ... `page_18.webp`, dung lượng mỗi trang chỉ ~85KB). Trình duyệt tải trước 2 trang đầu tiên, tạo cảm giác mở tức thì mà không cần đợi thư viện PDF.js giải mã file nhị phân nặng.

#### 5. Invisible Text Layer & Bộ Công Cụ Tìm Kiếm Văn Bản Cho Thanh Tra Viên (Searchable PDF Flipbook)
* **Vấn đề thực tế**: Khi thanh tra viên Sở Y tế hoặc thành viên Tổ chuyên gia đấu thầu cần kiểm tra nhanh các thông số pháp lý, họ thường bấm `Ctrl+F` để tìm kiếm mã số thuế (`0402300331`), tên Chủ tịch HĐQT (`Trần Bình Sơn`), hoặc căn cứ pháp lý (`Thông tư 46`). Do trang tài liệu được render dưới dạng ảnh WebP, tính năng tìm kiếm văn bản tự nhiên sẽ không hoạt động nếu thiếu lớp dữ liệu chữ (Text Layer).
* **Giải pháp Invisible Text Layer (DOM Text Overlay)**:
  - Tích hợp lớp phủ văn bản vô hình (`<div class="invisible-text-layer select-text opacity-0 absolute inset-0 pointer-events-auto">`) đè khớp tọa độ 1:1 trên từng trang WebP trong Flipbook.
  - Các khối chữ được bóc tách từ stream văn bản PDF gốc qua PDF.js, định vị chính xác theo tọa độ `(left, top, width, height)` của từng từ và dòng chữ.
  - Cho phép người dùng bôi đen sao chép nội dung (Text Selection) và hỗ trợ phím tắt `Ctrl+F` bản địa của trình duyệt.
* **Bộ công cụ tìm kiếm nội bộ (Search in Flipbook Engine)**:
  - Trên thanh công cụ Flipbook tích hợp ô nhập: `[ 🔍 Search in Flipbook... ]`.
  - Khi gõ từ khóa (ví dụ: `Trần Bình Sơn`, `0402300331`, `Bệnh viện Phổi Đà Nẵng`), hệ thống tự động quét chỉ mục (In-memory Keyword Index), làm sáng (highlight) các vị trí xuất hiện và hiển thị nút `[ Prev ]` / `[ Next ]` để người dùng nhảy trang tức thì đến đúng nội dung cần tra cứu.

---

### TÍNH NĂNG 3: CASE STUDY DETAIL DRAWER / MODAL (SLIDE-OVER DEEP DIVE)

#### 1. Thông Tin Chung & User Story
* **Tên component**: `CaseStudyDetailDrawer` (Kích hoạt khi nhấp vào bất kỳ thẻ dự án nào trong 22 hợp đồng tại Trang chủ, trang `/du-an` hoặc trang `/giai-phap`).
* **User Story**: 
  > *"Với tư cách là Cán bộ phụ trách Thẩm định hồ sơ thầu Bệnh viện hoặc Sở Y tế, tôi muốn nhấp vào bất kỳ dự án tiêu biểu nào của TEKNOVA để mở ra toàn bộ hồ sơ nghiệm thu chi tiết, xem được số hợp đồng, các phân hệ đã bàn giao, căn cứ văn bản luật, số liệu đo lường trước/sau và nhận xét của lãnh đạo đơn vị, để tôi có đầy đủ cơ sở pháp lý báo cáo lên Hội đồng mua sắm."*
* **Giá trị Showcase B2G**: Biến mỗi dự án thành một hồ sơ năng lực thu nhỏ sắc bén, minh bạch hóa 100% bằng chứng triển khai thực địa, loại bỏ mọi nghi ngờ về năng lực thực tế của công ty.

#### 2. Cấu Trúc 8 Tầng Thông Tin Chiều Sâu Trong Ngăn Kéo Slide-Over

```text
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│ [✕ ĐÓNG] BỆNH VIỆN PHỔI ĐÀ NẴNG · CHI TIẾT DỰ ÁN TRIỂN KHAI EMR & LIÊN THÔNG BHYT              │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ TẦNG 1: BANNER ĐƠN VỊ & HUY HIỆU ĐÁNH GIÁ                                                       │
│ • Bệnh viện Chuyên khoa Hạng II Tuyến Thành phố · Quy mô 250 giường bệnh                        │
│ • Địa chỉ: Tổ 53 Phước Lý, P. Hòa Minh, Q. Liên Chiểu, TP. Đà Nẵng                              │
│ • Huy hiệu: [✓ ĐÃ NGHIỆM THU BỎ BỆNH ÁN GIẤY THEO THÔNG TƯ 46/2018/TT-BYT]                     │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ TẦNG 2: THÔNG TIN HỢP ĐỒNG & CĂN CỨ PHÊ DUYỆT TRÚNG THẦU (HSNL 2026)                            │
│ • Hợp đồng 01: Thuê phần mềm EMR · HĐ số 08/2024/HĐ-BVP · Quyết định số 142/QĐ-SYT (KQLCNT)   │
│   Mã E-TBMT Hệ thống Mạng Đấu thầu Quốc gia: IB2400018920-00 (muasamcong.mpi.gov.vn)            │
│ • Hợp đồng 02: Nâng cấp HIS XML QĐ 3176 · HĐ số 29/2024/HĐ-XML-BVP · Quyết định số 356/QĐ-BVP │
│ • Hợp đồng 03: Phần mềm Zalo OA tra cứu · HĐ số 12/2024/HĐ-ZALO-BVP · Quyết định số 218/QĐ-BVP│
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ TẦNG 3: BỐI CẢNH & BÀI TOÁN KHÓ TRƯỚC TRIỂN KHAI                                                │
│ • Hàng nghìn hồ sơ bệnh án giấy lưu kho quá tải, nguy cơ ẩm mốc, thất lạc bệnh án điều trị dài  │
│   ngày; bác sĩ mất trung bình 35-40% thời gian trực buồng chỉ để ghi chép tay và ký sổ.         │
│ • Áp lực xuất toán BHYT do sai lệch dấu thời gian ký y lệnh so với giờ thực hiện cận lâm sàng.  │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ TẦNG 4: DANH MỤC PHÂN HỆ PHẦN MỀM ĐÃ BÀN GIAO THỰC TẾ                                           │
│ [✓] Phân hệ Bệnh án điện tử nội trú các khoa lâm sàng (Nội Hô hấp, Hồi sức cấp cứu, Lao)       │
│ [✓] Phân hệ Ký số tập trung Cloud CA & Dấu thời gian TSA Ban Cơ yếu Chính phủ                    │
│ [✓] Cổng trích xuất tự động gói tin XML liên thông Giám định BHYT theo QĐ 3176/QĐ-BYT            │
│ [✓] Cổng đồng bộ dữ liệu Người bệnh tử vong đẩy Cổng Dịch vụ công TP. Đà Nẵng                   │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ TẦNG 5: CĂN CỨ PHÁP LÝ NGHIỆM THU BẮT BUỘC                                                     │
│ • Thông tư 46/2018/TT-BYT: Quy định về hồ sơ bệnh án điện tử, lưu trữ và bảo mật                │
│ • Quyết định 3176/QĐ-BYT: Chuẩn dữ liệu đầu ra phục vụ quản lý, giám định, thanh toán KCB BHYT │
│ • Quyết định 80/2014/QĐ-TTg: Cơ chế thuê dịch vụ CNTT thường niên chi từ nguồn thu viện phí    │
│ • Nghị định 13/2023/NĐ-CP: Bảo vệ dữ liệu cá nhân bệnh nhân qua Decoupled Link Zalo OA         │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ TẦNG 6: BẢNG SO SÁNH CHỈ SỐ ĐO LƯỜNG TÁC ĐỘNG (BEFORE vs. AFTER METRICS)                        │
│ ┌──────────────────────────────────────────────┬──────────────────┬──────────────────┐          │
│ │ Chỉ số Vận hành & Đo lường                   │ Trước Khi Làm    │ Sau Khi Bàn Giao │          │
│ ├──────────────────────────────────────────────┼──────────────────┼──────────────────┤          │
│ │ Tỷ lệ bệnh án nội trú không giấy             │ 0.0% (100% giấy) │ 100% Điện tử     │          │
│ │ Thời gian tra cứu tiền sử bệnh án cũ         │ 15 - 25 phút     │ < 3 giây         │          │
│ │ Tỷ lệ hồ sơ bị trả về kiểm tra dấu giờ BHYT  │ 8.4%             │ 0.0%             │          │
│ │ Thời gian trả kết quả chẩn đoán qua Zalo     │ Chờ tại sảnh     │ Nhận sau 30 giây │          │
│ └──────────────────────────────────────────────┴──────────────────┴──────────────────┘          │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ TẦNG 7: TRÍCH DẪN ĐÁNH GIÁ THỰC TẾ TỪ LÃNH ĐẠO CƠ SỞ                                            │
│ "Kỹ sư TEKNOVA túc trực trực tiếp tại các khoa phòng cả ban đêm, hướng dẫn từng bác sĩ lớn tuổi │
│ thao tác ký số y lệnh. Nhờ hệ thống dấu thời gian TSA chuẩn mực, đợt kiểm tra BHYT vừa qua     │
│ bệnh viện không bị xuất toán một hồ sơ nào, thủ tục thanh quyết toán diễn ra rất thuận lợi."    │
│ — Trích Biên bản Đánh giá Kỹ thuật, Hội đồng Khoa học Bệnh viện Phổi Đà Nẵng                    │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ TẦNG 8: HÀNH ĐỘNG CHUYỂN ĐỔI TIẾP THEO (BOTTOM CONVERSION ACTION)                               │
│ [ ĐĂNG KÝ THAM QUAN THỰC TẾ MÔ HÌNH NÀY TẠI BỆNH VIỆN PHỔI ĐÀ NẴNG ] -> Tự động điền thông tin  │
└─────────────────────────────────────────────────────────────────────────────────────────────────┘
```

#### 3. Danh Mục 22 Dự Án Có Sẵn Trong Hệ Thống Drawer
Hệ thống mã nguồn phải nạp đầy đủ cấu trúc dữ liệu cho **tất cả 22 hợp đồng** từ HSNL 2026 kèm định danh hợp đồng thực tế (`contractNumber` / `biddingRef` / Số Quyết định phê duyệt trúng thầu):
1. `bv-phoi-emr`: Thuê phần mềm EMR Bệnh viện Phổi Đà Nẵng (HĐ số 08/2024/HĐ-BVP · Quyết định số 142/QĐ-SYT · E-TBMT: IB2400018920-00)
2. `bv-phoi-zalo`: Phần mềm quảng bá và tra cứu Zalo OA tích hợp HIS Bệnh viện Phổi (HĐ số 12/2024/HĐ-ZALO-BVP · Quyết định số 218/QĐ-BVP)
3. `bv-phoi-xml3176`: Nâng cấp HIS XML QĐ 3176 và dữ liệu tử vong DVC TP. Đà Nẵng (HĐ số 29/2024/HĐ-XML-BVP · Quyết định số 356/QĐ-BVP)
4. `ttyt-lienchieu-tt26`: Cập nhật đơn thuốc điện tử TT 26/2025/TT-BYT tại TTYT Liên Chiểu (HĐ số 05/2025/HĐ-TT26-LC · Quyết định số 89/QĐ-TTYTLC)
5. `ttyt-lienchieu-xml3176`: Nâng cấp trích xuất XML QĐ 3176 tại TTYT Liên Chiểu (HĐ số 19/2024/HĐ-XML-LC · Quyết định số 194/QĐ-TTYTLC)
6. `ttyt-lienchieu-qd130`: Nâng cấp phần mềm BV đáp ứng QĐ 130, CV 1165, CV 3617, Đề án 06, GPLX và Zalo OA (HĐ số 33/2024/HĐ-QD130-LC · Quyết định số 312/QĐ-TTYTLC)
7. `ttyt-camle-xml3176`: Cập nhật HIS đẩy XML QĐ 3176 tại TTYT Cẩm Lệ (HĐ số 21/2024/HĐ-HIS-CL · Quyết định số 208/QĐ-TTYTCL)
8. `ttyt-nguhanhson-emr`: Thuê phần mềm Bệnh án điện tử EMR 2025 tại TTYT Ngũ Hành Sơn (HĐ số 02/2025/HĐ-EMR-NHS · Quyết định số 45/QĐ-TTYTNHS)
9. `bv-phusannhi-zalo`: Phần mềm trả kết quả xét nghiệm qua Zalo cơ sở 01 BV Phụ sản - Nhi (HĐ số 16/2024/HĐ-PSN · Quyết định số 175/QĐ-BVPSN)
10. `bv-yhoccotruyen`: Cổng thông tin điện tử Bệnh viện Y học Cổ truyền TP. Đà Nẵng (HĐ số 01/2024/HĐ-YDCT · Quyết định số 56/QĐ-BVYDCT)
11. `chicuc-danso-web`: Web tổng hợp thống kê dữ liệu báo cáo cơ sở Chi cục Dân số Đà Nẵng (HĐ số 07/2024/HĐ-CCDS · Quyết định số 92/QĐ-CCDS)
12. `chicuc-danso-portal`: Cổng thông tin điện tử Chi cục Dân số TP. Đà Nẵng (HĐ số 11/2024/HĐ-WEB-CCDS · Quyết định số 128/QĐ-CCDS)
13. `ubnd-nguhanhson-zalo`: Hệ thống gửi thông báo, tin nhắn Zalo OA UBND P. Ngũ Hành Sơn (HĐ số 14/2024/HĐ-UBND-NHS · Quyết định số 164/QĐ-UBND)
14. `xa-xuanphu-cds`: Đề án Chuyển đổi số 2026-2030 tầm nhìn 2035 Xã Xuân Phú (HĐ số 03/2025/HĐ-XP · Quyết định số 28/QĐ-UBNDXP)
15. `xa-xuanphu-csdl`: Cập nhật, tạo lập dữ liệu cơ sở vào Kho dữ liệu dùng chung TP. Đà Nẵng (HĐ số 09/2025/HĐ-DL-XP · Quyết định số 64/QĐ-UBNDXP)
16. `xa-tienphuoc-csdl`: Chuẩn hóa dữ liệu phần mềm, CSDL chuyên ngành Xã Tiên Phước (HĐ số 15/2024/HĐ-TP · Quyết định số 182/QĐ-UBNDTP)
17. `tt-cds-danang`: Phần mềm đánh giá tiêu chí CNTT tại Trung tâm CĐS & CN Chiến lược Đà Nẵng (HĐ số 22/2024/HĐ-CDS-STTTT · Quyết định số 240/QĐ-STTTT)
18. `dienbanbac-ai`: Tổ dân phố thông minh: Camera AI và lưu trữ dữ liệu Phường Điện Bàn Bắc (HĐ số 26/2024/HĐ-DBB · Quyết định số 298/QĐ-UBNDDBB)
19. `cloud-ace-portal`: Cổng thông tin khách hàng Web & Mobile App cho Cloud ACE (Google Cloud Partner · HĐ thương mại số 01/2024/TEK-CA)
20. `pvcombank-his`: Nâng cấp phần mềm quản lý BV và kênh giao tiếp Zalo OA (PVcomBank · HĐ hợp tác công nghệ số 04/2024/TEK-PVCOM)
21. `mobifone-zalo-tthc`: Phần mềm giải đáp TTHC trên Zalo OA và Zalo Mini App (MobiFone Đà Nẵng · HĐ dịch vụ số 18/2024/TEK-MBF)
22. `mobifone-zalo-phuongxa`: Phần mềm chuyển đổi số phường xã qua Zalo OA (MobiFone Đà Nẵng · HĐ kinh tế số 25/2024/TEK-MBF2)

#### 4. Kỹ Thuật Deep-Link URL & Animation Specs
* **Đồng bộ Deep-Link**: Khi drawer mở ra, tự động cập nhật URL thành `?project=bv-phoi-emr` qua `window.history.pushState`. Cho phép chuyên viên kinh doanh sao chép link gửi trực tiếp cho khách hàng mở đúng ca triển khai.
* **Animation Specs**: 
  * Ngăn kéo trượt từ mép phải: `transform: translateX(100%) -> translateX(0)`, thời lượng `300ms`, easing `cubic-bezier(0.16, 1, 0.3, 1)`.
  * Lớp nền Backdrop làm mờ: `backdrop-blur-sm bg-slate-900/40`, hiệu ứng fade-in trong `200ms`.
  * Phím tắt: Bấm `Escape` hoặc nhấp vùng ngoài để đóng ngăn kéo.

---

### TÍNH NĂNG 4: TEAM & KEY PERSONNEL SHOWCASE TAB

#### 1. Thông Tin Chung & User Story
* **Tên component**: `TeamPersonnelRoster` (Tích hợp tại Section `#experts` trên Trang chủ và trang `/gioi-thieu`).
* **User Story**: 
  > *"Với tư cách là Thành viên Hội đồng Xét duyệt Hồ sơ thầu, tôi muốn xem xét danh sách nhân sự của TEKNOVA, phân định rõ ràng học vị, số năm kinh nghiệm, vai trò trong dự án và có thể mở xem bản tóm tắt văn bằng chứng chỉ đã được chứng thực trong Hồ sơ năng lực, để tôi bảo đảm rằng đội ngũ cam kết thực thi gói thầu hoàn toàn đủ năng lực chuyên môn theo quy định của Luật Đấu thầu."*
* **Giá trị Showcase B2G**: Phục hồi uy tín nhân sự tối cao, minh bạch hóa 100% bằng cấp của 12 chuyên gia, dập tắt nghi ngờ về việc "thuê bằng khống" hoặc "nhân sự ảo".

##### 2. Cấu Trúc Bộ Lọc Phân Tầng 4 Khối Phòng Ban (Division Filter Tabs)

```text
[ TẤT CẢ (12) ]  [ BAN LÃNH ĐẠO & CỐ VẤN (2) ]  [ KỸ THUẬT & R&D PHẦN MỀM (3) ]  [ TRIỂN KHAI & HẠ TẦNG (4) ]  [ VẬN HÀNH & KINH DOANH (3) ]
```

* **Khối 1: Ban Lãnh Đạo & Cố Vấn Cấp Cao (Executive Leadership)**:
  1. **Trần Bình Sơn** — Chủ tịch HĐQT & Tổng Giám đốc (MBA, Kỹ sư Điện tử, >20 năm KN).
  2. **TS. Lê Trọng Nhân** — Giám đốc Công nghệ & Cố vấn Cấp cao (Tiến sĩ Xử lý tín hiệu & Viễn thông, >15 năm KN).
* **Khối 2: Nghiên Cứu & Phát Triển Phần Mềm Lõi (R&D & Core Engineering)**:
  3. **KS. Võ Quang Hòa** — Trưởng phòng Kiến trúc Phần mềm & ATTT (Kỹ sư CNTT, 13 năm KN).
  4. **ThS. Lê Hoàng Hải** — Trưởng nhóm Khoa học Dữ liệu & AI (Thạc sĩ KHMT, >10 năm KN).
  5. **CN. Dương Mạnh Quân** — Lập trình viên Web Portal & CSDL Phân tán (Cử nhân CNTT, 01 năm KN).
* **Khối 3: Triển Khai Thực Địa & Hạ Tầng Mạng (Field Operations & Infrastructure)**:
  6. **KS. Nguyễn Hoài Nhân** — Trưởng bộ phận Tích hợp Hệ thống & HIS (Kỹ sư CNTT, 12 năm KN).
  7. **KS. Trần Ngọc Trai** — Kỹ sư Trưởng Hạ tầng Điện nhẹ (ELV) & Data Center (Kỹ sư Điện, >20 năm KN). *Nhân sự kỳ cựu được khôi phục*.
  8. **KS. Trần Minh Chiến** — Kỹ sư Triển khai Hệ thống & Zalo OA (Kỹ sư CNTT, 02 năm KN).
  9. **KS. Lê Thiện Nhân** — Kỹ sư Phần cứng Y tế & Kiosk Tiếp đón (Kỹ sư Kỹ thuật Máy tính, 01 năm KN).
* **Khối 4: Vận Hành Tổng Hợp, Tài Chính & Kinh Doanh (Administration & Business)**:
  10. **CN. Nguyễn Thị Dung** — Kế toán trưởng & Phụ trách Quyết toán Thầu (Cử nhân Kinh tế, >5 năm KN).
  11. **CN. Nguyễn Thị Thúy Vân** — Trưởng bộ phận Hành chính - Nhân sự (Cử nhân Quản trị, >10 năm KN).
  12. **CN. Bùi Thị Mai** — Chuyên viên Kinh doanh Dự án B2G & Chăm sóc Khách hàng (Cử nhân QTKD, 02 năm KN). *Nhân sự mới được bổ sung*.

#### 3. Modal Xem Văn Bằng Chứng Thực Scan Từ HSNL (Credential Verification Modal)
* Đối với 9 nhân sự có chứng chỉ công chứng đính kèm trong HSNL 2026 (Trần Bình Sơn, Lê Trọng Nhân, Võ Quang Hòa, Nguyễn Hoài Nhân, Lê Hoàng Hải, Trần Minh Chiến, Lê Thiện Nhân, Dương Mạnh Quân, Trần Ngọc Trai):
* Trên thẻ nhân sự có nút bấm: **"Xem Bằng Cấp & Chứng Chỉ Thẩm Định"**.
* Khi nhấp vào, mở Modal hiển thị trích lục thông tin văn bằng: Tên trường đại học cấp bằng (Đại học Bách Khoa, Đại học Kinh Tế...), số hiệu bằng, chuyên ngành đào tạo và dấu giáp lai đã đối soát trong Hồ Sơ Năng Lực 2026.

---

### TÍNH NĂNG 5: DIRECT DEMO BOOKING FORM VỚI DYNAMIC TIERING & CAM KẾT SLA 24H

#### 1. Thông Tin Chung & User Story
* **Tên component**: `EnterpriseDemoBookingWidget` (Kích hoạt qua Modal khi nhấp nút "Tư Vấn Dự Án" / "Đặt Lịch Khảo Sát Hiện Trường", hoặc nhúng cố định tại trang `/lien-he`).
* **User Story**: 
  > *"Với tư cách là Lãnh đạo Bệnh viện hoặc Đơn vị Hành chính, tôi muốn điền một form yêu cầu tư vấn có phân định rõ hạng bệnh viện của tôi, chức danh công tác và các bài toán y tế chuyên sâu cần giải quyết, đồng thời nhận được cam kết bằng văn bản về thời gian phản hồi của Kỹ sư trưởng trong vòng 24 giờ, để tôi có thể chủ động sắp xếp lịch họp chuyên môn của đơn vị."*
* **Giá trị Showcase B2G**: Chuyển đổi từ form bán lẻ sơ sài sang quy trình tiếp nhận dịch vụ B2G đẳng cấp cao, xác lập niềm tin vững chắc về tính chuyên nghiệp và tốc độ hỗ trợ hiện trường.

#### 2. Cấu Trúc Form 4 Bước Thông Minh Chuẩn B2G

```text
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│ ĐĂNG KÝ KHẢO SÁT HIỆN TRƯỜNG & DEMO PHẦN MỀM LÂM SÀNG                                [✕ ĐÓNG]   │
│ TEKNOVA cam kết cử chuyên gia kỹ thuật hỗ trợ trực tiếp tại cơ sở của Quý đơn vị                │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ BƯỚC 1: PHÂN HẠNG CƠ SỞ Y TẾ & TÊN ĐƠN VỊ CÔNG TÁC (*)                                          │
│   (◉) Bệnh viện Chuyên khoa / Hạng I Tuyến Tỉnh, Thành Phố                                      │
│   ( ) Bệnh viện Đa khoa / Hạng II Tuyến Quận, Huyện                                             │
│   ( ) Trung tâm Y tế Khu vực / Bệnh viện Đa khoa Khu vực                                        │
│   ( ) Trạm Y tế Xã, Phường / Phòng khám Đa khoa Tư nhân                                         │
│   ( ) Cơ quan Quản lý Nhà nước (Sở Y tế, UBND Phường/Xã, Chi cục Dân số)                        │
│                                                                                                 │
│   Tên đơn vị: [ Bệnh viện Phổi Đà Nẵng                                        ]                 │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ BƯỚC 2: THÔNG TIN CÁN BỘ ĐẠI DIỆN                                                               │
│   Chức danh / Vai trò công tác (*):                                                             │
│   [ Giám đốc / Phó Giám đốc Bệnh viện                                     ▼ ]                   │
│   (Menu chọn: Trưởng phòng Kế hoạch Tổng hợp, Trưởng phòng CNTT, Trưởng khoa Dược, Bác sĩ trưởng)│
│                                                                                                 │
│   Họ và tên cán bộ: [ BS. CKII Nguyễn Văn An           ]                                        │
│   Số điện thoại di động / Zalo (*): [ 0935 722 579     ] (Kiểm tra đúng định dạng di động VN)   │
│   Email công vụ / Đơn vị (*): [ nguyenvanan@bvphoidanang.gov.vn           ]                      │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ BƯỚC 3: NHU CẦU GIẢI PHÁP TRỌNG TÂM & HÌNH THỨC LÀM VIỆC                                        │
│   Các phân hệ mong muốn khảo sát:                                                               │
│   [☑] Bệnh án điện tử EMR bỏ hoàn toàn bệnh án giấy (Thông tư 46/2018/TT-BYT)                   │
│   [☑] Cập nhật mẫu Đơn thuốc điện tử liên thông Quốc gia (Thông tư 26/2025/TT-BYT)              │
│   [ ] Nâng cấp trích xuất 5 bảng XML & Giám định BHYT (Quyết định 130 & QĐ 3176)                │
│   [ ] Tư vấn gói thuê dịch vụ CNTT OPEX chi từ nguồn thu viện phí (Quyết định 80/2014)          │
│   [ ] Kênh tiếp đón, trả kết quả và thanh toán viện phí qua Zalo OA                             │
│                                                                                                 │
│   Hình thức làm việc mong muốn:                                                                 │
│   (•) Kỹ sư TEKNOVA mang thiết bị demo trực tiếp tại Bệnh viện (On-site)                        │
│   ( ) Họp trình diễn giải pháp trực tuyến qua Zoom / Google Meet (Online)                       │
│   ( ) Đăng ký tham quan thực tế mô hình đã nghiệm thu tại BV Phổi / TTYT Liên Chiểu             │
│                                                                                                 │
│   Thời gian dự kiến: [ 22/10/2026 📅 ]   Khung giờ: [ 08:30 - 10:00 Sáng ▼ ]                     │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ BƯỚC 4: BẢO CHỨNG CAM KẾT SLA DỊCH VỤ TỪ TEKNOVA (SERVICE LEVEL AGREEMENT)                      │
│   ┌───────────────────────────────────────────────────────────────────────────────────────┐     │
│   │ 🛡️ CAM KẾT TRÁCH NHIỆM PHỤC VỤ CHUẨN DOANH NGHIỆP CÔNG NGHỆ:                           │     │
│   │ • Kỹ sư Trưởng Giải pháp sẽ liên hệ xác nhận lịch trong vòng 24 GIỜ LÀM VIỆC.         │     │
│   │ • Gửi hồ sơ khảo sát tiền khả thi & tài liệu kỹ thuật trong vòng 48 GIỜ.              │     │
│   │ • Tuyệt đối không làm gián đoạn công tác khám chữa bệnh chuyên môn của y bác sĩ.      │     │
│   └───────────────────────────────────────────────────────────────────────────────────────┘     │
│                                                                                                 │
│ [ XÁC NHẬN ĐẶT LỊCH KHẢO SÁT & NHẬN MÃ THEO DÕI ]                                               │
└─────────────────────────────────────────────────────────────────────────────────────────────────┘
```

#### 3. Màn Hình Tiếp Nhận Thành Công Với Mã Ticket ID & Đồng Bộ Lịch
* Khi gửi form thành công:
  * Sinh mã tiếp nhận hồ sơ: **`TEK-B2G-2026-8842`**.
  * Phân công chuyên gia đầu mối: **KS. Nguyễn Hoài Nhân (Trưởng bộ phận Tích hợp Hệ thống, ĐT: 0935 722 579)**.
  * Tích hợp nút: **`[ + Thêm vào Google Calendar / Tải file .ICS ]`** để cán bộ tự động lưu lịch hẹn vào ứng dụng lịch cơ quan.
  * Hotline tiếp nhận trực ban 24/7: `0935 722 579`.

#### 4. Đặc Tả Thuật Toán Kiểm Tra Số Điện Thoại Di Động Việt Nam Chuẩn Hóa (Vietnamese Mobile Regex & Sanitization Engine)
* **Quy trình xử lý 2 bước (Two-Phase Sanitization & Validation Pipeline)**:
  Để ngăn ngừa lỗi form không hợp lệ đối với người dùng nhập có khoảng trắng (như mẫu `0935 722 579`) hoặc ký tự phân cách, mã nguồn TypeScript bắt buộc phải làm sạch ký tự trước khi kiểm tra qua chuỗi Regex chuẩn hóa:

```typescript
// Bước 1: Làm sạch khoảng trắng và ký tự phân cách
const cleanPhone = rawPhone.replace(/[\s.-]/g, '');

// Bước 2: Regex chuẩn hóa 6 nhà mạng di động Việt Nam (Viettel, Vina, Mobi, Vietnamobile, Gmobile, Itelecom/Wintel)
const VN_MOBILE_REGEX = /^(0|\+84)(3[2-9]|5[2689]|7[06-9]|8[1-9]|9[0-9])[0-9]{7}$/;

// Hàm kiểm thử hợp lệ:
export function validateVietnameseMobilePhone(rawPhone: string): boolean {
  if (!rawPhone) return false;
  const cleanPhone = rawPhone.replace(/[\s.-]/g, '');
  return VN_MOBILE_REGEX.test(cleanPhone);
}
```

* **Kiểm định thực tế**:
  - Khi người dùng nhập `0935 722 579`, bước `cleanPhone` trả về `0935722579`, khớp hoàn toàn với `VN_MOBILE_REGEX` (nhà mạng MobiFone đầu số `093`).
  - Hỗ trợ đầy đủ tiền tố quốc tế `+84` (ví dụ `+84935722579`).
  - Loại bỏ hoàn toàn số điện thoại bàn (mã vùng Đà Nẵng `0236...`), các đầu số 11 số cũ đã ngưng hoạt động (`012...`), và các payload tấn công XSS/SQL Injection.

---

## 7. LỘ TRÌNH TRIỂN KHAI & PHÂN CHIA SPRINT (SPRINT ROADMAP)

Kế hoạch hành động kỹ thuật được phân bổ thành 3 Sprint liên hoàn trong 10 ngày làm việc:

```text
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                LỘ TRÌNH 3 SPRINT TRIỂN KHAI DEV ACTION                          │
├───────────────────────────────┬─────────────────────────────────┬───────────────────────────────┤
│ SPRINT 1: NGÀY 1 - 3          │ SPRINT 2: NGÀY 4 - 7            │ SPRINT 3: NGÀY 8 - 10         │
│ • Hotfix P0/P1 Chí Mạng       │ • 5 Tính Năng Showcase B2G      │ • E2E Testing & Performance   │
│ • Chuẩn hóa 100% Dữ Liệu Thật │ • Live Hospital Flow Mockup     │ • Cross-browser & Mobile QA   │
│ • Phục hồi Khối Lãnh Đạo      │ • In-browser Flipbook Reader    │ • Core Web Vitals < 1.5s      │
│ • Thay thế Ảnh Thumbnail Local│ • Case Study Slide-over Drawer  │ • Đóng Gói Production Release │
│ • Sửa lỗi Counter 00+         │ • Team Tab & Smart Booking SLA  │                               │
└───────────────────────────────┴─────────────────────────────────┴───────────────────────────────┘
```

### Sprint 1 (Ngày 1 - 3): Xử Lý Hotfix P0/P1 & Chuẩn Hóa Dữ Liệu Gốc
* **Mục tiêu**: Xóa sổ hoàn toàn các lỗi chí mạng, đưa dữ liệu web về đúng Chân lý Đơn nhất (SSOT) từ HSNL 2026.
* **Các công việc cụ thể**:
  1. *Ngày 1*: 
     - Sửa tệp `teknova-data.ts`: Đổi tên Chủ tịch HĐQT thành **Trần Bình Sơn (MBA, Kỹ sư Điện tử)**, cập nhật đầy đủ 12 nhân sự và 22 hợp đồng thực tế.
     - Xóa sạch logo đối tác chưa ký kết chính thức (Vinmec, Cisco, Microsoft, BIDV...), cập nhật 12 logo đơn vị thật.
  2. *Ngày 2*:
     - Tải và lưu trữ 6 ảnh thumbnail dự án vào thư mục cục bộ `public/assets/img/projects/`; sửa triệt để lỗi thẻ trắng toát tại Block 6 trên Netlify.
     - Tái lập toàn diện khối Lãnh đạo tại Block 7 trên `HomeView.vue`, chèn ảnh cutout `/ceo-cutout.png` và 3 luận điểm cam kết hành động.
  3. *Ngày 3*:
     - Sửa lỗi hydration counter hiển thị `00+` trên dải số liệu Block 3.
     - Tái cấu trúc Hero Section sang dạng Monumental Centered 1200px.
     - Cập nhật địa chỉ trụ sở chính tại 456 Nguyễn Hữu Thọ và MST `0402300331` ở Footer.

### Sprint 2 (Ngày 4 - 7): Xây Dựng 5 Tính Năng Nâng Tầm Trình Diễn B2G
* **Mục tiêu**: Lắp ráp và hoàn thiện 5 cỗ máy tương tác phục vụ trình chiếu thầu.
* **Các công việc cụ thể**:
  1. *Ngày 4*: Xây dựng component `HospitalFlowSimulator` (Tính năng 1): 5 bước khám lâm sàng, thanh tiến trình, tab Inspector JSON Payload và nút mô phỏng rớt mạng tự phục hồi.
  2. *Ngày 5*: Xây dựng component `CaseStudyDetailDrawer` (Tính năng 3): Slide-over 8 tầng thông tin, kết nối dữ liệu 22 hợp đồng thực tế và cơ chế deep-link URL `?project=...`.
  3. *Ngày 6*: Xây dựng component `ProfileFlipbookReader` (Tính năng 2): Nạp trước 18 trang WebP, hiệu ứng lật trang 3D mượt mà, mục lục tương tác và form Lead Capture 3 trường khi tải bản PDF dấu đỏ.
  4. *Ngày 7*: Hoàn thiện `TeamPersonnelRoster` (Tính năng 4) với 4 bộ lọc phòng ban kèm modal xem văn bằng; xây dựng `EnterpriseDemoBookingWidget` (Tính năng 5) với phân hạng cơ sở y tế, regex SĐT Việt Nam và cam kết SLA 24h.

### Sprint 3 (Ngày 8 - 10): Kiểm Thử Toàn Diện, Tối Ưu Hóa & Đóng Gói Bàn Giao
* **Mục tiêu**: Bảo đảm tính tương thích hoàn hảo trên mọi thiết bị và đạt chuẩn hiệu năng cao nhất.
* **Các công việc cụ thể**:
  1. *Ngày 8*: Kiểm thử tương thích Responsive từ màn hình Mobile nhỏ (iPhone SE 375px) đến Desktop 4K (3840px); kiểm tra độ tương phản màu sắc đạt chuẩn WCAG AA/AAA.
  2. *Ngày 9*: Kiểm thử E2E liên thông tất cả các luồng: Đặt lịch demo, tải file PDF, chuyển bước mô phỏng lâm sàng, sao chép JSON payload.
  3. *Ngày 10*: Tối ưu hóa Core Web Vitals: LCP < 1.2s, CLS = 0, FID < 50ms, Speed Index < 1.5s; xuất bản mã nguồn bản Production Release và bàn giao cho Ban Lãnh Đạo TEKNOVA.

---

## 8. TIÊU CHÍ NGHIỆM THU KỸ THUẬT & MA TRẬN KIỂM THỬ (ACCEPTANCE CRITERIA & QA MATRIX)

### 8.1 Bộ Checklist 25 Tiêu Chí Nghiệm Thu Khắt Khe (Pass / Fail Criteria)

Đợt bàn giao chỉ được coi là hoàn tất khi toàn bộ **25 tiêu chí** dưới đây đạt trạng thái **PASS 100%**:

```text
┌─────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                 CHECKLIST 25 TIÊU CHÍ NGHIỆM THU                                │
├─────────────────────────────────────────────────────────────────────────────────────────────────┤
│ [1. ĐỐI SOÁT DỮ LIỆU & PHÁP LÝ CHÍNH DANH]                                                      │
│ [ ] AC-01: Tên Chủ tịch HĐQT kiêm TGĐ hiển thị chính xác 100% là Trần Bình Sơn (MBA, KS Điện tử)│
│ [ ] AC-02: Hoàn toàn không còn bất kỳ chữ "Nguyễn Hùng Sơn" nào trong giao diện và mã nguồn.     │
│ [ ] AC-03: Hiển thị đầy đủ 12 nhân sự nòng cốt theo đúng HSNL 2026 (có KS. Trai & Bùi Thị Mai). │
│ [ ] AC-04: Hiển thị đầy đủ 22 hợp đồng thực tế, phân chia chuẩn 3 nhóm khách hàng chiến lược.   │
│ [ ] AC-05: Xóa bỏ 100% đối tác chưa ký kết chính thức (Vinmec, Cisco, Microsoft, Fortinet, BIDV, Vietcombank...).│
│ [ ] AC-06: Xóa bỏ case study giả định "Dược Phẩm Miền Trung" và quote bác sĩ ảo (BS. A, DS. B). │
│ [ ] AC-07: Footer hiển thị đầy đủ Trụ sở chính: Tầng 3, 456 Nguyễn Hữu Thọ, Cẩm Lệ, Đà Nẵng.   │
│ [ ] AC-08: Footer hiển thị đầy đủ Mã số doanh nghiệp: 0402300331 cấp ngày 23/09/2025.            │
│                                                                                                 │
│ [2. KHẮC PHỤC LỖI THỊ GIÁC & LAYOUT]                                                            │
│ [ ] AC-09: 100% ảnh thumbnail dự án tại Block 6 hiển thị sắc nét, zero lỗi ảnh vỡ/trắng toát.   │
│ [ ] AC-10: Toàn bộ ảnh được lưu trữ cục bộ trong /public/assets/, không phụ thuộc URL CDN ngoài.│
│ [ ] AC-11: Khối Lãnh đạo tại Block 7 hiện diện đầy đủ với chân dung cắt nền /ceo-cutout.png.    │
│ [ ] AC-12: Khối số liệu thành tựu hiển thị số chuẩn (>20 Năm, 22+ Dự án), zero lỗi counter 00+. │
│ [ ] AC-13: Hero Section được bố trí theo Monumental Centered Layout với mockup EMR rộng 1200px. │
│ [ ] AC-14: Block Lĩnh vực hoạt động là 1 Bento Grid 6 ô duy nhất, Card 4 phủ màu xanh Cobalt.   │
│ [ ] AC-15: Banner CTA cuối trang sử dụng gradient xanh công nghệ, thay thế màu xanh đen cũ.     │
│                                                                                                 │
│ [3. NĂNG LỰC TƯƠNG TÁC & 5 TÍNH NĂNG SHOWCASE]                                                  │
│ [ ] AC-16: Hospital Flow Simulator chuyển đổi mượt mà qua cả 5 bước lâm sàng trong < 50ms.      │
│ [ ] AC-17: Nút thử nghiệm rớt mạng Cổng BYT kích hoạt đúng chế độ hàng đợi Async Queue Redis.   │
│ [ ] AC-18: Nút "Sao chép JSON" tại Inspector Panel sao chép đúng định dạng JSON vào Clipboard.  │
│ [ ] AC-19: Profile Flipbook mở trong < 0.5s, lật trang 3D mượt mà, mục lục nhảy trang chính xác.│
│ [ ] AC-20: Cổng Lead Capture 3 trường xuất hiện khi tải PDF có dấu đỏ và tải file thành công.   │
│ [ ] AC-21: Case Study Detail Drawer trượt êm ái từ phải sang trái, hiển thị đủ 8 tầng thông tin.│
│ [ ] AC-22: URL tự động cập nhật tham số ?project=... khi Drawer mở và hỗ trợ nút Back.         │
│ [ ] AC-23: Team Tab cho phép lọc theo 4 phòng ban và mở xem modal bằng cấp chứng thực.         │
│ [ ] AC-24: Form Demo Booking kiểm tra đúng Regex SĐT Việt Nam và phân hạng cơ sở y tế B2G.      │
│ [ ] AC-25: Submit form demo thành công hiển thị mã ticket dạng TEK-B2G-2026-XXXX và cam kết SLA.│
└─────────────────────────────────────────────────────────────────────────────────────────────────┘
```

---

### 8.2 Ma Trận Kiểm Thử Chấp Nhận & Tiêu Chuẩn Hiệu Năng (QA Matrix & Core Web Vitals)

| Tiêu Chí Hiệu Năng / Trải Nghiệm | Phương Pháp Đo Lường | Ngưỡng Tiêu Chuẩn Cho Phép | Kết Quả Mục Tiêu |
|---|---|:---:|:---:|
| **Largest Contentful Paint (LCP)** | Google Lighthouse (Desktop) | `< 2.5 giây` | **`1.15 giây` (Xuất sắc)** |
| **Cumulative Layout Shift (CLS)** | Chrome DevTools Performance | `< 0.1` | **`0.002` (Không giật khung hình)** |
| **First Input Delay (FID) / INP** | Web Vitals Chrome Extension | `< 100 mili-giây` | **`18 mili-giây` (Phản hồi tức thì)** |
| **Speed Index (Tốc độ hiển thị)** | WebPageTest (Cable 4G Connection) | `< 2.0 giây` | **`1.35 giây`** |
| **Độ Tương Phản Màu Sắc (Contrast)**| WCAG 2.1 Accessibility Audit | Tối thiểu `AA (4.5:1)` | **Đạt `AAA (7.2:1)` cho tiêu đề** |
| **Tỷ Lệ Lỗi Console (Console Errors)**| Trình thu thập log trình duyệt | `0 Lỗi (Zero Errors)` | **0 Warnings, 0 Errors** |
| **Tính Toàn Vẹn Liên Kết (Broken Links)**| Screaming Frog SEO Spider | `0 Link 404` | **100% Liên kết nội bộ 200 OK** |

---

## 9. KẾT LUẬN & THÔNG ĐIỆP BÀN GIAO CHO BAN LÃNH ĐẠO TEKNOVA

Tài liệu **Báo Cáo Đối Soát Toàn Diện & Kế Hoạch Hành Động Dev (PRD) — Nâng Cấp Portal TEKNOVA 2026** này xác lập một bước chuyển mình mang tính bước ngoặt cho năng lực công nghệ và hình ảnh thương hiệu của Công ty Cổ phần Đổi mới Sáng tạo TEKNOVA.

Bằng việc kiên quyết:
1. **Khôi phục Chân lý Dữ liệu**: Khẳng định tư cách lãnh đạo tối cao của **Ông TRẦN BÌNH SƠN (MBA, Kỹ sư Điện tử)**, tôn vinh chất xám của **12 nhân sự chuyên gia** và minh chứng chiều sâu thực tiễn qua **22 hợp đồng dự án thực tế** đã nghiệm thu tại Đà Nẵng và cả nước;
2. **Triệt phá các sai phạm thị giác**: Chấm dứt vĩnh viễn tình trạng ảnh thumbnail trắng toát, dẹp bỏ toàn bộ đối tác chưa ký kết chính thức và xóa sạch các văn mẫu AI sáo rỗng;
3. **Trang bị 5 cỗ máy trình diễn B2G tương tác**: Tái hiện sống động quy trình lâm sàng EMR, trao tận tay cuốn hồ sơ năng lực 2026 lật trang siêu tốc và xác lập cam kết SLA phục vụ 24 giờ chuyên nghiệp;

Nền tảng **TEKNOVA Portal 2026** sẽ trở thành niềm tự hào công nghệ, một vũ khí bán hàng đắc lực và là bảo chứng niềm tin không thể lay chuyển giúp TEKNOVA tự tin khẳng định vị thế một trong những doanh nghiệp giải pháp Y tế số & Chính quyền số hàng đầu Miền Trung trong năm 2026 và các năm tiếp theo.
