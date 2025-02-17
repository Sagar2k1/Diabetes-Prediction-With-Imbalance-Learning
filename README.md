# Dự đoán bệnh tiểu đường với Dữ Liệu Không Cân Bằng

# 1. Thông tin dự án

Trong những năm gần đây, bệnh tiểu đường có xu hướng gia tăng trên thế giới. Theo số liệu của IDF vào 2045, nhóm bệnh nhân ở độ tuổi 20 – 79 dự báo sẽ có gần 800 triệu ca, tốn hơn 1000 tỷ đô la Mỹ ngân sách dành cho y tế. Với xu hướng gia tăng của bệnh, việc xây dựng một mô hình dùng để dự đoán là một trong những điều cần thiết. Trong học máy, việc xử lý dữ liệu không cân bằng là một vấn đề cần giải quyết trong giai đoạn tiền xử lý dữ liệu. Việc thiếu dữ liệu hay dư thừa dữ liệu ở một hay nhiều phân lớp bài toán là nguyên nhân gây ra việc suy giảm hiệu suất trong tính toán. Bài báo cáo này tập trung vào nghiên cứu các phương pháp xử lý dữ liệu qua đây cải thiện một số vấn đề mà các nghiên cứu trước đây còn tồn đọng. Các giả thuyết của Fernández và cộng sự (2018) cũng như phương pháp thực nghiệm của Trịnh (2024) là một trong những giả thuyết và phương pháp thực nghiệm được sử dụng trong bài. Qua đó, các kết quả nghiên cứu được cải thiện nhất là dự đoán chính xác các phân lớp thiểu số.

# 2. Cây thư mục
Cây thư mục của source code
```
    source.
        ├───Code -- folder chứa code của dự án
        │   ├───d1 -- chứa các file chạy code
        │   ├───d2
        │   └───d6
        ├───Data
        │   ├───d1
        │   │   └───Balanced Data -- Chứa data sẽ chạy mô hình (train, test và data đã được cân bằng)
        │   ├───d2
        │   │   └───Balanced Data
        │   └───d6
        │       └───Balanced Data
        ├───Result -- Các kết quả chạy code (thời gian chạy, kích thước từng phân lớp, kết quả chạy mô hình)
            ├───d1
            │   └───Scores -- Các kết quả chạy mô hình sau cùng (Precision, Average Precision, Recall, etc.)
            ├───d2
            │   └───Scores
            └───d6
                └───Scores
```



# 3. Các bước chạy code

. Bước 1. Mở Thư mục Code. Chạy lệnh 

```
    ! pip install -r requirements.txt
```

để chạy set up môi trường

. Bước 2. Ở từng folder d1, d2, d6 chứa 3 file .ipynb

```
    .d6
        Data Cleaning.ipynb -- file tiền xử lý input
        Data Engineering.ipynb -- file xử lý dữ liệu, huấn luyện mô hình và 
        Modelling and Testing.ipynb
```

. a chạy file Data Cleaning.ipynb. Kết quả được trả tại folder /Data/Tên tập dữ liệu/*_cleaned.csv
. b chạy file Data Engineering.ipynb. Kết quả được trả tại folder /Data/Tên tập dữ liệu/
    . Với Mỗi tập cân bằng kết quả được lưu trong /Data/Tên tập dữ liệu/Balanced Data
. c chạy file Modelling and Testing.ipynb để huấn luyện mô hình. Kết quả được trả tại folder /Result/Tên tập dữ liệu

