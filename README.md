# Lineer Regresyon ile Konut Fiyat Tahmini

Bu projede, **King County House Sales** veri seti kullanılarak konut satış fiyatlarının Lineer Regresyon yöntemiyle tahmin edilmesi amaçlanmıştır.

Çalışma, veri analizi ve modelleme sürecinde **CRISP-DM** metodolojisi izlenerek **Weka 3.8.6** üzerinde gerçekleştirilmiştir.

## Veri Seti

- 21.613 konut satış kaydı
- 19 özellik
- Veri kaynağı: King County House Sales
- Eksik değer bulunmamaktadır.

Modelleme öncesinde `id` ve `date` alanları veri setinden çıkarılmış, sayısal veriler `[0,1]` aralığına normalize edilmiştir.

## Kullanılan Yöntemler

- Lineer Regresyon
- Keşifçi Veri Analizi (EDA)
- Veri Ön İşleme
- Özellik Seçimi
- Normalizasyon
- %80 Eğitim / %20 Test Holdout
- 10-Fold Cross-Validation
- Model Performans Değerlendirmesi

## Model Sonuçları

### 10-Fold Cross-Validation

- Korelasyon Katsayısı (R): **0,8356**
- MAE: **0,0165**
- RMSE: **0,0264**

### %80 Eğitim / %20 Test

- Korelasyon Katsayısı (R): **0,8317**
- MAE: **0,0169**
- RMSE: **0,0282**

10-Fold Cross-Validation yöntemi, Holdout yöntemine göre daha yüksek korelasyon ve daha düşük hata değerleri sağlamıştır.

## Kullanılan Teknolojiler

- Weka 3.8.6
- Machine Learning
- Linear Regression
- CRISP-DM
- Exploratory Data Analysis (EDA)
- Cross-Validation
- Model Evaluation

## Proje Raporu

Projeye ait ayrıntılı analiz, metodoloji, görseller ve sonuçlar repository içerisinde bulunan proje raporunda yer almaktadır.

> Proje Weka 3.8.6 arayüzü üzerinden gerçekleştirildiği için ayrı bir kaynak kod dosyası bulunmamaktadır.

## Geliştirenler

- Mert Uğur
- Tolga Uslu
