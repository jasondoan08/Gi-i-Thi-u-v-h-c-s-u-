# Pandas 

các khái niệm cơ bản của **Pandas** trong Python. Từ cách tạo Series/DataFrame, indexing, slicing, đến groupby, aggregate và merge dữ liệu.

## Công nghệ sử dụng
- Pandas
- NumPy
- Jupyter Notebook

## Nội dung chính

Notebook bao gồm:

- Tạo Series từ list, array, dictionary, scalar
- Indexing, slicing, masking, fancy indexing
- Tạo DataFrame nhiều cách (dict, list of dict, numpy array…)
- Các thuộc tính: `.values`, `.index`, `.columns`
- Broadcasting và alignment
- GroupBy: sum, mean, median, aggregate, filter, transform, apply
- Xử lý missing data, merge DataFrame

## 2 bài tập thực hành (Life Expectancy dataset)

Dataset: [Life Expectancy (WHO) – Kaggle](https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who) 
### Bài tập 1
- Đọc file CSV
- Xem 2 dòng đầu/cuối, shape, columns, describe
- Xóa 2 cột không cần thiết: `Hepatitis B`, `Population`
- Chuyển cột `Status` thành số (Developed = 1, Developing = 0)

### Bài tập 2
- Đếm missing value mỗi cột
- Fill missing bằng mean của cột tương ứng
- Groupby theo **Country** → tìm quốc gia có tuổi thọ trung bình thấp nhất / cao nhất
- Groupby theo **Status** → so sánh tuổi thọ trung bình giữa Developed và Developing
- Tạo DataFrame mới với cột ID (tên quốc gia) + Noise_level (random)
- Merge 2 DataFrame dựa trên cột ID/Country

## Cách chạy

1. Tải dataset từ link Kaggle ở trên (file `Life Expectancy Data.csv`)
2. Đổi tên thành `howlongwelive.csv` (hoặc sửa lại tên file trong notebook)
3. Mở file `Pandas.ipynb` bằng Jupyter Notebook / VS Code / Google Colab
4. Chạy từng cell từ trên xuống dưới

## Kết quả nổi bật (từ dataset)

- Tuổi thọ trung bình toàn cầu ~69 năm
- Developed countries: ~80 năm
- Developing countries: ~67–68 năm
- Quốc gia thấp nhất: thường là Sierra Leone hoặc một số nước châu Phi (~46–50 năm)
- Quốc gia cao nhất: thường là Nhật Bản hoặc một số nước châu Âu (~82–83 năm)

hết ạ. Chúc thầy Anh và anh Hải ăn tết vui vẻ <3
