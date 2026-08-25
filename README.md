# ⚡ Grid Maintenance and Outage Impact Analysis 
*🇹🇷 Türkçe versiyon için [aşağıya kaydırın](#türkçe-versiyon)*

This project was developed to analyze the impact of grid maintenance operations on power outages. The dashboard provides analytical insights into how maintenance activities influence both the frequency and duration of outages across different operational centers.

> **🔒 Data Privacy Notice:** Due to strict company confidentiality, all original datasets and the Power BI Template (`.pbit`) file have been permanently excluded. This repository showcases the project design, visual structures, and analytical insights exclusively through documentation and screenshots.

### 📊 Dashboard Views & Analytical Insights

**1. Overall Outage Frequency Impact**
<p align="center">
  <img src="outage_count_impact.png" width="85%" title="Overall Outage Frequency Impact" />
</p>
> 💡 *Key Insight:* Demonstrates a measurable decrease in fault frequency post-intervention, validating the effectiveness of scheduled preventive maintenance in suppressing recurring grid anomalies and enhancing overall network resilience.

<br><br>

**2. Outage Source Distribution**
<p align="center">
  <img src="source_distribution.png" width="45%" title="Outage Source Distribution" />
</p>
> 💡 *Key Insight:* Highlights that Medium Voltage (MV) lines account for the vast majority of outage distribution (86.86%), indicating that capital allocation and predictive maintenance strategies must prioritize high-voltage feeder networks to maximize ROI on field operations.

<br><br>

**3. Low Voltage (LV) Outage Frequency Analysis**
<p align="center">
  <img src="lv_outage_analysis.png" width="85%" title="Low Voltage View" />
</p>
> 💡 *Key Insight:* Provides granular, localized visibility into Low Voltage network performance, mapping regional response efficiencies and helping operations centers isolate low-tier distribution bottlenecks.

<br><br>

**4. Medium Voltage (MV) Outage Frequency Analysis**
<p align="center">
  <img src="mv_outage_analysis.png" width="85%" title="Medium Voltage View" />
</p>
> 💡 *Key Insight:* Evaluates trunk-line stability for Medium Voltage infrastructure, illustrating how targeted interventions on critical feeders successfully mitigate widespread outages and protect downstream assets.

<br><br>

**5. Overall Affected Customers Impact**
<p align="center">
  <img src="affected_customers_impact.png" width="85%" title="Overall Affected Customers Impact" />
</p>
> 💡 *Key Insight:* Measures the substantial reduction in affected customer volume post-maintenance, illustrating how targeted grid interventions successfully minimize large-scale disruptions and elevate end-user service reliability.

<br><br>

**6. Low Voltage (LV) Affected Customers Analysis**
<p align="center">
  <img src="lv_affected_customers.png" width="85%" title="Low Voltage Affected Customers" />
</p>
> 💡 *Key Insight:* Evaluates customer-centric impacts specifically across Low Voltage distribution lines, tracking how localized maintenance minimizes residential and small-scale commercial disruptions.

<br><br>

**7. Medium Voltage (MV) Affected Customers Analysis**
<p align="center">
  <img src="mv_affected_customers.png" width="85%" title="Medium Voltage Affected Customers" />
</p>
> 💡 *Key Insight:* Analyzes the reduction of affected customers on critical Medium Voltage feeder lines, highlighting how high-voltage maintenance protects large consumer groups from widespread outages.

<br><br>

**8. Overall Outage Duration Impact**
<p align="center">
  <img src="outage_duration_impact.png" width="85%" title="Overall Outage Duration Impact" />
</p>
> 💡 *Key Insight:* Quantifies a consistent 25% to 45% contraction in total outage durations across regional operational centers, proving that maintenance optimization directly translates to minimized downtime and maximized service continuity.

### 🎯 Key Metrics & Visualizations
The dashboard focuses on translating raw grid data into actionable business intelligence through the following key visuals:
*   **Impact on Outage Frequencies:** Tracks the percentage change in the number of outage incidents resulting from maintenance work.
*   **LV & MV Breakdowns:** Detailed comparative performance metrics separated by grid voltage levels.
*   **Affected Customers Analysis:** Evaluates the scale of maintenance effectiveness based on the reduction of impacted customers across overall, LV, and MV tiers.
*   **Impact on Outage Durations:** Analyzes the change in total outage durations before and after maintenance interventions.

### 🛠️ Tools & Techniques
*   **Business Intelligence:** Power BI
*   **Data Preparation & Processing:** Python, Excel, Power Query
*   **Data Modeling:** Star Schema
*   **Languages:** Python, DAX (Data Analysis Expressions)

---

<h2 id="türkçe-versiyon">⚡ Şebeke Bakım ve Kesinti Etki Analizi</h2>

Bu proje, şebeke bakım çalışmalarının güç kesintileri üzerindeki etkisini analiz etmek amacıyla geliştirilmiştir. Hazırlanan dashboard, bakım operasyonlarının farklı operasyon merkezlerindeki kesinti sıklığını, etkilenen müşteri sayısını ve süresini nasıl etkilediğine dair analitik içgörüler sunar.

> **🔒 Veri Gizliliği Notu:** Şirket gizlilik politikaları gereği, tüm orijinal veri setleri ve Power BI Şablon (`.pbit`) dosyası kapsam dışı bırakılmıştır. Bu depo, dokümantasyon ve ekran görüntüleri aracılığıyla proje tasarımını, görsel yapıları ve analitik içgörüleri sergilemektedir.

### 📊 Dashboard Görünümleri ve Bulgular

**1. Genel Kesinti Sayısı Etkisi**
<p align="center">
  <img src="outage_count_impact.png" width="85%" title="Genel Kesinti Sayısı" />
</p>
> 💡 *Analitik Bulgu:* Müdahaleler sonrasında arıza sıklığında ölçülebilir bir düşüş olduğunu göstererek, planlı koruyucu bakımların tekrarlayan şebeke anomalilerini bastırmadaki ve şebeke direncini (resilience) artırmadaki etkinliğini doğrular.

<br><br>

**2. Kaynak Dağılımı**
<p align="center">
  <img src="source_distribution.png" width="45%" title="Kaynak Dağılımı" />
</p>
> 💡 *Analitik Bulgu:* Kesintilerin çok büyük bir kısmının (%86,86) Orta Gerilim (OG) hatlarından kaynaklandığını ortaya koyarak; saha operasyonlarında yatırım getirisini (ROI) maksimize etmek için sermaye tahsisi ve kestirimci bakım stratejilerinin ana besleme hatlarına odaklanması gerektiğini vurgular.

<br><br>

**3. Alçak Gerilim (AG) Kesinti Analizi**
<p align="center">
  <img src="lv_outage_analysis.png" width="85%" title="AG Görünümü" />
</p>
> 💡 *Analitik Bulgu:* Alçak gerilim şebeke performansına bölgesel ve ayrıntılı bir vizyon kazandırarak, operasyon merkezlerinin uç nokta dağıtım darboğazlarını izole etmesine ve yerel müdahale etkinliğini haritalandırmasına olanak tanır.

<br><br>

**4. Orta Gerilim (OG) Kesinti Analizi**
<p align="center">
  <img src="mv_outage_analysis.png" width="85%" title="OG Görünümü" />
</p>
> 💡 *Analitik Bulgu:* Kritik orta gerilim altyapısı için ana hat kararlılığını değerlendirerek, kritik besleyiciler üzerinde yapılan hedefli müdahalelerin yaygın kesintileri nasıl başarıyla önlediğini ve alt şebeke varlıklarını koruduğunu gösterir.

<br><br>

**5. Genel Etkilenen Müşteri Sayısı Etkisi**
<p align="center">
  <img src="affected_customers_impact.png" width="85%" title="Genel Etkilenen Müşteri Sayısı" />
</p>
> 💡 *Analitik Bulgu:* Bakım çalışmaları sonrasında kesintilerden etkilenen müşteri hacmindeki ciddi düşüşü ölçerek, hedefli şebeke müdahalelerinin büyük ölçekli kesintileri nasıl en aza indirdiğini ve son kullanıcı hizmet güvenilirliğini artırdığını ortaya koyar.

<br><br>

**6. Alçak Gerilim (AG) Etkilenen Müşteri Analizi**
<p align="center">
  <img src="lv_affected_customers.png" width="85%" title="AG Etkilenen Müşteriler" />
</p>
> 💡 *Analitik Bulgu:* Alçak gerilim dağıtım hatlarındaki müşteri odaklı etkileri değerlendirerek, yerel bakımların konut ve küçük ölçekli ticari kesintileri nasıl azalttığını takip eder.

<br><br>

**7. Orta Gerilim (OG) Etkilenen Müşteri Analizi**
<p align="center">
  <img src="mv_affected_customers.png" width="85%" title="OG Etkilenen Müşteriler" />
</p>
> 💡 *Analitik Bulgu:* Kritik orta gerilim besleme hatlarında etkilenen müşteri sayısındaki azalışı analiz ederek, yüksek gerilim bakımlarının geniş müşteri kitlelerini yaygın kesintilerden nasıl koruduğunu vurgular.

<br><br>

**8. Genel Kesinti Süresi Etkisi**
<p align="center">
  <img src="outage_duration_impact.png" width="85%" title="Genel Kesinti Süresi" />
</p>
> 💡 *Analitik Bulgu:* Bölgesel operasyon merkezlerinde toplam kesinti sürelerinde tutarlı bir şekilde %25 ila %45 daralma olduğunu kantitatif olarak kanıtlayarak, bakım optimizasyonunun doğrudan minimum kesinti süresine (downtime) ve gelişmiş hizmet sürekliliğine dönüştüğünü gösterir.

### 🛠️ Kullanılan Araçlar ve Teknikler
*   **İş Zekası (BI):** Power BI
*   **Veri Hazırlama ve İşleme:** Python, Excel, Power Query
*   **Veri Modelleme:** Yıldız Şema (Star Schema)
*   **Diller:** Python, DAX
