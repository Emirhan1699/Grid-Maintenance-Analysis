# ⚡ Grid Maintenance and Outage Impact Analysis 
*🇹🇷 Türkçe versiyon için [aşağıya kaydırın](#türkçe-versiyon)*

This project was developed to analyze the impact of grid maintenance operations on power outages. The dashboard provides analytical insights into how maintenance activities influence both the frequency and duration of outages across different operational centers.

> **🔒 Data Privacy Notice:** Due to strict company confidentiality, all original datasets and the Power BI Template (`.pbit`) file have been permanently excluded. This repository showcases the project design, visual structures, and analytical insights exclusively through documentation and screenshots.

### 📊 Dashboard Views & Analytical Insights (Dashboard Görünümleri ve Bulgular)

**1. Overall Outage Frequency Impact (Genel Kesinti Sayısı Etkisi)**
<p align="center">
  <img src="Bakım Öncesi ve Sonrası Kesinti Sayısı Değişimi.png" width="85%" title="Genel Kesinti Sayısı" />
</p>
> 💡 *Key Insight:* Tracks the fluctuation in total outage incidents before and after interventions, highlighting how targeted maintenance operations help mitigate recurring faults and stabilize network performance.

**2. Overall Outage Duration Impact (Genel Kesinti Süresi Etkisi)**
<p align="center">
  <img src="Bakım Öncesi ve Sonrası Kesinti Süresi Değişimi.png" width="85%" title="Genel Kesinti Süresi" />
</p>
> 💡 *Key Insight:* Post-maintenance analysis reveals a consistent reduction in total outage durations across nearly all operational centers (mostly ranging between 25% and 45%). This proves the tangible positive impact of preventive maintenance on minimizing grid downtime.

**3. Outage Source Distribution (Kaynak Dağılımı)**
<p align="center">
  <img src="Kaynak Dağılımı.png" width="45%" title="Kaynak Dağılımı" />
</p>
> 💡 *Key Insight:* Demonstrates that the vast majority of recorded outages originate from Low Voltage (AG) lines (86.86%), while Medium Voltage (OG) accounts for 13.14%, providing a clear strategic roadmap for field team resource allocation.

**4. LV vs. MV Frequency Comparison (AG ve OG Kesinti Sayısı Karşılaştırması)**
<p align="center">
  <img src="Bakım Öncesi ve Sonrası Kesinti Sayısı Değişimi (AG).png" width="49%" title="AG (Alçak Gerilim) Görünümü" />
  <img src="Bakım Öncesi ve Sonrası Kesinti Sayısı Değişimi (OG).png" width="49%" title="Orta Gerilim) Görünümü" />
</p>
> 💡 *Key Insight:* Offers a granular comparative breakdown of maintenance efficiency separated by grid types (AG vs. MV), allowing managers to evaluate localized grid performance across different operational regions.

### 🎯 Key Metrics & Visualizations
The dashboard focuses on translating raw grid data into actionable business intelligence through the following key visuals:
*   **Impact on Outage Frequencies:** Tracks the percentage change in the number of outage incidents resulting from maintenance work.
*   **Impact on Outage Durations:** Analyzes the change in total outage durations before and after maintenance interventions.
*   **LV vs. MV Breakdown:** A proportional analysis showing the percentage distribution of outages across Low Voltage (AG) and Medium Voltage (OG) lines.

### 🛠️ Tools & Techniques
*   **Business Intelligence:** Power BI
*   **Data Modeling:** Star Schema, Power Query
*   **Languages:** DAX (Data Analysis Expressions)

---

<h2 id="türkçe-versiyon">⚡ Şebeke Bakım ve Kesinti Etki Analizi</h2>

Bu proje, şebeke bakım çalışmalarının güç kesintileri üzerindeki etkisini analiz etmek amacıyla geliştirilmiştir. Hazırlanan dashboard, bakım operasyonlarının farklı operasyon merkezlerindeki kesinti sıklığını ve süresini nasıl etkilediğine dair analitik içgörüler sunar.

> **🔒 Veri Gizliliği Notu:** Şirket gizlilik politikaları gereği, tüm orijinal veri setleri ve Power BI Şablon (`.pbit`) dosyası kapsam dışı bırakılmıştır. Bu depo, dokümantasyon ve ekran görüntüleri aracılığıyla proje tasarımını, görsel yapıları ve analitik içgörüleri sergilemektedir.

### 🎯 Öne Çıkan Metrikler ve Bulgular
Dashboard, ham şebeke verilerini eyleme dönüştürülebilir iş zekasına (BI) çevirmek için şu temel görsellere ve bulgulara odaklanır:

*   **Bakım Sonucu Sayı Değişimi:** Müdahaleler öncesi ve sonrası kesinti sıklıklarını takip ederek, tekrarlayan arızaların önlenmesindeki operasyonel başarıyı raporlar.
*   **Bakım Sonucu Süre Değişimi:** Bakım çalışmaları sonrasında neredeyse tüm operasyon merkezlerinde kesinti sürelerinde belirgin bir düşüş (%25 ila %45 arası) olduğu gözlemlenmiştir. Bu durum, planlı bakımın arıza sürelerini kısaltmadaki başarısını kanıtlar.
*   **AG ve OG Kesinti Dağılımı:** Kesintilerin oransal olarak büyük kısmının Alçak Gerilim (%86,86), daha küçük kısmının ise Orta Gerilim (%13,14) hatlarından kaynaklandığını göstererek saha ekiplerine stratejik yönelim sağlar.

### 🛠️ Kullanılan Araçlar ve Teknikler
*   **İş Zekası (BI):** Power BI
*   **Veri Modelleme:** Yıldız Şema (Star Schema), Power Query
*   **Diller:** DAX
