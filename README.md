# Final Project: Coffee Quality Analysis and Prediction

> **รายวิชา:** 1145 201 คณิตศาสตร์สำหรับวิทยาการข้อมูล | ภาคการศึกษา 1/2568  
> **สถาบัน:** มหาวิทยาลัยอุบลราชธานี

---

## 👥 สมาชิกในกลุ่ม
1. **นางสาวปัญญาพร มูลดับ** — รหัสนักศึกษา 68114540399
2. **นางสาวรัชรินทร์ แสงศักดิ์** — รหัสนักศึกษา 68114540515

---

## 📌 รายละเอียดโครงงาน (Project Overview)
โครงงานนี้จัดทำขึ้นเพื่อศึกษาและวิเคราะห์ปัจจัยทางกายภาพและมิติรสชาติต่างๆ ที่ส่งผลต่อคะแนนรวมคุณภาพกาแฟ (**Total.Cup.Points**) โดยประยุกต์ใช้ความรู้ด้านคณิตศาสตร์สำหรับวิทยาการข้อมูล ได้แก่ Linear Algebra, Statistical Learning, Regression Modeling และ Model Evaluation ผ่าน Cross-Validation

* **Dataset:** [Coffee Quality Database (CQI)](https://www.kaggle.com/datasets/volpatto/coffee-quality-database-from-cqi?resource=download)
* **ไฟล์ข้อมูล:** `merged_data_cleaned.csv`

---

## 📊 สรุปผลการวิเคราะห์ (CLO Summary)

| CLO | หัวข้อการวิเคราะห์ | ผลการศึกษาหลัก |
|:---:|---|---|
| **CLO1** | Linear Algebra Analysis (PCA) | PC1 และ PC2 สามารถอธิบายความแปรปรวนของคุณลักษณะรสชาติกาแฟรวมกันได้ถึง **76.98%** (โดย PC1 อธิบายได้ถึง **63.33%**) |
| **CLO2** | Statistical Learning | รสชาติ (`Flavor`) และการตกค้างในลำคอ (`Aftertaste`) เป็นปัจจัยที่มี Correlation สูงที่สุดกับคะแนนรวมสุทธิ |
| **CLO3** | Model Building | โมเดล **Multiple Ridge Regression** ให้ประสิทธิภาพดีที่สุดโดยทำทำนายคะแนนกาแฟสุทธิได้ $R^2 = 0.6635$ |
| **CLO4** | Model Selection | การประเมินด้วย **5-Fold Cross-Validation** ยืนยันว่า Multiple Ridge ให้ค่า CV MSE ต่ำที่สุดชิ ($2.3489$) |

---

## 📁 โครงสร้างไฟล์ใน Repository
* `Coffee_Quality_Analysis_and_Prediction.ipynb` : ไฟล์ Notebook แสดงโค้ดการวิเคราะห์และกราฟผลลัพธ์
* `merged_data_cleaned.csv` : ชุดข้อมูลกาแฟที่ใช้ในการทดลอง
* `README.md` : สรุปภาพรวมและรายละเอียดของโครงงาน
