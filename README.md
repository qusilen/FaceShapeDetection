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

- Face Shape Dataset (5 farklı yüz şekli sınıfı)  
- Eğitim ve doğrulama için ayrı klasör yapısı  
- Görseller 128x128 boyutuna ölçeklendirildi
- Kullanılan veri seti linkler bölümüne eklenmiştir.

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

## 📊 Sonuçlar ve Yorum

Yaptığım deneylerde, sıfırdan oluşturduğum CNN modeli temel doğruluk seviyelerine ulaştı ve bana CNN’in çalışma mantığını daha iyi anlama fırsatı verdi. Transfer learning (EfficientNetB0) denemelerinde ise, beklediğim gibi yüksek doğruluklar elde edemedim; doğruluk oranları custom CNN modeline göre daha düşük kaldı. Bunun nedeni, modelin veri setine tam olarak uyum sağlayamaması veya fine-tuning stratejisinin yeterince optimize edilmemesi olabilir.

Sonuç olarak, kendi CNN mimarimi kurmak öğrenme açısından çok değerli oldu ve tatmin edici doğruluklara ulaştım. Transfer learning kısmında ise şimdilik başarı sınırlı olsa da, ilerleyen süreçte farklı transfer learning modelleri (ResNet, MobileNet vb.) ve fine-tuning yöntemleri deneyerek performansı artırmayı hedefliyorum.
---

## 🔮 Gelecek Çalışmalar

İlerleyen süreçte aşağıdaki geliştirmeleri hayata geçirmek istiyorum:  

- 🤖 **Farklı derin öğrenme modelleri:** Diğer transfer learning modelleri (ResNet, MobileNet vb.) ile denemeler yapmak.
- 🎨 **Arayüz geliştirme:** Kullanıcı dostu bir arayüzle önerilerin interaktif şekilde sunulması. 
- 📱 **Mobil uygulama entegrasyonu:** Eğitilen modeli bir mobil uygulamaya gömerek, kameradan gelen görüntülerle **yüz şekli tespiti** yapılmasını sağlamak.  
- 💇‍♀️ **Kişiselleştirilmiş öneriler:** Kullanıcının yüz tipine göre saç modeli, gözlük seçimi gibi öneriler sunmak.  
- 🌐 **Gerçek zamanlı tahmin:** Dinamik ve gerçek zamanlı veri akışıyla yüz şeklinin anlık olarak belirlenmesi.     

Bu çalışmalar projeyi sadece bir öğrenme denemesi olmaktan çıkarıp, günlük hayatta faydalı bir uygulamaya dönüştürebilir.  

---

## 🔗 Linkler

[- Proje notebook linki](https://www.kaggle.com/code/qusilen/faceshapedetection)

[- Projede kullanılan veri seti](https://www.kaggle.com/datasets/niten19/face-shape-dataset)

