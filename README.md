# Dijital Duyarlılık ve Makroekonomik Göstergeler Arasındaki İlişki Analizi

Bu projede, Türkiye’de açıklanan makroekonomik göstergeler ile dijital duyarlılık arasındaki ilişki incelenmektedir. Projede, Google Trends üzerinden elde edilen "euro", "dolar", "faiz" ve "enflasyon" arama trend verileri ile iki resmi ekonomik veri seti (Fiyat Endeksi [Tüketici Fiyatları] (2003=100) ve Bankalarca Açılan Kredilere Uygulanan Ağırlıklı Ortalama Faiz Oranları) kullanılarak zaman serisi analizi yapılacaktır.

## Proje Hakkında

**Amaç:**  
Projenin temel amacı, dijital arama trendlerinin resmi ekonomik göstergeler (enflasyon ve kredi faiz oranları) ile ilişkisini ortaya koymaktır. Bu ilişki sayesinde, dijital duyarlılık üzerinden erken uyarı sinyalleri yakalanması ve ekonomik politikaların dijital yansımalarının analiz edilmesi hedeflenmektedir.

**Kapsam:**  
- Google Trends üzerinden "euro", "dolar", "faiz" ve "enflasyon" terimlerinin son 1 yıl içerisindeki arama trendlerinin toplanması.
- TÜİK tarafından yayınlanan Fiyat Endeksi (Tüketici Fiyatları) (2003=100) verisinin temini.
- TCMB tarafından yayınlanan Bankalarca Açılan Kredilere Uygulanan Ağırlıklı Ortalama Faiz Oranları verisinin temini.
- Zaman serisi analizi, korelasyon testleri (ör. Pearson, Spearman) ve zaman gecikmesi (lag) etkilerinin incelenmesi (ör. Granger nedensellik testi).

## Veri Kaynakları

- **Google Trends Verileri:**  
  - Arama terimleri: "euro", "dolar", "faiz", "enflasyon".  
  - Veriler, Google Trends API veya manuel indirme yöntemleriyle elde edilecektir.

- **Fiyat Endeksi (Tüketici Fiyatları) (2003=100):**  
  - Resmi TÜİK veri portalından temin edilebilir.  
  - [TÜİK Veri Portalı](https://data.tuik.gov.tr/)

- **Bankalarca Açılan Kredilere Uygulanan Ağırlıklı Ortalama Faiz Oranları:**  
  - Resmi TCMB web sitesinden temin edilebilir.  
  - [TCMB İstatistikler](https://www.tcmb.gov.tr/wps/wcm/connect/tcmb+tr/tcmb+tr/main+menu/istatistikler)

## Kullanılan Yöntem ve Teknolojiler

- **Programlama Dili:** Python
- **Kütüphaneler:**  
  - `pandas`, `numpy` (veri işleme ve analiz)  
  - `matplotlib`, `seaborn` veya alternatif görselleştirme kütüphaneleri (grafik oluşturma)  
  - `statsmodels` (istatistiksel testler, Granger nedensellik testi)  
  - `pytrends` (Google Trends verilerinin toplanması)
- **Analiz Yöntemleri:**  
  - Zaman serisi analizi  
  - Korelasyon analizi (Pearson ve Spearman)  
  - Granger nedensellik testi (zaman gecikmesi etkilerinin incelenmesi)

## Proje Akışı

1. **Veri Toplama:**  
   - Google Trends API kullanılarak gerekli arama trend verilerinin toplanması.
   - TÜİK ve TCMB kaynaklarından ilgili ekonomik verilerin indirilmesi.

2. **Veri Temizleme ve Ön İşleme:**  
   - Tarih uyumluluğu sağlanması ve verilerin ölçeklendirilmesi.
   - Gerekli veri dönüşümlerinin uygulanması.

3. **Analiz:**  
   - Zaman serisi grafiklerinin oluşturulması.
   - Korelasyon analizlerinin yapılması.
   - Gecikme etkilerinin incelenmesi için Granger nedensellik testlerinin uygulanması.

4. **Sonuçların Yorumlanması:**  
   - Elde edilen bulguların yorumlanması.
   - Dijital duyarlılık ile ekonomik göstergeler arasındaki ilişkinin değerlendirilmesi.

5. **Raporlama ve Sunum:**  
   - Analiz sonuçlarının görselleştirilmesi ve raporlanması.
   - Proje çıktılarının sunulması.

## Nasıl Çalıştırılır?

1. **Gerekli Kütüphaneleri Yükleyin:**

   ```bash
   pip install pandas numpy matplotlib statsmodels pytrends
