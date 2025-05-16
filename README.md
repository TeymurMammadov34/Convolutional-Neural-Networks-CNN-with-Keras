# Evrişimli Sinir Ağı (CNN) ile Görüntü Sınıflandırma

Bu projede, **Keras** kullanarak **Evrişimli Sinir Ağı (CNN)** modeli ile **CIFAR-10** veri seti üzerinde görüntü sınıflandırması yapılmıştır. CNN, derin öğrenme modelleri arasında özellikle görüntü işleme alanında etkili bir yöntemdir.

## Proje Hedefi

Bu projede amacımız:
- **CIFAR-10** veri setini kullanarak, her biri farklı bir kategoriye ait 60,000 renkli görüntüyü doğru bir şekilde sınıflandırmak.
- Keras kütüphanesini kullanarak CNN modeli inşa etmek ve eğitmek.
- Modelin doğruluk oranını artırmak için **data augmentation** (veri artırma) tekniklerini kullanmak.

## Kullanılan Teknolojiler

- **Python 3.x**
- **Keras**: Derin öğrenme için yüksek seviyeli API.
- **TensorFlow**: Keras backend olarak TensorFlow kullanıldı.
- **NumPy**: Matematiksel hesaplamalar için.
- **Matplotlib**: Görselleştirme için.
- **scikit-learn**: Model değerlendirmesi için `classification_report` fonksiyonu kullanıldı.

## Veri Seti

- **CIFAR-10** veri seti, 10 farklı sınıfa ait toplamda 60,000 renkli 32x32 boyutlarında görüntü içerir.
- Sınıflar: "Airplane", "Automobile", "Bird", "Cat", "Deer", "Dog", "Frog", "Horse", "Ship", "Truck".

## Model Mimarisi

- **Conv2D** katmanları ile görüntüler üzerinde evrişimsel işlem yaparak özellik çıkarımı.
- **MaxPooling2D** ile özellik haritalarının boyutları küçültülür.
- **Dropout** ile aşırı öğrenme (overfitting) önlenir.
- Son olarak, **Flatten** ve **Dense** katmanları ile sınıflandırma yapılır.

## Eğitim Süreci

- Model, 20 epoch boyunca eğitildi ve eğitim sırasında doğrulama verileriyle test edilmiştir.
- **RMSprop** optimizasyon algoritması kullanılmıştır.
- Eğitim verisi üzerinde **data augmentation** uygulanmıştır (dönme, kaydırma, zoom).

## Sonuçlar

- Modelin doğruluğu ve kaybı her epoch için görselleştirildi.
- Sınıflandırma raporu (`classification_report`) ile modelin her sınıf için doğruluk oranları ve diğer metrikler değerlendirildi.

## Çalıştırma Talimatları

1. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install tensorflow numpy matplotlib scikit-learn



## 👨‍💻 Geliştirici

**Teymur Mammadov** 
