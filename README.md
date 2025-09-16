# Data Lakehouse for Fitness Classification Analytics

## 📌 Giới thiệu
Đồ án tốt nghiệp: **Xây dựng hệ thống Data Lakehouse phục vụ phân tích dữ liệu phân loại thể chất**  
(*Design and Implementation of a Data Lakehouse for Fitness Classification Data Analytics*)  

Mục tiêu:
- Xây dựng pipeline Data Lakehouse (ingestion → transform → lưu trữ → phân tích).
- Sử dụng dataset **Fitness Classification (Kaggle)**.
- Trực quan hóa kết quả bằng dashboard (Power BI hoặc Apache Superset).

---

## 🛠 Công nghệ sử dụng
- **Apache Spark (PySpark)** – xử lý & transform dữ liệu.
- **Delta Lake** – quản lý dữ liệu (ACID, schema, time travel).
- **MinIO / AWS S3** – lưu trữ dữ liệu dạng object.
- **Power BI / Apache Superset** – trực quan hóa dữ liệu.
- **Python, SQL** – xử lý và phân tích dữ liệu.

---

## 📂 Cấu trúc thư mục

data-lakehouse-fitness/
│
├── data/ # Dữ liệu
│ ├── raw/ # Dữ liệu gốc (CSV từ Kaggle)
│ └── processed/ # Dữ liệu đã xử lý (Parquet / Delta)
│
├── notebooks/ # Jupyter/PySpark notebooks cho EDA & demo
├── scripts/ # ETL scripts (Python + PySpark)
├── reports/ # Báo cáo, hình ảnh, kết quả
│
├── requirements.txt # Danh sách thư viện Python cần thiết
└── README.md # Tài liệu mô tả dự án

---

## 🚀 Cách chạy (local)
1. Clone repo:
   ```bash
   git clone https://github.com/duongpham1411/data-lakehouse-fitness.git
   cd data-lakehouse-fitness
2. Tạo môi trường ảo và cài thư viện:
    python -m venv venv
    source venv/bin/activate   # hoặc venv\Scripts\activate trên Windows
    pip install -r requirements.txt
3. Chạy PySpark để test ingestion: pyspark
4. Mở notebook trong notebooks/ để khám phá dữ liệu.

---

## ✨ Kết quả dự kiến
- Hệ thống Data Lakehouse cơ bản (batch data pipeline).
- Dashboard hiển thị xu hướng và phân bố mức độ thể chất.
- So sánh hiệu quả lưu trữ & truy vấn giữa dữ liệu CSV và Delta/Parquet.
