# BTL_CSE_Machine-Learning
Dự án: Dự đoán chất lượng rượu vang (Wine Quality Prediction)

Dự án thuộc môn Học Máy của nhóm 14, sử dụng bộ dữ liệu Wine Quality – White Wine (UCI Machine Learning Repository) với 4898 mẫu và 11 đặc trưng hóa học để dự đoán chất lượng rượu vang.

🎯 Mục tiêu

Phân loại chất lượng rượu vang trắng thành 3 mức:

Thấp (quality < 5)

Trung bình (5–7)

Cao (quality > 7)

Xây dựng, huấn luyện và đánh giá hai mô hình học máy:

Logistic Regression

Decision Tree (ID3)

Tạo giao diện người dùng (Tkinter) cho phép nhập thông số rượu và dự đoán chất lượng.

📊 Dữ liệu & đặc trưng

Bộ dữ liệu gồm 11 thuộc tính hóa học:
fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, free sulfur dioxide, total sulfur dioxide, density, pH, sulphates, alcohol.

Nhãn đầu ra (quality) được quy đổi thành 3 lớp để phù hợp bài toán phân loại.

⚙️ Quy trình thực hiện

Tiền xử lý dữ liệu

Làm sạch dữ liệu, xử lý thiếu.

Chuẩn hóa đặc trưng (StandardScaler).

Chia dữ liệu Train/Test (80/20).

Khám phá dữ liệu (EDA)

Heatmap tương quan.

Phân cụm bằng K-Means để quan sát xu hướng chất lượng.

Huấn luyện mô hình

Logistic Regression (multinomial) + GridSearch tìm tham số tối ưu.

Decision Tree (ID3 – entropy) + tối ưu siêu tham số.

Đánh giá

Accuracy, F1-macro.

Confusion Matrix.

Xây dựng giao diện đồ họa (Tkinter)

Cho phép nhập 11 đặc trưng rượu.

Chọn mô hình (Logistic/Decision Tree).

Trả kết quả & độ tin cậy.

Hiển thị hình minh họa mô hình (cây quyết định / trọng số logistic).

📈 Kết quả
Mô hình	Accuracy	F1-macro	Nhận xét
Decision Tree (ID3)	0.9245	0.37	Hiệu suất tốt, mô tả được quan hệ phi tuyến, dễ trực quan hóa
Logistic Regression	0.4612	0.31	Tốc độ nhanh nhưng không phù hợp dữ liệu phi tuyến

➡️ Decision Tree cho kết quả vượt trội, phù hợp nhất cho bài toán này.

💡 Hướng phát triển

Kết hợp mô hình Random Forest để giảm overfitting.

Thử nghiệm SVM hoặc XGBoost.

Dùng SMOTE để xử lý mất cân bằng lớp.

Tối ưu tham số sâu hơn bằng Grid Search mở rộng.

🖥️ Công nghệ sử dụng

Python

scikit-learn

pandas, numpy

matplotlib, seaborn

Tkinter (giao diện người dùng)
