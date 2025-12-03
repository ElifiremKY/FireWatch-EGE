# FireWatch-EGE: Bölgesel Yangın Erken Tespit ve Risk Yönetim Sistemi

FireWatch-EGE, Ege Bölgesi için uydu + meteoroloji + topografya verilerini birleştirerek
**yangın erken tespit**, **risk analizi** ve **kestirimci yangın yayılımı tahmini** yapan bir sistemdir.

---

## 🎯 Projenin Amacı
- NASA FIRMS yangın noktalarını kullanarak sıcak noktaları tespit etmek  
- OpenWeatherMap ile rüzgâr, nem, sıcaklık gibi meteorolojik verileri eşleştirmek  
- DEM/SLOPE verileriyle bölgenin eğim etkisini hesaplamak  
- Birleşik risk skorunu çıkararak yüksek riskli bölgeleri belirlemek  
- Folium tabanlı etkileşimli risk haritası üretmek  

---

## 🛰 Kullanılan Veri Kaynakları
- **NASA FIRMS** – uydu tabanlı yangın verisi  
- **OpenWeatherMap API** – meteorolojik parametreler  
- **DEM / Slope** – arazi eğim modeli  
- **Geopy / Haversine** – bölgesel konum filtreleme  

---

## 🧠 Teknolojiler
- **Python**  
- **Apache Spark** (büyük veri işleme)  
- **MongoDB** (veri depolama)  
- **Scikit-learn** (Random Forest model)  
- **Folium** (ısı haritası ve risk haritaları)  

---

## 🛠 Metodoloji – 6 Aşamalı Geliştirme Süreci
1. **Veri Toplama:** FIRMS, OWM ve DEM kaynaklarından veri çekildi  
2. **Veri Depolama & Füzyon:** MongoDB ve Spark üzerinde birleştirme  
3. **Risk Hesaplama:**  
   R = f(sıcaklık, rüzgar, nem, eğim, konum ilişkisi)  
4. **ML Modeli:** Random Forest ile risk sınıflandırma  
5. **Web Arayüzü:** Folium ile etkileşimli harita prototipi  
6. **Test:** Gerçek yangın geçmişi ile karşılaştırma  

---

## 📌 Proje Çıktıları
- Anlık risk haritası  
- Kestirimci risk haritası  
- Bölgeler arası risk karşılaştırma  
- Kullanıcı dostu harita arayüzü  
- Raporlama modülü  

---

## 📂 Repo Yapısı (Yüklemeye Hazır)
