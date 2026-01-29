# ECS-VB-1125
Titanic: Machine Learning from Disaster
Bu proje, Kaggle üzerinde yer alan Titanic veri kümesini kullanarak yolcuların hayatta kalma durumlarını tahmin eden bir makine öğrenmesi çalışmasıdır.

Proje Amacı
Titanic kazasındaki yolcu verilerini (ad, yaş, cinsiyet, sosyo-ekonomik durum vb.) analiz ederek, hangi özelliklerin kişilerin hayatta kalma ihtimalini artırdığını belirlemek ve bu verilerle bir tahmin modeli oluşturmaktır.

Kullanılan Teknolojiler
Python

Pandas (Veri işleme ve analiz)

Scikit-learn (Makine öğrenmesi modelleri ve değerlendirme)

Kodun Çalışma Mantığı
Notebook içerisindeki akış şu adımları izlemektedir:

Veri Yükleme: Pandas kütüphanesi ile eğitim ve test veri setleri projeye dahil edilmiştir.

Özellik Seçimi: Modelin tahmin gücünü artırmak amacıyla yolcu sınıfı (Pclass), cinsiyet (Sex), kardeş/eş sayısı (SibSp) ve ebeveyn/çocuk sayısı (Parch) değişkenleri seçilmiştir.

Veri Ön İşleme: Kategorik bir değişken olan cinsiyet verisi, makine öğrenmesi modelinin işleyebilmesi için get_dummies yöntemiyle sayısal formatta vektörleştirilmiştir.

Model Eğitimi: Tahminleme işlemi için RandomForestClassifier algoritması kullanılmıştır. Model, 100 karar ağacı ve maksimum 5 derinlik parametreleri ile yapılandırılmıştır.

Tahmin ve Çıktı: Eğitilen model test verileri üzerinde çalıştırılmış ve sonuçlar Kaggle formatına uygun olarak submission.csv dosyasına kaydedilmiştir.

Sonuç
Oluşturulan model ile test veri seti üzerinde tahminler yapılmış ve elde edilen sonuçlar yarışma platformuna yüklenmiştir.
