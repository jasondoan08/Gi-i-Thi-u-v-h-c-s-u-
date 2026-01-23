# Công nghệ sử dụng#
- Ngôn ngữ: Python 3
- **Thư viện chính**:
  - NumPy (np) – mảng đa chiều, indexing, slicing, boolean masking, tạo dữ liệu giả lập
- Môi trường: Jupyter Notebook / JupyterLab
# Cách hoạt động chính của code#

1. Tạo & chuyển đổi mảng NumPy 
   - Từ list Python → np.array()  
   - Tự động ép kiểu dữ liệu 
   - Chuyển kiểu: .astype(int)

2. Indexing & Slicing nâng cao
   - Truy cập phần tử: arr[i], arr[i,j]
   - Slicing: arr[start:end:step], arr[:, col], arr[rows, cols]
   - Lấy nhiều vị trí không liền kề: arr[[idx1, idx2, ...]] 
   - Indexing ngược: arr[-1, ::-1]

3. Boolean Masking & Điều kiện 
   - Tạo mask: arr % 2 == 0
   - Lọc dữ liệu: arr[mask]  
   - Kết hợp nhiều điều kiện: arr[(cond1) & (cond2) | cond3]

