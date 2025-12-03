# FireWatch-EGE: Bölgesel Yangın Erken Tespit ve Risk Yönetim Sistemi

FireWatch-EGE, Ege Bölgesi için uydu + meteoroloji + topografya verilerini birleştirerek
**yangın erken tespiti**, **risk analizi** ve **kestirimci yangın yayılımı tahmini** yapan bir veri işleme ve analiz sistemidir.

---

## 🎯 Projenin Amacı
- NASA FIRMS sıcak nokta verileriyle **yangın başlangıçlarını tespit etmek**
- OpenWeatherMap API verileriyle **rüzgâr, nem, sıcaklık** gibi faktörleri birleştirmek
- DEM/Slope verileri ile **arazi eğim etkisini** modele dahil etmek
- Farklı veri kaynaklarını birleştirip **risk skorunu** hesaplamak
- Folium tabanlı etkileşimli bir arayüz ile **risk haritası** oluşturmak

---

## 🛰 Kullanılan Veri Kaynakları
- **NASA FIRMS** – Uydu tabanlı yangın / sıcak nokta verisi  
- **OpenWeatherMap API** – Meteorolojik parametreler  
- **DEM (Digital Elevation Model)** – Yüzey yüksekliği ve eğim verisi  
- **Geopy / Haversine** – Coğrafi uzaklık hesaplama  

---

## 🧠 Teknolojiler
- **Python**  
- **Apache Spark** (ölçeklenebilir veri işleme)
- **MongoDB** (ham ve işlenmiş verilerin depolanması)
- **Scikit-learn** (Random Forest risk modeli)
- **Folium** (etkileşimli yangın ve risk haritaları)
- **Pandas, NumPy, Requests** (veri işleme + API entegrasyonu)

---

## 🛠 Proje Metodolojisi – 6 Aşamalı Geliştirme Süreci

### 1) Veri Toplama  
NASA FIRMS, OpenWeatherMap ve DEM kaynaklarından veriler çekilir.

### 2) Veri Depolama ve Füzyon  
Veriler MongoDB’de tutulur ve Spark ile eş zamanlı birleştirilir.

### 3) Risk Skoru Hesaplama  
Sıcaklık, nem, rüzgâr hızı, eğim ve konum ilişkisi kullanılarak bir **R skoru** üretilir.

### 4) Makine Öğrenmesi  
Random Forest modeli ile geçmiş veriler üzerinden **yangın riski sınıflandırması** yapılır.

### 5) Harita Arayüzü  
Folium ile **bölgesel risk haritası**, sıcak nokta haritası ve yayılım tahmin haritası oluşturulur.

### 6) Test ve Doğrulama  
Modelin çıktıları gerçek geçmiş yangınlarla karşılaştırılarak doğruluk kontrolü yapılır.

---

## 📌 Üretilen Çıktılar
- **Anlık risk haritası**
- **Kestirimci risk haritası**
- **Eğim + hava durumu + sıcak nokta ilişkili bölgesel analiz**
- **Web tabanlı interaktif prototip**

---

## 📂 Önerilen Klasör Yapısı
(İleride ekleyeceğin .ipynb ve .py dosyaları için hazırdır.)
