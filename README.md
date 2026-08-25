# ⚡ Grid Maintenance and Outage Impact Analysis

🇹🇷 [Türkçe versiyon için aşağıya kaydırın](#-şebeke-bakım-ve-kesinti-etki-analizi)

## 📌 Project Overview

Electrical grid reliability is critical for minimizing service disruptions and ensuring continuous energy delivery. This project was developed to evaluate the quantitative impact of scheduled grid maintenance operations on power outages across various regional operational centers.

By transforming raw enterprise grid outage and maintenance data into actionable business intelligence, the dashboard provides analytical visibility into how proactive maintenance interventions influence outage frequency, customer impact, and total outage duration.

### 🏗️ Project Architecture & Workflow

The end-to-end data workflow was designed to combine data preparation, transformation, modeling, analysis, and visualization:

1. **Data Preparation & Cleaning (Python & Excel):**  
   Raw outage and maintenance records were cleaned and structured using Python (`pandas`, `numpy`) and Excel. This included handling missing values, standardizing timestamps, and normalizing categorical fields.

2. **ETL & Transformation (Power Query):**  
   The prepared data was loaded into Power Query for additional transformations, conditional column creation, data standardization, and operational mapping.

3. **Data Modeling (Star Schema):**  
   A Star Schema architecture was developed by separating fact tables containing outage-related metrics from dimension tables containing operational attributes such as operational centers, voltage levels, and maintenance status.

4. **Analytics & DAX:**  
   DAX measures were developed to calculate pre- and post-maintenance metrics, percentage changes, and aggregated KPIs, enabling dynamic comparisons across different operational dimensions.

5. **Interactive Visualization (Power BI):**  
   Interactive Power BI dashboards were designed using KPI cards, trend visualizations, distribution charts, and synchronized filters for regional and voltage-level analysis.

### 🎯 Key Business Questions Addressed

- **What is the measurable impact of preventive maintenance?**  
  Evaluating whether scheduled maintenance interventions are associated with reductions in recurring outage frequency and total outage duration.

- **Where should field operations and resource allocation focus?**  
  Identifying operational centers and voltage levels associated with the highest levels of customer impact and outage activity.

- **How do Medium Voltage (MV) and Low Voltage (LV) incidents differ in scale?**  
  Comparing Medium Voltage feeder reliability with localized Low Voltage distribution issues.

> 🔒 **Data Privacy Notice:** Due to company confidentiality requirements, all original datasets and the Power BI Template (`.pbit`) file have been excluded from this repository. The project is presented through documentation, methodology, visual structures, and aggregated analytical insights without exposing confidential source data.

---

## 📊 Dashboard Views & Analytical Insights

### 1. Overall Outage Frequency Impact

<p align="center">
  <img src="outage_count_impact.png" width="85%" title="Overall Outage Frequency Impact" />
</p>

> 💡 **Key Insight:**  
> The analysis shows a measurable decrease in outage frequency following maintenance interventions, indicating an improvement in network reliability after scheduled maintenance activities.

<br><br>

### 2. Outage Source Distribution

<p align="center">
  <img src="source_distribution.png" width="45%" title="Outage Source Distribution" />
</p>

> 💡 **Key Insight:**  
> Medium Voltage (MV) lines account for **86.86%** of the analyzed outage distribution. This highlights the importance of prioritizing MV feeder maintenance and operational planning when addressing the largest share of outage activity.

<br><br>

### 3. Low Voltage (LV) Outage Frequency Analysis

<p align="center">
  <img src="lv_outage_analysis.png" width="85%" title="Low Voltage View" />
</p>

> 💡 **Key Insight:**  
> Provides granular visibility into Low Voltage network performance, allowing localized outage patterns and distribution-level issues to be examined across operational centers.

<br><br>

### 4. Medium Voltage (MV) Outage Frequency Analysis

<p align="center">
  <img src="mv_outage_analysis.png" width="85%" title="Medium Voltage View" />
</p>

> 💡 **Key Insight:**  
> Evaluates Medium Voltage feeder performance and highlights how maintenance activities on critical feeders can contribute to reducing outage frequency across the network.

<br><br>

### 5. Overall Affected Customers Impact

<p align="center">
  <img src="affected_customers_impact.png" width="85%" title="Overall Affected Customers Impact" />
</p>

> 💡 **Key Insight:**  
> The analysis shows a significant reduction in affected customers following maintenance activities across operational centers. Medium Voltage (MV) outages account for **97.11%** of the analyzed customer impact, while Low Voltage (LV) outages account for **2.89%**.

<br><br>

### 6. Low Voltage (LV) Affected Customers Analysis

<p align="center">
  <img src="lv_affected_customers.png" width="85%" title="Low Voltage Affected Customers" />
</p>

> 💡 **Key Insight:**  
> Examines localized customer impact within Low Voltage networks, which represent **2.89%** of the analyzed customer exposure, providing additional visibility into distribution-level issues.

<br><br>

### 7. Medium Voltage (MV) Affected Customers Analysis

<p align="center">
  <img src="mv_affected_customers.png" width="85%" title="Medium Voltage Affected Customers" />
</p>

> 💡 **Key Insight:**  
> Focuses on the Medium Voltage network, which represents **97.11%** of the analyzed affected-customer impact. Highlighting that Medium Voltage (MV) maintenance has the greatest impact on customer exposure and reduces the potential customer impact of widespread outages.

<br><br>

### 8. Overall Outage Duration Impact

<p align="center">
  <img src="outage_duration_impact.png" width="85%" title="Overall Outage Duration Impact" />
</p>

> 💡 **Key Insight:**  
> The analysis indicates a consistent **25% to 45% reduction in total outage duration** across the analyzed operational centers following maintenance activities.

---

## 🏁 Conclusion & Key Takeaways

This end-to-end analytical solution demonstrates how raw grid maintenance and outage data can be transformed into actionable insights for operational decision-making.

Key findings include:

- **Maintenance Impact:**  
  Scheduled maintenance activities were associated with reductions in outage frequency and total outage duration, with analyzed operational centers showing **25% to 45% reductions in total outage duration**.

- **Strategic Resource Allocation:**  
  Medium Voltage (MV) infrastructure accounts for **86.86% of outage activity** and **97.11% of analyzed affected-customer impact**, highlighting MV infrastructure as a key area for operational attention.

- **Improved Network Reliability:**  
  Comparing pre- and post-maintenance performance provides a data-driven approach for evaluating maintenance effectiveness and identifying areas requiring further operational attention.

> **Note:** The analysis measures the observed relationship between maintenance activities and outage metrics within the available dataset. It should not be interpreted as a direct causal or financial ROI calculation without additional cost and investment data.

---

## 🛠️ Tools & Techniques

- **Business Intelligence:** Power BI, DAX, Interactive Slicers, Custom Tooltips
- **Data Engineering & ETL:** Python (`pandas`, `numpy`), Excel, Power Query
- **Data Modeling:** Star Schema Architecture (Fact & Dimension Tables)
- **Programming & Analytics:** Python, DAX (Data Analysis Expressions)

---

# ⚡ Şebeke Bakım ve Kesinti Etki Analizi

## 📌 Proje Özeti

Elektrik şebekesi güvenilirliği, enerji kesintilerinin en aza indirilmesi ve kesintisiz enerji arzının sağlanması açısından büyük önem taşır. Bu proje, planlı şebeke bakım operasyonlarının farklı bölgesel operasyon merkezlerindeki kesinti performansı üzerindeki ölçülebilir etkisini değerlendirmek amacıyla geliştirilmiştir.

Ham şebeke kesinti ve bakım verileri iş zekasına dönüştürülerek; bakım müdahalelerinin kesinti sıklığı, etkilenen müşteri sayısı ve toplam kesinti süresi üzerindeki etkisi analiz edilmiştir.

### 🏗️ Proje Mimarisi ve İş Akışı

Projenin uçtan uca veri işleme süreci; veri hazırlama, dönüştürme, modelleme, analiz ve görselleştirme aşamalarından oluşturulmuştur:

1. **Veri Hazırlama ve Temizleme (Python & Excel):**  
   Ham kesinti ve bakım kayıtları Python (`pandas`, `numpy`) ve Excel kullanılarak temizlenmiş ve yapılandırılmıştır. Eksik verilerin işlenmesi, zaman bilgilerinin standardize edilmesi ve kategorik alanların düzenlenmesi bu aşamada gerçekleştirilmiştir.

2. **ETL ve Dönüştürme (Power Query):**  
   Hazırlanan veriler Power Query'ye aktarılmış; veri dönüşümleri, koşullu sütun oluşturma, standardizasyon ve operasyonel eşleştirmeler gerçekleştirilmiştir.

3. **Veri Modelleme (Yıldız Şema - Star Schema):**  
   Kesinti metriklerini içeren olgu tabloları ile operasyon merkezleri, gerilim seviyeleri ve bakım durumu gibi operasyonel bilgileri içeren boyut tablolarından oluşan Yıldız Şema mimarisi kurulmuştur.

4. **Analitik ve DAX:**  
   Bakım öncesi ve sonrası metrikleri, yüzde değişimleri ve toplulaştırılmış KPI'ları hesaplamak için DAX ölçüleri geliştirilmiştir.

5. **İnteraktif Görselleştirme (Power BI):**  
   KPI kartları, trend görselleri, dağılım grafikler ve senkronize filtreler kullanılarak interaktif Power BI dashboard'ları oluşturulmuştur.

### 🎯 Çözülen Temel İş Soruları

- **Koruyucu bakımların ölçülebilir etkisi nedir?**  
  Planlı bakım müdahalelerinin kesinti sıklığı ve toplam kesinti süresi üzerindeki etkisi değerlendirilmiştir.

- **Saha operasyonları ve kaynak tahsisi nereye odaklanmalıdır?**  
  En yüksek kesinti aktivitesine ve müşteri etkisine sahip operasyon merkezleri ve gerilim seviyeleri belirlenmiştir.

- **Orta Gerilim (OG) ve Alçak Gerilim (AG) olayları ölçek olarak nasıl ayrışır?**  
  Orta Gerilim fider güvenilirliği ile daha lokal Alçak Gerilim dağıtım problemleri karşılaştırılmıştır.

> 🔒 **Veri Gizliliği Notu:** Şirket gizlilik gereklilikleri nedeniyle orijinal veri setleri ve Power BI Şablon (`.pbit`) dosyası bu depoya dahil edilmemiştir. Proje; gizli kaynak verileri paylaşmadan dokümantasyon, metodoloji, görsel yapılar ve toplulaştırılmış analitik bulgular üzerinden sunulmaktadır.

---

## 📊 Dashboard Görünümleri ve Bulgular

### 1. Genel Kesinti Sayısı Etkisi

<p align="center">
  <img src="outage_count_impact.png" width="85%" title="Overall Outage Frequency Impact" />
</p>

> 💡 **Analitik Bulgu:**  
> Bakım müdahaleleri sonrasında kesinti sıklığında ölçülebilir bir düşüş gözlemlenmiştir. Bu durum, planlı bakım faaliyetleri sonrasında şebeke güvenilirliğinde iyileşme olduğunu göstermektedir.

<br><br>

### 2. Kesinti Kaynaklarının Dağılımı

<p align="center">
  <img src="source_distribution.png" width="45%" title="Outage Source Distribution" />
</p>

> 💡 **Analitik Bulgu:**  
> Analiz edilen kesintilerin **%86,86'sı Orta Gerilim (OG)** seviyesindeki hatlarla ilişkilidir. Bu sonuç, kesinti aktivitesinin büyük bölümünü oluşturan OG fiderlerinin bakım ve operasyon planlamasında önemli bir yere sahip olduğunu göstermektedir.

<br><br>

### 3. Alçak Gerilim (AG) Kesinti Analizi

<p align="center">
  <img src="lv_outage_analysis.png" width="85%" title="Low Voltage View" />
</p>

> 💡 **Analitik Bulgu:**  
> Alçak Gerilim şebeke performansına daha ayrıntılı bir bakış sağlayarak, operasyon merkezleri arasındaki yerel kesinti örüntülerinin ve dağıtım seviyesindeki problemlerin incelenmesine olanak tanır.

<br><br>

### 4. Orta Gerilim (OG) Kesinti Analizi

<p align="center">
  <img src="mv_outage_analysis.png" width="85%" title="Medium Voltage View" />
</p>

> 💡 **Analitik Bulgu:**  
> Orta Gerilim fiderlerinin performansını değerlendirerek, kritik fiderlerde gerçekleştirilen bakım faaliyetlerinin kesinti sıklığının azaltılmasına nasıl katkı sağlayabileceğini ortaya koyar.

<br><br>

### 5. Genel Etkilenen Müşteri Sayısı Etkisi

<p align="center">
  <img src="affected_customers_impact.png" width="85%" title="Overall Affected Customers Impact" />
</p>

> 💡 **Analitik Bulgu:**  
> Bakım faaliyetleri sonrasında operasyon merkezlerinde etkilenen müşteri sayısında belirgin bir düşüş gözlemlenmiştir. Analiz edilen müşteri etkisinin **%97,11'i Orta Gerilim (OG)**, **%2,89'u ise Alçak Gerilim (AG)** kesintileriyle ilişkilidir.

<br><br>

### 6. Alçak Gerilim (AG) Etkilenen Müşteri Analizi

<p align="center">
  <img src="lv_affected_customers.png" width="85%" title="Low Voltage Affected Customers" />
</p>

> 💡 **Analitik Bulgu:**  
> Analiz edilen toplam müşteri etkisinin **%2,89'unu** oluşturan Alçak Gerilim şebekesindeki lokal müşteri etkilerini inceler ve dağıtım seviyesindeki problemlere daha ayrıntılı bir bakış sağlar.

<br><br>

### 7. Orta Gerilim (OG) Etkilenen Müşteri Analizi

<p align="center">
  <img src="mv_affected_customers.png" width="85%" title="Medium Voltage Affected Customers" />
</p>

> 💡 **Analitik Bulgu:**  
> Analiz edilen etkilenen müşteri etkisinin **%97,11'ini** oluşturan Orta Gerilim şebekesine odaklanarak, OG fiderlerinin bakım ve operasyon planlamasındaki önemini ortaya koyar.

<br><br>

### 8. Genel Kesinti Süresi Etkisi

<p align="center">
  <img src="outage_duration_impact.png" width="85%" title="Overall Outage Duration Impact" />
</p>

> 💡 **Analitik Bulgu:**  
> Analiz edilen operasyon merkezlerinde bakım faaliyetleri sonrasında toplam kesinti sürelerinde **%25 ila %45 arasında azalma** gözlemlenmiştir.

---

## 🏁 Sonuç ve Değerlendirme

Bu uçtan uca analitik çözüm, ham şebeke bakım ve kesinti verilerinin operasyonel karar alma süreçlerinde kullanılabilecek anlamlı içgörülere dönüştürülebileceğini göstermektedir.

Projeden elde edilen temel çıkarımlar:

- **Bakım Etkisi:**  
  Planlı bakım faaliyetleri sonrasında kesinti sıklığı ve toplam kesinti süresinde azalma gözlemlenmiştir. Analiz edilen operasyon merkezlerinde toplam kesinti süresinde **%25 ila %45 arasında azalma** görülmüştür.

- **Stratejik Kaynak Tahsisi:**  
  Orta Gerilim (OG) altyapısı, analiz edilen kesinti aktivitesinin **%86,86'sını** ve etkilenen müşteri etkisinin **%97,11'ini** oluşturmaktadır. Bu sonuç, OG altyapısının operasyonel planlamada öncelikli alanlardan biri olduğunu göstermektedir.

- **Şebeke Güvenilirliği:**  
  Bakım öncesi ve sonrası performansın karşılaştırılması, bakım faaliyetlerinin etkinliğinin veri odaklı şekilde değerlendirilmesine ve iyileştirme gerektiren alanların belirlenmesine olanak sağlamaktadır.

> **Not:** Bu analiz, mevcut veri setindeki bakım faaliyetleri ile kesinti metrikleri arasındaki gözlemlenen ilişkiyi değerlendirir. Ek maliyet, yatırım ve kaynak verileri olmadan doğrudan nedensel bir etki veya finansal ROI hesaplaması olarak yorumlanmamalıdır.

---

## 🛠️ Tools & Techniques

- **Business Intelligence:** Power BI, DAX, Interactive Slicers, Custom Tooltips
- **Data Engineering & ETL:** Python (`pandas`, `numpy`), Excel, Power Query
- **Data Modeling:** Star Schema Architecture (Fact & Dimension Tables)
- **Programming & Analytics:** Python, DAX (Data Analysis Expressions)
