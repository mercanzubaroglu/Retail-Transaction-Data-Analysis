# 🛍️ Perakende Alışveriş Verisi Analizi / Retail Transaction Data Analysis

## 📦 Kullanılan Veri Seti / Dataset Used

🔗 [Kaggle: Retail Transaction Dataset](https://www.kaggle.com/datasets/bkcoban/retail-transaction-dataset)

**TR:**  
Bu projede, bir mağazada yapılan alışverişleri içeren işlem verisi kullanılmıştır. Her satır, bir müşterinin alışverişinde aldığı ürünleri ve işlem zamanını temsil etmektedir.

**EN:**  
This project uses a transaction dataset from a retail store. Each row represents the list of items purchased by a customer and the timestamp of the transaction.

---

## 🎯 Projenin Amacı / Project Objective

**TR:**  
Amacımız, müşteri alışveriş alışkanlıklarını analiz ederek:
- En çok tercih edilen ürünleri belirlemek,
- Satışların aylık ve haftalık dönemsel değişimlerini incelemek,
- Birlikte sıkça satın alınan ürün gruplarını ortaya çıkarmak,
- Ürün öneri sistemi geliştirerek müşteri davranışını modellemektir.

**EN:**  
The goal is to analyze customer shopping behavior by:
- Identifying top-selling products,
- Exploring monthly and weekly sales trends,
- Discovering frequently bought-together item sets,
- Building a basic recommendation system based on customer behavior.

---
## 🔍 Analiz Süreci / Analysis Process

### En Çok ve En Az Satılan Ürünler / Most & Least Sold Products
- Ürünler ayrıştırılıp adetlerine göre sıralandı.
- En çok ve en az tercih edilen ürünler `bar chart` ile görselleştirildi.

**EN:**  
- Split and counted product names.
- Visualized top and bottom products using bar charts.

---

### Zaman Analizi / Time Analysis
- Aylara ve haftanın günlerine göre işlem sayısı hesaplandı.
- Satış yoğunluğunun hangi dönemde arttığı tespit edildi.

**EN:**  
- Analyzed transaction counts by month and weekday.
- Identified seasonal or weekly patterns in customer activity.

---

###  Mevsimsellik Analizi / Seasonality by Product
- En popüler ürünlerin aylara göre satış dağılımı incelendi.
- Mevsimsel eğilim gösteren ürünler belirlendi.

**EN:**  
- For top products, monthly sales were plotted.
- Seasonal patterns for specific items were detected.

---

### Apriori ve Birliktelik Kuralları / Association Rules with Apriori
- Alışverişler sepete çevrilip apriori algoritması uygulandı.
- Destek, güven ve lift skorlarına göre ürünler arası ilişkiler çıkarıldı.

**EN:**  
- Transactions were one-hot encoded and fed into Apriori.
- Generated item associations based on support, confidence, and lift.

---

### Ürün Öneri Sistemi / Product Recommendation System
- Her müşterinin aldığı ürünlerden yola çıkarak benzer kullanıcılar bulundu.
- Kozinüs benzerliği ile ortak ürünler önerildi.

**EN:**  
- Built a user-item matrix to compare customers.
- Used cosine similarity to suggest new products based on similar users.

---

**📊 Görselleştirmeler / Visualizations:**
- 📅 **Monthly Transactions:** Bar chart showing sales by month.
- 🗓️ **Weekday Distribution:** Bar chart showing daily shopping intensity.
- 🧃 **Top 15 Products:** Bar chart of most frequently purchased products.
- 🧊 **Least Sold Products:** Visual analysis of least popular items.

---
