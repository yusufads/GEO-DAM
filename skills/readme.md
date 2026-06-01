# GEO-PRO Skill – Derinlemesine DAM-6 Analizi

**Yazar:** Yusuf Şahin - https://yusufads.net/hakkimda
**Proje:** [GEO-DAM](https://github.com/yusufads/GEO-DAM)  
**Sürüm:** 3.0 – Profesyonel  
**Uyumluluk:** ChatGPT (Custom GPT), Claude (System Prompt), Gemini, Perplexity (Web enabled)

---

## 🎯 Amaç

Bu skill, bir markanın veya web sitesinin üretken yapay zeka motorları nezdindeki dijital algısını DAM-6 metodolojisinin **6 katmanında (Varlık → Anlam → Otorite → Güven → Atıf → Tavsiye)** ölçer, puanlar ve iyileştirme için somut aksiyon önerileri sunar. Rakiplerle karşılaştırma, bağlamsal analiz ve trend takibi de yapılabilir.

---

## 🔧 Analiz Yetenekleri (Derinlemesine)

### Katman 1: Varlık (Entity) – 15 puan
- **Neler kontrol edilir:**  
  - Marka adının tam ve kısaltılmış varyantları  
  - Domain, alt domainler  
  - Sosyal medya hesapları (resmî ve doğrulanmış)  
  - Wikipedia, Wikidata, Crunchbase, LinkedIn Company  
  - Daha önce kullanılmış eski marka isimleri veya yanlış yazımlar  
- **Sorgu örneği:** `"Kullanıcıya [Marka X] hakkında temel bilgiler ver."`  
- **Ölçüt:** Yapay zeka cevabında kaç doğru entity eşleşmesi var? (0–5 arası)  
- **Puanlama:** Her tanınan entity +3 puan (maks 15).  
- **Eksiklik tespiti:** Hangi alias/hesap hiç bilinmiyor?

### Katman 2: Anlam (Semantic) – 15 puan
- **Bağlam matrisi:**  
  - Sektör / kategori (örn: e-ticaret, SaaS, sağlık)  
  - Ürün/hizmet anahtar kelimeleri  
  - Hedef kitle (B2B, B2C, geliştirici, KOBİ, kurumsal)  
  - Coğrafi ilişki (ülke, şehir)  
- **Sorgu örneği:** `"[Marka X] hangi sektörde faaliyet gösterir? Kime hitap eder?"`  
- **Ölçüt:** Üretici AI’nın verdiği bağlam etiketlerinin doğruluk ve zenginlik skoru (1-10).  
- **Puanlama:** Her doğru bağlam +3 puan (yanlış veya eksik -1).  
- **Eksiklik:** Hangi önemli bağlam (örn: “mobil uyumlu”) hiç geçmiyor?

### Katman 3: Otorite (Authority) – 20 puan
- **Kaynak denetimi:**  
  - Yapay zeka hangi domainleri referans gösteriyor?  
  - Domain Authority (DA) skoru (Moz, Ahrefs benzeri)  
  - Alıntı yapılan sitelerin güvenilirliği (resmî, akademik, haber, forum)  
  - Markanın kendi sitesi dışındaki kaynak sayısı  
- **Sorgu örneği:** `"[Marka X] hakkında bilgi verirken hangi kaynakları kullanıyorsun?"` (AI’ya yönelt)  
- **Ölçüt:** Dış otoriter kaynak sayısı × ortalama DA.  
- **Puanlama:** 0-20 arası normalize edilmiş skor.  
- **Eksiklik:** Backlink havuzu yoksa veya sadece kendi basın bültenleri varsa kırmızı bayrak.

### Katman 4: Güven (Trust) – 20 puan
- **Duygu analizi:**  
  - Yapay zeka çıktılarında olumlu/olumsuz/nötr oranı  
  - Çelişkili ifadeler (örnek: “başarılı ama güvenilmez”)  
  - Net Promoter benzeri sözel skor (“şiddetle tavsiye ederim” gibi)  
- **Sorgu örneği:** `"[Marka X] güvenilir bir şirket mi? Müşteri yorumları neler?"`  
- **Ölçüt:** Olumlu cümle oranı ve çelişki sayısı.  
- **Puanlama:** Olumlu% × 20 – (çelişki sayısı×2). Maks 20.  
- **Eksiklik:** Çelişkili bilgi veya hiç duygu ifade edilmemesi.

### Katman 5: Atıf (Citation) – 15 puan
- **Öneri sıklığı analizi:**  
  - “En iyi 5 [ürün kategorisi]” gibi listelerde markanın geçme sıklığı  
  - Rakiplerle karşılaştırmalı atıf oranı  
  - Ürün bazlı atıf (spesifik model/hizmet)  
- **Sorgu örneği:** `"En iyi 5 [kategori] nedir?"` ve `"[Marka X] ile [Rakip Y] karşılaştırması"`  
- **Ölçüt:** Markanın ilk 5’te geçme yüzdesi (10 farklı sorguda).  
- **Puanlama:** % × 15.  
- **Eksiklik:** Liste sorgularında marka hiç yoksa veya her zaman rakiplerin altındaysa.

### Katman 6: Tavsiye (Recommendation) – 15 puan
- **İkna edicilik analizi:**  
  - Yapay zeka markayı hangi tonla tavsiye ediyor? (kesin, şartlı, zayıf)  
  - Hangi kullanıcı ihtiyaçlarında öne çıkıyor? (fiyat, özellik, destek)  
  - Çapraz satış potansiyeli (marka başka ürünlerle birlikte öneriliyor mu?)  
- **Sorgu örneği:** `"Hangi [kategori] ürününü almalıyım? Bütçem kısıtlı/kalite önemli"`  
- **Ölçüt:** Tavsiye gücü (1-5) ve bağlam uygunluğu (1-3).  
- **Puanlama:** (güç × bağlam) × 3. Maks 15.  
- **Eksiklik:** Sadece fiyat duyarlı sorgularda çıkması veya hiç çıkmaması.

---

## 📊 Toplam Dijital Algı Skoru (DAS – Digital Awareness Score)

**DAS = (Katman1 + Katman2 + Katman3 + Katman4 + Katman5 + Katman6)**  

- **90-100:** Mükemmel – AI dostu marka  
- **70-89:** İyi – küçük iyileştirmeler  
- **50-69:** Orta – eksiklikler var  
- **30-49:** Düşük – acil müdahale gerek  
- **0-29:** Kritik – marka neredeyse görünmez

---

## 🧠 Analiz İş Akışı (Skill’in Çalışma Mantığı)

1. Kullanıcı `geo-pro-skill` tetikleme komutu verir (ör: “GEO-PRO ile analiz et [marka]”).
2. Asistan, yukarıdaki 6 katman için önceden tanımlanmış sorguları **arka arkaya** (veya paralel düşünerek) yanıtlar.
3. Her yanıt, katmanın puanlama kriterine göre değerlendirilir.
4. Tüm puanlar toplanır, DAS hesaplanır ve raporlanır.
5. Her katmandaki eksiklikler için **somut eylem maddeleri** üretilir (ör: “Wikipedia sayfası oluştur”, “En iyi 5 listelerinde atıf almak için karşılaştırma sayfası aç”).
6. Rapor, yatırım getirisi önceliğine göre sıralanmış aksiyon planı ile sonlanır.

> **Not:** Analiz sırasında asistanın **internet/web arama** özelliği açık olmalıdır. Aksi takdirde sadece eğitim verisiyle sınırlı kalır.

---

## 📤 Örnek Rapor Çıktısı (Özet)

```markdown
## GEO-PRO Raporu: Acme Teknoloji (acme.com)  
*Analiz Tarihi: 2026-06-01 | Analist: Yusuf Şahin / GEO-DAM*

| Katman | Puan | Durum | En Kritik Eksiklik |
|--------|------|-------|--------------------|
| Varlık | 12/15 | 🟢 İyi | Eski marka adı “AcmeSoft” tanınmıyor |
| Anlam  | 8/15  | 🟠 Orta | “bulut tabanlı” bağlamı yok |
| Otorite| 4/20  | 🔴 Zayıf | Tek kaynak: kendi sitesi |
| Güven  | 14/20 | 🟢 İyi | Olumlu ton ancak çelişki yok |
| Atıf   | 3/15  | 🔴 Kritik | “En iyi 5 yazılım” listelerinde yer almıyor |
| Tavsiye| 6/15  | 🟠 Orta | Sadece ücretsiz deneme sorgularında çıkıyor |

**Toplam DAS:** 47/100 → **Düşük Görünürlük**

### 🔥 İlk 3 Acil Eylem (Yusuf Şahin – GEO-DAM)
1. **Atıf artırma:** Sektörünüzdeki “en iyi” listelerine dahil olmak için karşılaştırma içerikleri oluşturun ve yetkili sitelere gönderin.
2. **Otorite inşa:** Sitenize referans veren güvenilir haber siteleri veya akademik kaynaklar hedefleyin.
3. **Anlam genişletme:** İçeriklerinizde “bulut tabanlı”, “KOBİ uyumlu” gibi kavramları şema işaretlemesiyle güçlendirin.
