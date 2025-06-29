# 🍬 Candy Detection Using YOLOv11s

## 🧭 Overview
This project is part of the final assignment for the **Computer Vision** course, titled **"Candy Detection Using YOLOv11s"**. The goal is to build an automatic detection system to identify candy using the YOLOv11s object detection algorithm. The system is designed to replace manual inspection processes in candy production lines, which are often inefficient and error-prone.

YOLOv11s is chosen for its speed, accuracy, and lightweight architecture, making it ideal for real-time detection tasks. The model is trained on a custom dataset consisting of normal and defective candy images. All training and testing are conducted using Google Colab.

---


## 📊 Dataset & Preprocessing

### 📸 Data Collection
- Images were captured from the production line using industrial cameras.
- Multiple lighting conditions and candy positions were recorded to increase data diversity.

### 📝 Preprocessing
- **Annotation**: Candy objects (normal and defective) were labeled using bounding boxes via LabelImg.
- **Augmentation**: Techniques like rotation, flipping, and brightness adjustment were applied to expand and balance the dataset.

---

## 🧠 YOLOv11s Model

- Utilizes the YOLOv11s architecture (lightweight version).
- Trained over 60 epochs using Google Colab.
- Dataset split: 90% training, 10% validation.
- Uses `data.yaml` for configuration.

---

## 📈 Evaluation Metrics

- Model performance is evaluated using **Precision**, **Recall**, and **mAP** (mean Average Precision).
- Each prediction includes a bounding box, class label, and confidence score.

---

## 🛠️ Tools & Frameworks

- 🧰 Ultralytics YOLOv5/YOLOv11s
- 💻 Google Colab
- 📦 Python (OpenCV, NumPy, Matplotlib, PyYAML)

---

## 🧪 Implementation Flow

1. Upload `data.zip` to Google Colab.
2. Extract and annotate the dataset.
3. Generate `data.yaml` configuration.
4. Train YOLOv11s model using the Ultralytics training command.
5. Test the model with new images.
6. Export the model as `.pt` or `.zip` for deployment.

---

## 🎯 Expected Output & System Mockup

- Accurate candy detection (normal vs defective).
- Supports multi-object detection in a single image.
- Real-time inference with confidence scores per object.
- Visual result display directly on the image.

**🖼️ System Mockup:**

Users upload an image of candy, then press the "Detect" button. The system displays bounding boxes and classifies each candy as normal or defective. The output includes class labels and confidence scores for each detected object.

---

## 📚 References

- Andhika, R., & Wijaya, A. (2021). *Implementasi YOLOv4 untuk Deteksi Buah Apel dan Jeruk pada Citra Digital*. Journal of Computer System and Technology, 9(2), 88–94. https://doi.org/10.14710/jtsiskom.9.2.2021.88-94  
- Kusumawati, D., & Firmansyah, A. (2022). *Penerapan YOLOv5 dalam Deteksi Kualitas Roti pada Jalur Produksi*. Journal of Informatics and Computation, 7(1), 45–52. https://doi.org/10.32672/jik.v7i1.5892  
- Liu, Y., Chen, C., & Wu, H. (2023). *Small Object Detection Based on Improved YOLOv7 Architecture*. IEEE Access, 11, 12934–12946. https://doi.org/10.1109/ACCESS.2023.3245678  

---

## 🚀 How to Try

1. Open Google Colab.
2. Upload `data.zip` and extract to the `custom_data/` folder.
3. Annotate data and configure `data.yaml`.
4. Run YOLO training with the appropriate command.
5. Test the model with new images.
6. Download `.pt` or `.zip` model file for future use.

---

## 💬 License

This project is developed for academic and educational purposes under the Computer Vision UAS at **Politeknik Caltex Riau**.

---

> You can add screenshots or Colab results under an `assets/` folder using:
>
> `![Detection Result](assets/detection_result.png)`

Let me know if you want me to generate a sample `requirements.txt`, `data.yaml`, or Colab `.ipynb` training notebook!

