# ⚡ Grid Maintenance and Outage Impact Analysis

🇹🇷 [Türkçe versiyon için tıklayın](#-şebeke-bakım-ve-kesinti-etki-analizi)

## 📌 Project Overview

Electrical grid reliability is critical for minimizing service disruptions and ensuring continuous energy delivery. This project was developed to quantitatively evaluate the impact of scheduled grid maintenance operations on power outages across different regional operational centers.

By transforming large-scale outage and maintenance records into actionable business intelligence, the dashboard provides analytical visibility into how maintenance interventions are associated with changes in outage frequency, affected customers, and total outage duration.

### 🏗️ Project Architecture & Workflow

The end-to-end data workflow was designed to support reliable analysis and interactive reporting:

1. **Data Preparation & Cleaning (Python & Excel):**  
   Raw outage and maintenance records were cleaned and structured using Python (`pandas`, `numpy`) and Excel. The process included handling missing values, standardizing timestamps, and normalizing categorical fields across large-scale operational datasets.

2. **ETL & Transformation (Power Query):**  
   The prepared data was loaded into Power Query for data transformation, conditional column creation, data standardization, and mapping of operational hierarchies.

3. **Data Modeling (Star Schema):**  
   A **Star Schema** data model was developed by separating fact tables containing outage events, durations, and affected customer counts from dimension tables such as operational centers, voltage levels, and maintenance status.

4. **Advanced Analytics & DAX:**  
   DAX measures were developed to calculate pre- and post-maintenance values, absolute and percentage changes, and aggregated KPIs for dynamic comparisons.

5. **Interactive Visualization (Power BI):**  
   Interactive dashboards were designed using KPI cards, trend visualizations, distribution charts, custom tooltips, and synchronized filters to enable operational analysis across different regions and voltage levels.

### 🎯 Key Business Questions Addressed

* **What measurable changes are observed after maintenance interventions?**  
  Evaluating changes in outage frequency, affected customers, and total outage duration between pre- and post-maintenance periods.

* **Where should maintenance efforts be prioritized?**  
  Identifying operational centers and voltage levels with higher outage frequency and customer impact to support maintenance prioritization.

* **How do Medium Voltage (MV) and Low Voltage (LV) incidents differ in scale and impact?**  
  Comparing outage patterns, affected customers, and outage durations across different voltage levels.

### 📈 Measurable Impact

The analysis focuses on three primary measurable outcomes:

* **Outage Frequency:** Changes in the number of outage incidents following maintenance interventions.
* **Affected Customers:** Changes in the number of customers impacted by outages.
* **Outage Duration:** Changes in total outage duration across operational centers.

These metrics provide a quantitative basis for evaluating changes in network performance following maintenance activities.

### 🔧 Maintenance Impact

The dashboard provides operational insights that can support maintenance planning by:

* Highlighting operational centers with significant changes in outage performance.
* Identifying voltage levels associated with higher customer exposure.
* Comparing LV and MV outage patterns.
* Supporting the prioritization of maintenance activities based on observed outage and customer impact.
* Providing a centralized view of maintenance-related performance indicators.

> **🔒 Data Privacy Notice:** Due to company confidentiality requirements, all original datasets and the Power BI Template (`.pbit`) file have been excluded from this repository. The project is presented through documentation, dashboard screenshots, and aggregated analytical findings without exposing confidential source data.

---

## 📊 Dashboard Views & Analytical Insights

### 1. Overall Outage Frequency Impact

<p align="center">
  <img src="outage_count_impact.png" width="85%" title="Overall Outage Frequency Impact" />
</p>

> 💡 *Key Insight:* The analysis shows a measurable decrease in outage frequency following maintenance interventions across the analyzed operational centers, indicating improved outage performance during the post-maintenance period.

<br><br>

### 2. Outage Source Distribution

<p align="center">
  <img src="source_distribution.png" width="45%" title="Outage Source Distribution" />
</p>

> 💡 *Key Insight:* Medium Voltage (MV) lines account for **86.86%** of the analyzed outage distribution, highlighting MV infrastructure as a major area of focus for outage monitoring and maintenance prioritization.

<br><br>

### 3. Low Voltage (LV) Outage Frequency Analysis

<p align="center">
  <img src="lv_outage_analysis.png" width="85%" title="Low Voltage View" />
</p>

> 💡 *Key Insight:* Provides detailed visibility into Low Voltage network performance, enabling comparisons between operational centers and helping identify localized outage patterns and distribution-level bottlenecks.

<br><br>

### 4. Medium Voltage (MV) Outage Frequency Analysis

<p align="center">
  <img src="mv_outage_analysis.png" width="85%" title="Medium Voltage View" />
</p>

> 💡 *Key Insight:* Provides a detailed view of Medium Voltage outage behavior and enables comparison of maintenance-related changes across operational centers and critical feeder networks.

<br><br>

### 5. Overall Affected Customers Impact

<p align="center">
  <img src="affected_customers_impact.png" width="85%" title="Overall Affected Customers Impact" />
</p>

> 💡 *Key Insight:* The analysis shows a notable reduction in affected customers during the post-maintenance period. Medium Voltage (MV) outages account for **97.11%** of total affected customer exposure, compared with **2.89%** for Low Voltage (LV), emphasizing the larger customer-scale impact of MV incidents.

<br><br>

### 6. Low Voltage (LV) Affected Customers Analysis

<p align="center">
  <img src="lv_affected_customers.png" width="85%" title="Low Voltage Affected Customers" />
</p>

> 💡 *Key Insight:* Examines customer impact within Low Voltage networks, which represent **2.89%** of the total affected customer exposure, providing more granular visibility into localized distribution-level disruptions.

<br><br>

### 7. Medium Voltage (MV) Affected Customers Analysis

<p align="center">
  <img src="mv_affected_customers.png" width="85%" title="Medium Voltage Affected Customers" />
</p>

> 💡 *Key Insight:* Focuses on Medium Voltage networks, which account for **97.11%** of affected customer exposure in the analyzed data, highlighting the broader customer impact associated with MV outages.

<br><br>

### 8. Overall Outage Duration Impact

<p align="center">
  <img src="outage_duration_impact.png" width="85%" title="Overall Outage Duration Impact" />
</p>

> 💡 *Key Insight:* The analysis indicates a **25%–45% reduction in total outage duration** across the analyzed operational centers during the post-maintenance period, indicating a measurable improvement in outage duration performance.

---

## 🏁 Conclusion & Key Takeaways

This end-to-end analytical solution demonstrates how raw grid maintenance and outage data can be effectively transformed into actionable operational insights. 

Key takeaways include:
* **Measurable Performance Improvements:** Scheduled maintenance interventions are associated with consistent decreases in outage frequency and a **25%–45% reduction in total outage duration** across regional operational centers.
* **Targeted Resource Allocation:** Medium Voltage (MV) infrastructure drives the vast majority of both outage distribution (**86.86%**) and customer exposure (**97.11%**), providing a clear indication of where maintenance prioritization may have the greatest operational impact.
* **Data-Driven Evaluation:** Establishing a structured pre- and post-maintenance comparison framework enables organizations to objectively track network reliability and operational efficiency.

> **Note:** The analysis evaluates the observed relationship between scheduled maintenance activities and outage performance metrics within the available dataset. It focuses on operational impact rather than financial outcomes.

---

### 🎯 Key Metrics & Visualizations

The dashboard translates operational grid data into measurable performance indicators through the following key visualizations:

* **Outage Frequency Impact:** Measures changes in the number of outage incidents between pre- and post-maintenance periods.
* **LV & MV Breakdown:** Provides comparative analysis of outage performance across voltage levels.
* **Affected Customers Analysis:** Measures changes in customer exposure and highlights the **97.11% MV vs. 2.89% LV** distribution.
* **Outage Duration Impact:** Measures changes in total outage duration following maintenance interventions.
* **Operational Center Comparison:** Enables regional comparison of maintenance-related changes and outage performance.

### 🛠️ Tools & Techniques

* **Business Intelligence:** Power BI (DAX, Interactive Slicers, Custom Tooltips)
* **Data Engineering & ETL:** Python (`pandas`, `numpy`), Excel, Power Query
* **Data Modeling:** Star Schema Architecture (Fact & Dimension Tables)
* **Languages:** Python, DAX (Data Analysis Expressions)

---

<h2 id="türkçe-versiyon">⚡ Şebeke Bakım ve Kesinti Etki Analizi</h2>

## 📌 Proje Özeti

Elektrik şebekesi güvenilirliği, enerji kesintilerinin en aza indirilmesi ve kesintisiz enerji arzının sağlanması açısından kritik öneme sahiptir. Bu proje, planlı şebeke bakım operasyonlarının farklı bölgesel operasyon merkezlerindeki kesinti performansı üzerindeki etkisini kantitatif olarak değerlendirmek amacıyla geliştirilmiştir.

Büyük ölçekli arıza ve bakım kayıtları iş zekasına dönüştürülerek; bakım müdahaleleri sonrasında **kesinti sıklığı, etkilenen abone sayısı ve toplam kesinti süresinde gözlemlenen değişimlere** ilişkin analitik görünürlük sağlanmıştır.

### 🏗️ Proje Mimarisi ve İş Akışı

Projenin uçtan uca veri iş akışı, güvenilir analiz ve interaktif raporlama ihtiyaçları doğrultusunda tasarlanmıştır:

1. **Veri Hazırlama ve Temizleme (Python & Excel):** Ham kesinti ve bakım kayıtları Python (`pandas`, `numpy`) ve Excel kullanılarak temizlenmiş ve yapılandırılmıştır. Süreç kapsamında eksik verilerin işlenmesi, zaman bilgilerinin standardize edilmesi ve kategorik alanların normalleştirilmesi gerçekleştirilmiştir.

2. **ETL ve Dönüştürme (Power Query):** Hazırlanan veriler; veri dönüşümü, koşullu sütun oluşturma, veri standardizasyonu ve operasyonel hiyerarşilerin eşleştirilmesi amacıyla Power Query'ye aktarılmıştır.

3. **Veri Modelleme (Yıldız Şema - Star Schema):** Kesinti olayları, kesinti süreleri ve etkilenen abone sayılarını içeren olgu tabloları; operasyon merkezleri, gerilim seviyeleri ve bakım durumu gibi boyut tablolarından ayrıştırılarak **Yıldız Şema** veri modeli oluşturulmuştur.

4. **İleri Düzey Analitik ve DAX:** Bakım öncesi ve sonrası değerleri, mutlak ve yüzdesel değişimleri ve toplulaştırılmış KPI'ları hesaplamak için DAX ölçüleri geliştirilmiştir.

5. **İnteraktif Görselleştirme (Power BI):** KPI kartları, trend görselleri, dağılım grafikleri, özel araç ipuçları ve senkronize filtreler kullanılarak farklı bölgeler ve gerilim seviyeleri arasında karşılaştırmalı analiz yapılmasını sağlayan dashboard'lar tasarlanmıştır.

### 🎯 Çözülen Temel İş Soruları

* **Bakım müdahaleleri sonrasında hangi ölçülebilir değişimler gözlemleniyor?**  
  Bakım öncesi ve sonrası dönemler karşılaştırılarak kesinti sayısı, etkilenen abone sayısı ve toplam kesinti süresindeki değişimler değerlendirilmiştir.

* **Bakım çalışmalarında hangi alanlara öncelik verilmelidir?**  
  Daha yüksek kesinti sıklığına ve müşteri etkisine sahip operasyon merkezleri ve gerilim seviyeleri belirlenerek bakım önceliklendirmesine yönelik içgörüler sağlanmıştır.

* **Orta Gerilim (OG) ve Alçak Gerilim (AG) olayları ölçek ve etki açısından nasıl ayrışıyor?**  
  Farklı gerilim seviyelerindeki kesinti davranışları, etkilenen abone sayıları ve kesinti süreleri karşılaştırılmıştır.

### 📈 Measurable Impact — Ölçülebilir Etki

Analiz üç temel ölçülebilir sonuca odaklanmaktadır:

* **Kesinti Sıklığı:** Bakım müdahaleleri sonrasında kesinti olaylarının sayısındaki değişim.
* **Etkilenen Aboneler:** Kesintilerden etkilenen abone sayısındaki değişim.
* **Kesinti Süresi:** Operasyon merkezlerindeki toplam kesinti süresindeki değişim.

Bu göstergeler, bakım faaliyetleri sonrasında şebeke performansında gözlemlenen değişimlerin kantitatif olarak değerlendirilmesini sağlamaktadır.

### 🔧 Maintenance Impact — Bakım Etkisi

Dashboard, bakım planlama süreçlerini destekleyebilecek aşağıdaki operasyonel içgörüleri sunmaktadır:

* Kesinti performansında belirgin değişimler gösteren operasyon merkezlerinin belirlenmesi.
* Daha yüksek müşteri maruziyetine sahip gerilim seviyelerinin tespit edilmesi.
* AG ve OG kesinti davranışlarının karşılaştırılması.
* Gözlemlenen kesinti ve müşteri etkilerine göre bakım faaliyetlerinin önceliklendirilmesinin desteklenmesi.
* Bakım sonrası performans göstergelerinin merkezi bir dashboard üzerinden takip edilmesi.

> **🔒 Veri Gizliliği Notu:** Şirket gizlilik gereklilikleri nedeniyle tüm orijinal veri setleri ve Power BI Şablon (`.pbit`) dosyası bu depoya dahil edilmemiştir. Proje; gizli kaynak veriler paylaşılmadan dokümantasyon, dashboard ekran görüntüleri ve toplulaştırılmış analitik bulgular üzerinden sunulmaktadır.

---

## 📊 Dashboard Views & Analytical Insights

### 1. Genel Kesinti Sayısı Etkisi

<p align="center">
  <img src="outage_count_impact.png" width="85%" title="Genel Kesinti Sayısı" />
</p>

> 💡 *Analitik Bulgu:* Analiz edilen operasyon merkezlerinde bakım müdahaleleri sonrasında kesinti sıklığında ölçülebilir bir düşüş gözlemlenmiştir. Bu durum, bakım sonrası dönemde kesinti performansında iyileşme olduğunu göstermektedir.

<br><br>

### 2. Kesinti Kaynak Dağılımı

<p align="center">
  <img src="source_distribution.png" width="45%" title="Kesinti Kaynak Dağılımı" />
</p>

> 💡 *Analitik Bulgu:* Analiz edilen kesintilerin **%86,86'sının Orta Gerilim (OG)** hatlarıyla ilişkili olduğu görülmektedir. Bu sonuç, OG altyapısının kesinti izleme ve bakım önceliklendirmesinde önemli bir odak noktası olduğunu göstermektedir.

<br><br>

### 3. Alçak Gerilim (AG) Kesinti Analizi

<p align="center">
  <img src="lv_outage_analysis.png" width="85%" title="AG Görünümü" />
</p>

> 💡 *Analitik Bulgu:* Alçak Gerilim şebeke performansına ilişkin ayrıntılı görünürlük sağlayarak operasyon merkezleri arasındaki farklılıkların ve yerel dağıtım seviyesindeki kesinti modellerinin incelenmesine olanak tanımaktadır.

<br><br>

### 4. Orta Gerilim (OG) Kesinti Analizi

<p align="center">
  <img src="mv_outage_analysis.png" width="85%" title="OG Görünümü" />
</p>

> 💡 *Analitik Bulgu:* Orta Gerilim kesintilerinin operasyon merkezleri ve bakım dönemleri arasındaki değişimini inceleyerek kritik besleme hatlarının performansının karşılaştırılmasını sağlamaktadır.

<br><br>

### 5. Genel Etkilenen Abone Sayısı Etkisi

<p align="center">
  <img src="affected_customers_impact.png" width="85%" title="Genel Etkilenen Abone Sayısı" />
</p>

> 💡 *Analitik Bulgu:* Bakım sonrası dönemde etkilenen abone sayısında belirgin bir azalma gözlemlenmiştir. Analiz edilen verilerde etkilenen abonelerin **%97,11'i Orta Gerilim (OG)**, **%2,89'u ise Alçak Gerilim (AG)** kesintileriyle ilişkilidir. Bu dağılım, OG kesintilerinin müşteri ölçeğindeki etkisinin daha yüksek olduğunu göstermektedir.

<br><br>

### 6. Alçak Gerilim (AG) Etkilenen Abone Analizi

<p align="center">
  <img src="lv_affected_customers.png" width="85%" title="AG Etkilenen Aboneler" />
</p>

> 💡 *Analitik Bulgu:* Toplam etkilenen abone maruziyetinin **%2,89'unu** oluşturan Alçak Gerilim kesintilerinin yerel müşteri etkisini incelemekte ve dağıtım seviyesindeki farklılıkların daha ayrıntılı şekilde değerlendirilmesini sağlamaktadır.

<br><br>

### 7. Orta Gerilim (OG) Etkilenen Abone Analizi

<p align="center">
  <img src="mv_affected_customers.png" width="85%" title="OG Etkilenen Aboneler" />
</p>

> 💡 *Analitik Bulgu:* Etkilenen abone maruziyetinin **%97,11'ini** oluşturan Orta Gerilim kesintilerine odaklanarak OG altyapısındaki kesintilerin geniş müşteri grupları üzerindeki etkisini ortaya koymaktadır.

<br><br>

### 8. Genel Kesinti Süresi Etkisi

<p align="center">
  <img src="outage_duration_impact.png" width="85%" title="Genel Kesinti Süresi" />
</p>

> 💡 *Analitik Bulgu:* Analiz edilen operasyon merkezlerinde bakım sonrası dönemde toplam kesinti süresinde **%25–%45 arasında azalma** gözlemlenmiştir. Bu sonuç, bakım sonrası dönemde kesinti süresi performansında ölçülebilir bir iyileşmeye işaret etmektedir.

---

## 🏁 Sonuç ve Değerlendirme

Bu uçtan uca analitik çözüm, ham şebeke bakım ve kesinti verilerinin operasyonel karar alma süreçlerinde kullanılabilecek anlamlı içgörülere dönüştürülebileceğini somut bir şekilde ortaya koymaktadır.

Projeden elde edilen temel çıkarımlar:
* **Ölçülebilir Performans İyileşmesi:** Planlı bakım müdahalelerinin, kesinti sıklığında düşüş ve bölgesel operasyon merkezlerinde toplam kesinti süresinde **%25–%45 oranında azalma** ile ilişkili olduğu gözlemlenmiştir.
* **Hedef Odaklı Kaynak Tahsisi:** Orta Gerilim (OG) altyapısının, toplam kesinti aktivitesinin **%86,86'sını** ve etkilenen abone maruziyetinin **%97,11'ini** oluşturduğu tespit edilerek şebeke yatırımları ve bakım planlaması için net bir öncelik alanı tanımlanmıştır.
* **Veri Odaklı Değerlendirme:** Oluşturulan yapılandırılmış bakım öncesi ve sonrası analiz çerçevesi sayesinde, şebeke güvenilirliği objektif metriklerle takip edilebilir hale getirilmiştir.

> **Not:** Bu analiz, mevcut veri setindeki planlı bakım faaliyetleri ile kesinti performans göstergeleri arasındaki gözlemlenen ilişkiyi değerlendirir. Çalışma operasyonel etkiye odaklanmakta olup finansal sonuçları kapsamamaktadır.

---

### 🎯 Temel Metrikler ve Görselleştirmeler

Dashboard, operasyonel şebeke verilerini ölçülebilir performans göstergelerine dönüştürmektedir:

* **Kesinti Sıklığı Etkisi:** Bakım öncesi ve sonrası dönemler arasındaki kesinti sayısı değişimini ölçer.
* **AG & OG Dağılımı:** Gerilim seviyelerine göre kesinti performansını karşılaştırır.
* **Etkilenen Abone Analizi:** Müşteri maruziyetindeki değişimleri ölçer ve **%97,11 OG – %2,89 AG** dağılımını gösterir.
* **Kesinti Süresi Etkisi:** Bakım müdahaleleri sonrasında toplam kesinti süresindeki değişimi ölçer.
* **Operasyon Merkezi Karşılaştırması:** Bakım sonrası değişimleri ve kesinti performansını bölgesel olarak karşılaştırır.

### 🛠️ Tools & Techniques

* **Business Intelligence:** Power BI (DAX, Interactive Slicers, Custom Tooltips)
* **Data Engineering & ETL:** Python (`pandas`, `numpy`), Excel, Power Query
* **Data Modeling:** Star Schema Architecture (Fact & Dimension Tables)
* **Languages:** Python, DAX (Data Analysis Expressions)
