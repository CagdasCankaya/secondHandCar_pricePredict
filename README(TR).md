# 2. El Araç Fiyatlarının Tahmini – Regresyon Problemi

Bu projede, ikinci el araçlara ait çeşitli özellikleri kullanarak araç fiyatlarını tahmin etmek amacıyla bir regresyon modeli geliştirilmiştir. Modelin eğitimi ve değerlendirmesi, TensorFlow ve Keras kullanılarak gerçekleştirilmiştir.

Sayısal giriş değişkenleri, Normalization katmanı ile normalize edilerek modelin daha hızlı ve stabil öğrenmesi sağlanmıştır. Ardından aşağıdaki yapıya sahip bir yapay sinir ağı (ANN) modeli kurulmuştur

# Kullanılan Teknolojiler
TensorFlow / Keras

Pandas

NumPy

Seaborn & Matplotlib (görselleştirme)

Scikit-learn (veri işleme)


# PROJE AKIŞI

-> Giriş Katmanı

-> 3 Adet Gizli Katman (her biri 128 nöron, ReLU aktivasyon fonksiyonu)

-> 1 Çıkış Katmanı (tahmini araç fiyatını verir)

Modelin çıktısı sürekli bir değerdir (TL cinsinden tahmin edilen fiyat). Kayıp fonksiyonu olarak Mean Absolute Error (MAE), metrik olarak ise Root Mean Squared Error (RMSE) kullanılmıştır. Eğitim süreci sırasında modelin kayıp değeri ve doğruluk metriği izlenmiştir.

Ayrıca TensorFlow’un tf.data veri pipeline sistemi kullanılarak veri daha verimli şekilde işlenmiş ve eğitim performansı artırılmıştır. Görselleştirme için matplotlib kullanılmıştır.

# PROJE AŞAMALARI

# 1 - Veri Hazırlama
Veri seti .csv dosyasından okunup temizlendi, sayısal sütunlar ayrıldı.

# 2 - Normalize Etme
TensorFlow Normalization katmanı ile sayısal veriler ölçeklendirildi.

# 3 - Model Kurulumu
Giriş → 3 Gizli Katman (ReLU) → Çıkış katmanı şeklinde ANN oluşturuldu.

# 4 - Model Eğitimi
Optimizasyon: Adam, Kayıp Fonksiyonu: MAE, Metri̇k: RMSE

# 5 - Değerlendirme ve Görselleştirme
Kayıp ve RMSE eğrileri çizildi. Tahminler ile gerçek değerler karşılaştırıldı.

# Dosya Yapısı
├── train.csv          # Araç verisi içeren veri seti
├── model.png          # Model mimarisi görseli
├── scripts/           # Eğitim ve analiz kodları
├── README.md          # Proje açıklaması
└── requirements.txt   # Gereken Python kütüphaneleri


# Geliştirme Önerileri
Daha karmaşık derin öğrenme yapıları denenebilir
Araç markası, lokasyon gibi kategorik veriler de modele eklenebilir
Model, transfer öğrenme veya ensemble yöntemlerle güçlendirilebilir

#  Proje Sahibi
Çağdaş ÇANKAYA

