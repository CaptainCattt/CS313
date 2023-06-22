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

3.4 Kết quả thực nghiệm

![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/c1877d1c-c5e4-419e-b15c-1b2480f67621)

![image](https://github.com/CaptainCattt/CS313_PROJECT/assets/133556107/2955f712-ff8c-4b0a-be0b-693280583267)

# 4. Kết luận và hướng phát triển

Bài toán các yếu tố về nền tảng giáo dục trước đó có thể không thực sự ảnh hưởng
đến kết quả của điểm trung bình học kì kết quả đạt được từng kì là khác nhau và dao
động từ 43% - 69.9% với các mô hình SVM, Ensemble, Gradient Boosting. Ngoài ra
đối với điểm các môn trước (môn cơ sở ngành khác) có thể dự đoán được kết quả môn
học IT002 đạt kết quả phân loại khá cao với kết quả mô hình Logistic Regression
95.3982% đối với độ đo accuracy và mô hình Random Forest 76.02% với độ đo f1-
score. Đối với sinh viên, kết quả dự đoán này có thể giúp họ cải thiện khả năng đạt
được điểm số tốt trong IT002 bằng cách học tốt trong các môn học cơ sở ngành trước
đó và tham gia tích cực vào các hoạt động lớp học. Đối với giảng viên, việc dự đoán
này cung cấp một công cụ hữu ích để xác định những sinh viên có thể cần sự hỗ trợ
hoặc can thiệp thêm, giúp nâng cao chất lượng giảng dạy. Góp phần vào lĩnh vực khai
thác dữ liệu giáo dục bằng cách phát triển một phương pháp mới để dự đoán điểm số
của sinh viên dựa trên các khóa học trước và hiệu suất học tập. Phương pháp này có
thể giúp cả sinh viên và giảng viên cải thiện kết quả và trải nghiệm học tập của họ.


Hướng phát triển:
- Mở rộng bộ dữ liệu để bao gồm nhiều trường đại học và khóa học.
- Bổ sung thêm các biến vào mô hình dự đoán, chẳng hạn như các đặc tính cá nhân hoặc điểm phản hồi.
- Đánh giá hiệu suất của mô hình trong các bối cảnh và kịch bản khác nhau.
- Thêm các yếu tố tâm lý và tính cách như bài test MBTI để đánh giá một cách khách quan hơn.
- viên có thể đưa ra những lựa chọn phù hợp dựa trên đánh giá khách quan về điểm số và những thống kê từ các khóa học trước đó.

# 5. Tài liệu tham khảo

[1] M. H. R. J. L. a. A. J. Sweeney, "Next-term student performance prediction: A recommender
systems approach," arXiv:1604.01840, 2016.
[2] A. T. L. W. N. T. T. A. G. a. E.-P. L. Widjaja, "Next-term grade prediction: A machine learning
approach," (2020): 700..
[3] A. M. S. a. A. A.-E. Nabil, "Prediction of students’ academic performance based on courses’
grades using deep neural networks," 140731-140746, IEEE Access 9 (2021).
[4] "SMOTE for Imbalanced Classification with Python",

"https://machinelearningmastery.com/smote-oversampling-for-imbalanced-
classification/?fbclid=IwAR0sVHNWFU9bAtvxkRu70qDaR89xhwDHkBA05VwBsiQ0PwoVJ

yBO-MZ6L6I," ( Truy cập lần cuối: 28/05/2023).
[5] S. &. J. N. Musa Baig, "Stochastic Gradient Descent Algorithm (SGD).," 2022.
[6] Z. D. D. R. S. a. Q. V. L. Hanxiao Liu, "Pay Attention to MLPs," arXiv:2105.08050, 2021.
[7] T. S. a. J. Zhu, "Online Bayesian Passive-Aggressive Learning},"
https://doi.org/10.3389/fpsyg.2021.579183, 2013.
[8] B. A. Javier, "K-means vs Mini Batch K-means: a comparison," arXiv:1602.02934, 2013.
[9] D. L. T. L. M. W. Zhiyuan He, "Gradient Boosting Machine: A Survey," arXiv:1908.06951,
2019.
[10
]
G. G. A. V. A. V. D. A. G. Liudmila Prokhorenkova, "CatBoost: unbiased boosting with
categorical features," https://doi.org/10.48550/arXiv.1706.09516, 2019.
[11
]
"Scikitlearn," [Online]. Available: https://scikit-learn.org/stable/.

[12
]
"Coursera," [Online]. Available: https://www.coursera.org/learn/machine-learning.





