# 🛒 E-Commerce Customer Segmentation (ABC Analysis)

![Python](https://img.shields.io/badge/Python-3.13.16-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge&logo=python&logoColor=white)

---

## 💼 1. Business Problem

Thay vì phân bổ ngân sách Marketing cào bằng, dự án thực hiện phân loại $17,415$ khách hàng theo phương pháp **ABC Analysis** nhằm:
- **Tối ưu ROI:** Xác định tệp khách hàng gánh phần lớn lợi nhuận toàn hệ thống.
- **Vận hành hiệu quả:** Lọc Top 500 khách hàng VIP nhận quà tri ân khi ngân sách có hạn.
- **Tối ưu Acquisition:** Tìm điểm phân hóa thực sự để thu hút tệp khách hàng Nhóm A mới.

---

## 🛠️ 2. Tech Stack

- **Ngôn ngữ:** Python 3.13.16
- **Thư viện:** `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`
- **Phương pháp Phân tích:** Pareto 80/20, Cumulative Sum Indexing, Data Profiling & Visualization

---

## 📊 3. Key Insights

- **Quy luật Pareto 80/20 chuẩn xác:** 
  - **Nhóm A:** Chiếm **12.9%** số lượng ($2,254$ khách) nhưng đóng góp **80.0%** tổng lợi nhuận ($852,242).
  - **Nhóm B:** Chiếm **7.0%** số lượng ($1,217$ khách), đóng góp **15.0%** lợi nhuận ($159,831).
  - **Nhóm C:** Chiếm **80.1%** số đông ($13,944$ khách) nhưng chỉ mang lại **5.0%** lợi nhuận ($53,340).
- **Xử lý bài toán 500 quà VIP:** Nhóm A ($2,254$ người) vượt quá 500 suất. Giải pháp là lọc **Top 500 khách hàng có Lợi nhuận cao nhất trong Nhóm A** để trao quà, số còn lại tri ân bằng E-voucher đặc quyền.
- **Nghịch lý Nhân khẩu học:** Thu nhập trung bình 3 nhóm bằng nhau ($\sim \$56k - \$57k$) và cơ cấu ngành nghề tương đồng. **Điểm tạo nên Nhóm A nằm ở Hành vi tiêu dùng (Tần suất & Giá trị đơn hàng), không nằm ở Thu nhập.**

---

## 💡 4. Actionable Recommendations

### 🎯 A. Thu hút Khách hàng A mới (Acquisition)
1. **Bỏ Target theo Thu nhập cao:** Ngừng phung phí ngân sách vào các Adset lọc theo "Thu nhập $> \$100k$".
2. **Chạy Quảng cáo Lookalike (1% LAL):** Dùng $2,254$ ID khách Nhóm A làm dữ liệu hạt giống để AI nền tảng tự tìm kiếm người dùng mới có hành vi tương đồng.

### 📈 B. Nâng hạng Tệp Hiện tại (Retention & Growth)
1. **Chuyển hóa B $\rightarrow$ A:** Nhóm B ($1,217$ khách) là tệp tiềm năng nhất. Áp dụng **Combo Cross-sell** và **Loyalty Program** để kích thích họ tăng tần suất mua sắm chạm ngưỡng Nhóm A.
2. **Chi phí thấp cho Nhóm C:** Áp dụng Marketing tự động (Email/Push) giới thiệu các mặt hàng có biên lợi nhuận cao, tối ưu chi phí phục vụ.

---

Dự án được thực hiện bởi Vương Nghiệp Thuận
