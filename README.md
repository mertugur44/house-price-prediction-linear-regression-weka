# Lineer Regresyon ile Konut Fiyat Tahmini

Bu proje kapsamında **Lineer Regresyon algoritmasının çalışma mantığı, kullanım alanları ve model değerlendirme süreci** incelenmiş; öğrenilen yöntemler **King County House Sales** veri seti üzerinde konut fiyat tahmini problemiyle uygulamalı olarak test edilmiştir.

Çalışma, veri analizi ve modelleme sürecinde **CRISP-DM** metodolojisi izlenerek **Weka 3.8.6** üzerinde gerçekleştirilmiştir.

## Projenin Amacı

Projenin temel amacı:

- Lineer Regresyon algoritmasının ne olduğunu ve nasıl çalıştığını öğrenmek,
- algoritmanın farklı kullanım alanlarını incelemek,
- veri hazırlama ve modelleme adımlarını uygulamak,
- modeli gerçek bir veri seti üzerinde test etmek,
- farklı doğrulama yöntemleriyle model performansını değerlendirmektir.

## Veri Seti

- 21.613 konut satış kaydı
- 19 özellik
- Veri kaynağı: King County House Sales
- Eksik değer bulunmamaktadır

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

## Bulgular ve Model Sonuçları

Keşifçi veri analizi sonucunda, konutun yaşam alanı büyüklüğü (`sqft_living`) ile satış fiyatı (`price`) arasında **güçlü ve pozitif doğrusal bir ilişki** gözlemlenmiştir.

Bu bulgu, genel olarak yaşam alanı büyüdükçe konut satış fiyatının da artma eğiliminde olduğunu göstermektedir.

### 10-Fold Cross-Validation

- Korelasyon Katsayısı (R): **0,8356**
- MAE: **0,0165**
- RMSE: **0,0264**

### %80 Eğitim / %20 Test

- Korelasyon Katsayısı (R): **0,8317**
- MAE: **0,0169**
- RMSE: **0,0282**

10-Fold Cross-Validation yöntemi, Holdout yöntemine göre daha yüksek korelasyon katsayısı ve daha düşük hata değerleri sağlamıştır.

Elde edilen sonuçlar, Lineer Regresyon modelinin gerçek konut fiyatları ile güçlü ilişki gösteren tahminler üretebildiğini ve farklı doğrulama yöntemlerinde benzer performans sergilediğini göstermektedir.

> `0,8356` değeri doğruluk oranı değil, model tahminleri ile gerçek değerler arasındaki korelasyon katsayısıdır.

## Kullanılan Teknolojiler ve Yaklaşımlar

- Weka 3.8.6
- Machine Learning
- Linear Regression
- CRISP-DM
- Exploratory Data Analysis (EDA)
- Data Preprocessing
- Feature Selection
- Normalization
- Cross-Validation
- Model Evaluation

## Proje Raporu

📄 [Proje Raporunu Görüntüle](./HOUSE_PRICE_LINEAR_REGRESSION_FINAL_REPORT.pdf)

Projeye ait teorik araştırma, metodoloji, veri analizi, görseller ve model sonuçları yukarıdaki proje raporunda yer almaktadır.

> Proje Weka 3.8.6 arayüzü üzerinden gerçekleştirildiği için ayrı bir kaynak kod dosyası bulunmamaktadır.

## Geliştirenler

- Mert Uğur
- Tolga Uslu
