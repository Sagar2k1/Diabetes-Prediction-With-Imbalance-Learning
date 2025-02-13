# Diabetes-Prediction-With-Imbalance-Learning

. Tên dự án: Dự đoán bệnh tiểu đường với Dữ Liệu Không Cân Bằng

# 1. Thông tin dự án

```
    Cập nhật sau
```




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
        │   ├───d1
        │   │   └───Scores -- Các kết quả chạy mô hình sau cùng (Precision, Average Precision, Recall, etc.)
        │   ├───d2
        │   │   └───Scores
        │   └───d6
        │       └───Scores
        └───Slide
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

