# CNN từ đầu tay - Phân loại ảnh (MNIST → CIFAR-10)

Lab nhỏ này mình làm để thực hành CNN thuần túy (không pre-trained, không ResNet, không transfer learning). Mục tiêu là đạt >90% accuracy trên các dataset khác nhau mà vẫn tránh overfit.

### Dataset đã thử
- MNIST (baseline, dễ đạt ~99%)
- CIFAR-10 (10 lớp, đạt ~91–93%)

### Những gì mình đã làm
- Tăng augmentation (RandomCrop, Flip, ColorJitter, Rotation…)
- Thêm BatchNorm + Dropout ở mỗi block
- Dùng AdamW + ReduceLROnPlateau
- WeightedRandomSampler (dù CIFAR-10 cân bằng nhưng vẫn dùng để ổn định)
- Early stopping + label smoothing nhẹ
- Không dùng mô hình phức tạp, chỉ CNN tự build (4–5 conv blocks)

### Kết quả nổi bật
- CIFAR-10: ~92.5% (test)

