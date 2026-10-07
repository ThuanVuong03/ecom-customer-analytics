# 🛒 E-Commerce Customer Segmentation (ABC Analysis) & Marketing Strategy Optimization

![Python](https://img.shields.io/badge/Python-3.13.16-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Data Analytics](https://img.shields.io/badge/Analytics-E--Commerce-FF6F00?style=for-the-badge)

---

## 💼 1. Business Problem

Trong lĩnh vực Thương mại điện tử (E-Commerce), việc dàn trải ngân sách Marketing và áp dụng chính sách chăm sóc khách hàng cào bằng thường dẫn đến **lãng phí chi phí thu hút (CAC) cao nhưng ROI thu về lại thấp**. 

Dự án này tập trung giải quyết các bài toán kinh doanh cốt lõi:
- **Tối ưu hóa nguồn lực:** Phân loại $17,415$ khách hàng theo phương pháp **ABC Analysis** để xác định đâu là nhóm khách hàng thực sự mang lại phần lớn lợi nhuận cho công ty.
- **Kiểm chứng quy luật Pareto (80/20):** Đánh giá mức độ tập trung lợi nhuận để đưa ra chiến lược phân bổ ngân sách hợp lý.
- **Giải quyết bài toán vận hành thực tế:** Phương án xử lý tối ưu khi công ty chỉ có $500$ suất quà VIP nhưng danh sách tri ân vượt quá số lượng cho phép.
- **Định hình chân dung Marketing:** Tìm kiếm điểm phân hóa nhân khẩu học (Thu nhập, Ngành nghề) để tối ưu chiến dịch Acquisition thu hút tệp khách hàng Nhóm A mới.

---

## 🛠️ 2. Tech Stack

- **Ngôn ngữ xử lý:** Python 3.13.16
- **Thư viện thao tác dữ liệu:** `Pandas`, `NumPy` (Merge, GroupBy, Aggregation, Cumulative Sum, Pareto Indexing)
- **Trực quan hóa dữ liệu:** `Matplotlib`, `Seaborn` (Donut Chart, Grouped Bar Chart, Boxplot)
- **Môi trường thực thi:** Google Colab / Jupyter Notebook

---

## 📊 3. Key Insights & Visualization

### 📌 Insight 1: Tuân theo hoàn hảo Quy luật Pareto (80/20)
- **Nhóm A:** Chỉ chiếm **12.9%** tổng số lượng khách hàng ($2,254$ khách) nhưng tạo ra **80.0% tổng lợi nhuận** toàn hệ thống ($852,242).
- **Nhóm B:** Chiếm **7.0%** khách hàng ($1,217$ khách), đóng góp **15.0%** lợi nhuận ($159,831).
- **Nhóm C:** Chiếm **80.1%** số đông ($13,944$ khách) nhưng chỉ mang lại **5.0%** lợi nhuận ($53,340).

> 💡 **Nhận xét đắt giá:** Mô hình kinh doanh phụ thuộc nặng nề vào 12.9% khách hàng nòng cốt. Việc giữ chân Nhóm A là ưu tiên sống còn của doanh nghiệp.

---

### 📌 Insight 2: Bài toán 500 Suất quà VIP
- Danh sách Nhóm A ($2,254$ người) vượt xa hạn mức $500$ suất quà đặc biệt.
- Lọc **Top 500 khách hàng đóng góp Profit cao nhất** giúp đảm bảo quà tặng trao đúng cho nhóm $22\%$ đỉnh bảng - những người trực tiếp gánh phần lớn chỉ số ROI của doanh nghiệp.

---

### 📌 Insight 3: Nghịch lý Nhân khẩu học (The Demographic Paradox)
- **Mức thu nhập trung bình:** Nhóm A ($56,681$), Nhóm B ($55,982$) và Nhóm C ($57,379$) gần như **bằng nhau tuyệt đối**.
- **Cơ cấu Ngành nghề:** Cả 3 nhóm đều có tỷ lệ tương đồng lớn về các ngành nghề chính (*Professional* $\approx 29-30\%$, *Skilled Manual* $\approx 25-26\%$).

> 💡 **Nhận xét đắt giá:** **Thu nhập và Ngành nghề không phải là yếu tố tạo nên giá trị của Nhóm A.** Sự phân hóa Nhóm A nằm ở **Hành vi tiêu dùng** (Tần suất mua sắm, Giá trị đơn hàng và Lựa chọn sản phẩm có biên lợi nhuận cao).

---

## 💡 4. Strategic Recommendations

Dựa trên kết quả phân tích dữ liệu, chiến lược Marketing đề xuất tập trung vào 2 trụ cột chính:

### 🎯 A. Acquisition (Thu hút Khách hàng Nhóm A Mới)
1. **Chuyển dịch sang Target theo Hành vi (Behavioral Targeting):** Dừng việc ngốn ngân sách vào các Adset lọc theo "Thu nhập cao" ($> \$100k$) hoặc "Chức danh cao cấp".
2. **Khai thác Lookalike Audience (1% LAL):** Export danh sách $2,254$ ID/Email khách hàng Nhóm A hiện tại làm dữ liệu hạt giống (Seed Data) để chạy quảng cáo Lookalike trên Meta Ads & Google Ads. Thuật toán AI sẽ tìm kiếm những người dùng mới có hành vi tương đồng.

### 📈 B. Retention & Growth (Nâng hạng Tệp Hiện tại)
1. **Chiến dịch "B to A Upselling":** Tệp Nhóm B ($1,217$ khách hàng) là tệp tiềm năng nhất. Áp dụng chính sách **Combo Cross-sell** và **Tiered Loyalty Program** (Hạng thành viên tích điểm) để thúc đẩy họ gia tăng tần suất mua sắm chạm ngưỡng Nhóm A.
2. **Chiến lược Tri ân Phân tầng (Tiered Rewards):**
   - **Top 500 Nhóm A:** Tặng Quà VIP đặc biệt.
   - **1,754 khách Nhóm A còn lại:** Tặng E-voucher đặc quyền hạng Gold.
