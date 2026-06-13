# 📊 Phân Tích Thị Trường Tuyển Dụng Ngành Data Science Tại Việt Nam

## Giới thiệu

Đây là dự án phân tích dữ liệu tuyển dụng trong lĩnh vực **Data Science, Data Analyst và Machine Learning Engineer** tại Việt Nam.

Mục tiêu của dự án là thu thập dữ liệu tuyển dụng từ nhiều nền tảng việc làm, áp dụng các kỹ thuật xử lý ngôn ngữ tự nhiên (NLP) và Topic Modeling để khám phá:

* Các kỹ năng được nhà tuyển dụng yêu cầu nhiều nhất
* Xu hướng tuyển dụng trong lĩnh vực Data
* Mối quan hệ giữa kỹ năng, vị trí công việc và nhu cầu thị trường
* Những nhóm kỹ năng nổi bật dành cho sinh viên và người mới bắt đầu

---

## Thành viên thực hiện

* Nguyễn Hoàng Anh
* Hà Thế Anh
* Bạch Quang Tùng

---

## Dữ liệu sử dụng

Dữ liệu được thu thập từ nhiều nguồn tuyển dụng:

* VietnamWorks
* LinkedIn
* TopCV
* ITviec
* JobOKO

Các bộ dữ liệu được lưu trong thư mục:

```bash
Datasets/
```

Bao gồm:

* vietnamworks_jobs_detail.csv
* TopCV_Data.xlsx
* data_science_jobs.xlsx
* data wed It viec.xlsx
* joboko_phan_loai.xlsx
* data linkedin.xlsx

---

## Quy trình thực hiện

### 1. Thu thập dữ liệu

Notebook:

```bash
Code/vietnamworks_crawl.ipynb
```

Chức năng:

* Crawl danh sách việc làm
* Thu thập mô tả công việc
* Thu thập kỹ năng yêu cầu
* Lưu dữ liệu dưới dạng CSV

---

### 2. Gộp dữ liệu

Notebook:

```bash
Code/Gop_du_lieu.ipynb
```

Thực hiện:

* Hợp nhất dữ liệu từ nhiều nguồn
* Loại bỏ dữ liệu trùng lặp
* Chuẩn hóa cấu trúc dữ liệu

---

### 3. Tiền xử lý dữ liệu

Notebook:

```bash
Code/Step1_preprocessing.ipynb
```

Các bước xử lý:

* Làm sạch dữ liệu
* Loại bỏ ký tự đặc biệt
* Chuẩn hóa văn bản
* Tokenization
* Stopwords Removal
* Chuẩn hóa kỹ năng

---

### 4. Topic Modeling

Notebook:

```bash
Code/Step2_TopicModeling.ipynb
```

Các mô hình được thử nghiệm:

#### BERTopic + E5-Large

* Embedding: multilingual-e5-large
* Topic Modeling: BERTopic

#### BERTopic + BGE

* Embedding: BGE

#### BERTopic + LaBSE

* Embedding: LaBSE

#### Top2Vec

* Khám phá chủ đề tự động

Mục tiêu:

* Xác định các nhóm kỹ năng phổ biến
* So sánh chất lượng giữa các mô hình
* Đánh giá khả năng biểu diễn chủ đề

---

### 5. Trực quan hóa

Notebook:

```bash
Code/Step3_Visualiztion.ipynb
```

Bao gồm:

* Topic Distribution
* Topic Frequency
* Word Importance
* Topic Relationship
* Skill Analysis
* Demand Analysis

---

## Kết quả

Kết quả đánh giá mô hình được lưu tại:

```bash
Results/
```

File:

```bash
complete_model_evaluation_report.csv
```

Các chỉ số đánh giá:

* Topic Coherence
* Topic Diversity
* Topic Quality
* Topic Representation

---

## Công nghệ sử dụng

### Ngôn ngữ

* Python

### Thư viện

* Pandas
* NumPy
* Scikit-learn
* BERTopic
* Sentence Transformers
* Top2Vec
* Matplotlib
* Seaborn
* Plotly
* OpenPyXL

### NLP & Embedding Models

* Multilingual E5-Large
* BGE
* LaBSE

---

## Cấu trúc thư mục

```bash
Project_Phan_Tich_Nghe_Nghiep/
│
├── Code/
│   ├── vietnamworks_crawl.ipynb
│   ├── Gop_du_lieu.ipynb
│   ├── Step1_preprocessing.ipynb
│   ├── Step2_TopicModeling.ipynb
│   └── Step3_Visualiztion.ipynb
│
├── Datasets/
│   ├── vietnamworks_jobs_detail.csv
│   ├── TopCV_Data.xlsx
│   ├── data_science_jobs.xlsx
│   └── ...
│
├── Results/
│   └── complete_model_evaluation_report.csv
│
└── README.md
```

---

## Mục tiêu học thuật

Dự án được xây dựng nhằm:

* Nghiên cứu ứng dụng NLP trong phân tích thị trường lao động
* So sánh hiệu quả các mô hình Topic Modeling hiện đại
* Khám phá xu hướng kỹ năng trong lĩnh vực Data Science tại Việt Nam
* Hỗ trợ sinh viên định hướng học tập và phát triển nghề nghiệp

---

## Hướng phát triển

* Tích hợp Dashboard Power BI
* Tự động cập nhật dữ liệu tuyển dụng theo thời gian thực
* Xây dựng hệ thống gợi ý kỹ năng cần học
* Phân tích xu hướng tuyển dụng bằng LLM
* Xây dựng Career Recommendation System

```
```
