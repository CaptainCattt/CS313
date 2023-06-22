# CS313
# KHAI THÁC DỮ LIỆU GIÁO DỤC NHẰM DỰ ĐOÁN KẾT QUẢ HỌC TẬP CỦA SINH VIÊN
# NỘI DUNG

# 1. Giới thiệu
1.1 Tổng quan

Đánh giá kết quả học tập của ứng viên trong quá trình học đại học là một trong
những tiêu chí phổ biến được sử dụng trong quá trình tuyển dụng nguồn nhân lực của
các công ty và doanh nghiệp. Trong giai đoạn đầu tiên của cuộc sống học đại học, sinh
viên đối mặt với nhiều thay đổi và áp lực mới. Có rất nhiều yếu tố ảnh hưởng đến kết
quả học tập của sinh viên, chẳng hạn điều kiện, khả năng học tập, môi trường học tập,
độ tuổi, sức khỏe và tâm lý, giới tính hay nền tảng giáo dục trước đó. Liệu các yếu tố độ
tuổi, giới tính và nền tảng giáo dục trước đó có thể ảnh hưởng nhiều đến sự thích nghi
và thành công trong quá trình học tập của sinh viên.

1.2 Phát biểu bài toán

Bài toán dự đoán sinh viên có qua một môn hay không dựa trên các môn cơ sở
ngành đặt ra mục tiêu tìm hiểu và phân tích mối quan hệ giữa kết quả học tập của sinh
viên trong các môn học trước đó và môn học dự đoán [3]. Khả năng dự đoán kết quả
học tập có thể giúp các nhà quản lý giáo dục và giảng viên đưa ra các biện pháp hỗ trợ
phù hợp để nâng cao hiệu quả học tập và thành công của sinh viên đại học.
Với mục đích dự đoán được dữ liệu của kết quả học các môn học trước như Giải
tích, Xác suất thống kê, Nhập môn lập trình, Cấu trúc dữ liệu và giải thuật...có ảnh
hưởng như thế nào đến việc sinh viên có qua môn Lập trình hướng đối tượng hay không,
nhóm đề ra mục tiêu ban đầu xử lý lại bộ dữ liệu Education_dataset_v2 để được bộ dữ
liệu phù hợp với mục đích của bài toán mà nhóm đã đặt ra. Sau đó tiến hành cài đặt và
triển khai thực nghiệm các mô hình trên bộ dữ liệu sau khi đã được xử lý, từ đó thu thập
được các kết quả thực nghiệm khác nhau trên từng mô hình, từng phương pháp.
Bài toán nhận đầu vào là điểm của sinh viên trong các môn học trước đó, đầu ra
là dự đoán xem sinh viên có qua môn Lập trình hướng đối tượng hay không.

1.3 Thách thức
1.4 Đối tượng và phạm vi
1.5 Mục tiêu

# 2. Mô hình giải bài toán

2.1 Các bước tiền xử lý dữ liệu
- Làm sạch dữ liệu
  
  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/2b9d0344-b3f2-4c94-92f1-4b38f516b399)
  
- Tích hợp dữ liệu

  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/b93edb17-988f-4514-9042-5815b582d0ad)
  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/ec79b8a2-02ec-4a80-988a-f963f56d1e5f)
  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/44440750-298c-4489-bdbd-a24bce8b2b78)
  
- Biến đổi dữ liệu

  
  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/81ea3bc9-ade6-4df2-ac46-a1e5345d1a6b)
  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/b629be20-9e17-4241-884e-8bf63caab270)

  
- Rút gọn dữ liệu

  
  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/c05e149a-d8c7-4f2b-9aa6-2b116ca33991)
  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/0ccf5793-46d6-437d-8869-9942f84edcb8)

2.2 Các thuộc tính được sử dụng

- 01_sv_nentangGD.csv
- 02_sv_xeploaiHK.csv
- 03_diem_v1.csv
- 04_diem_v2.csv

2.3 Phương pháp đề xuất

- Support Vector Machine (SVM):
- Logistic Regression:
- Random Forest:
- K-Nearest Neighbors (KNN):
- Decision Tree:
- Sử dụng kỹ thuật Ensemble Learning (Voting Classifier)
- SMOTE (Synthetic Minority Over-sampling Technique)
- Stochastic Gradient Descent (SGD):
- MLP là viết tắt của Multi-Layer Perceptron (Perceptron đa tầng):
- Passive Aggressive:
- Mini Batch KMeans:
- Gradient Boosting:
- Cat Boost:

# 3. Cài đặt thực nghiệm

3.1 Dataset

Dữ liệu được đưa vào sử dụng bao gồm 8044 dòng và 21 cột. Được chia làm
thành tập train và tập test với tỉ lệ 0.8 và 0.2 (tương ứng 6426 và 1069 dòng dữ liệu).
Trong quá trình thực nghiệm mô hình chia theo phương pháp cross-validation với hệ
số k = 5.

3.2 Phương pháp đánh giá

Khi thực hiện bài toán phân loại, có 4 trường hợp của dự đoán có thể xảy ra:
− True Positive (TP): đối tượng ở lớp Positive, mô hình phân đối tượng vào lớp
Positive (dự đoán đúng).
− True Negative (TN): đối tượng ở lớp Negative, mô hình phân đối tượng vào lớp
Negative (dự đoán đúng).
− False Positive (FP): đối tượng ở lớp Negative, mô hình phân đối tượng vào lớp
Positive (dự đoán sai).
− False Negative (FN): đối tượng ở lớp Positive, mô hình phân đối tượng vào lớp
Negative (dự đoán sai).


![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/6f47cbb9-3c43-4023-9de6-f355709f646e)

- Confusion matrix

  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/3dd53118-03ec-429e-812c-d684e6f2df35)

- Accuracy

  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/20a7f3e4-284d-4b79-bffe-401b97920742)

- F1_score

  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/7f782168-ac9a-4c47-9110-c3e00a449e68)

  ![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/11baf3da-5685-4e16-a101-aab99cf74420)

3.3 Phương pháp thực nghiệm
- Thuật toán Naive Bayes với hyperparameters: {'var_smoothing': 1e-09}.
- Thuật toán SVM với hyperparameters: {'C': 1, 'gamma': 0.1, 'kernel': 'rbf'}.
- Thuật toán Gradient Boosting với hyperparameters: {'learning_rate': 0.01,'max_depth': 5}.
- Thuật toán Cat Boost với hyperparameters: {iterations = 1500, learning_rate = 0.02, depth = 6, l2_leaf_reg = 0.9, class_weight = mảng % phân bố nhãn của các lớp }.
- Kết hợp giữa các mô hình thuật toán lại với nhau bao gồm (SVM, Logistic Regression, Random Forest, KNN, Decision Tree) phương pháp Voting Classifier để kết hợp nhiều mô hình với { KNN: n_neighbors=5, Decision Tree: max_depth=5, SVM: kernel='rbf', C=1.0, Logistic Regression: solver='liblinear', RandomForest: n_estimators=100, max_depth=10}.Thuật toán tăng cường: SGD với hyperparameters: {loss='log',learning_rate = 'optimal', penalty='elasticnet', max_iter=1000, tol=1e-3, random_state=42}.
- Thuật toán tăng cường: MLP với hyperparameters: { hidden_layer_sizes=(200, 200)}.
- Thuật toán tăng cường: : PassiveAggressive.
- Thuật toán tăng cường: MiniBatchKMeans với hyperparameters: {n_clusters=5, batch_size=300}.
- Thuật Toán Random Forest kết hợp SMOTE: Hyperparameters: (n_estimators=100, random_state=42)



