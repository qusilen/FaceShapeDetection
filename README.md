# 📌 Face Shape Classification with CNN

Bu proje, yüz şekillerini sınıflandırmak için **sıfırdan tasarlanmış Convolutional Neural Network (CNN)** mimarisi ve **transfer learning tabanlı yaklaşımlar** (EfficientNet) kullanılarak geliştirilmiştir. Amaç, farklı modelleme tekniklerini karşılaştırarak en yüksek doğruluğa ulaşmaktır.

---

## 🚀 Özellikler
- TensorFlow/Keras tabanlı model geliştirme  
- CNN katmanları **manuel olarak inşa edildi**  
- **Transfer Learning** (EfficientNet) ile denemeler  
- **Veri artırma (ImageDataGenerator)** ile çeşitlilik sağlandı  
- **EarlyStopping** ve **ReduceLROnPlateau** callback’leri ile optimize eğitim süreci  
- Eğitim sonunda doğruluk ve kayıp metriklerinin görselleştirilmesi  

---

## 📂 Veri Seti
- Face Shape Dataset (ör: 5 farklı yüz şekli sınıfı)  
- Eğitim ve doğrulama için ayrı klasör yapısı  
- Görseller 128x128 boyutuna ölçeklendirildi  

---

## 🧠 Model Mimarisi
### Custom CNN
- Conv2D + MaxPooling katmanları  
- Flatten + Dense katmanları  
- Dropout ile regularization  

### Transfer Learning
- EfficientNetB0 (ImageNet ön-eğitimli)  
- GlobalAveragePooling katmanı  
- Dense sınıflandırıcı katman  

---

## 📊 Sonuçlar
- CNN ve Transfer Learning performansları karşılaştırıldı  
- Eğitim & doğrulama doğruluğu ve kaybı grafiklerle analiz edildi  

---

## 🔮 Gelecek Çalışmalar
- Daha derin CNN mimarileriyle deneyler  
- Farklı transfer learning modellerinin test edilmesi  
- Daha geniş veri setleriyle model genellemesinin iyileştirilmesi  

---

## ⚙️ Kurulum
```bash
# Gerekli kütüphaneleri yükle
pip install tensorflow matplotlib
