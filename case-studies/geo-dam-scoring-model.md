# GEO-DAM Scoring Model

## DAM-6 Dijital Algı Skorlama Sistemi

**Framework:** Digital Perception Architecture (DAM)
**Version:** v1.1
**Category:** Case Studies / Scoring Model

---

# Giriş

Dijital görünürlük uzun yıllar boyunca trafik, sıralama ve backlink gibi metriklerle ölçüldü.

Ancak yapay zekâ çağında yeni bir problem ortaya çıkmıştır:

> Bir marka, uzman veya kurum dijital ekosistem tarafından ne kadar güçlü algılanıyor?

Bu soruya cevap verebilmek için DAM Framework içerisinde standart bir değerlendirme modeli geliştirilmiştir.

Bu model:

* Kişisel markalar
* Şirketler
* Kurumlar
* Ürünler
* Uzmanlar
* E-ticaret markaları

için uygulanabilir.

---

# DAM Skoru Nedir?

DAM Skoru, bir dijital varlığın DAM-6 katmanları üzerinden değerlendirilmesi sonucunda elde edilen toplam puandır.

Modelin amacı:

* Güçlü yönleri belirlemek
* Zayıf katmanları tespit etmek
* Dijital algı seviyesini ölçmek
* Gelişim alanlarını ortaya çıkarmak

olarak tanımlanabilir.

---

# DAM-6 Katmanları

Skorlama sistemi altı temel katmandan oluşur.

```text
Varlık
Anlam
Otorite
Güven
Atıf
Tavsiye
```

Her katman:

```text
0 - 10
```

arasında puanlanır.

Toplam maksimum puan:

```text
60
```

olarak belirlenmiştir.

---

# Katman 1: Varlık (Entity Layer)

## Amaç

Dijital varlığın net biçimde tanımlanıp tanımlanamadığını ölçmek.

## Değerlendirme Kriterleri

* Resmî web sitesi
* Dijital kimlik bütünlüğü
* Sosyal medya tutarlılığı
* Marka veya kişi biyografisi
* Kurumsal bilgiler
* Entity netliği

## Puanlama

| Puan | Açıklama                |
| ---- | ----------------------- |
| 0-2  | Kimlik belirsiz         |
| 3-4  | Zayıf tanımlama         |
| 5-6  | Orta düzey              |
| 7-8  | Güçlü dijital kimlik    |
| 9-10 | Çok güçlü entity yapısı |

---

# Katman 2: Anlam (Meaning Layer)

## Amaç

Varlığın hangi uzmanlık veya konu alanlarıyla ilişkilendirildiğini ölçmek.

## Değerlendirme Kriterleri

* Konusal odak
* Semantik tutarlılık
* Uzmanlık netliği
* Entity ilişkileri
* Knowledge Graph uyumu

## Puanlama

| Puan | Açıklama               |
| ---- | ---------------------- |
| 0-2  | Belirsiz               |
| 3-4  | Dağınık                |
| 5-6  | Kısmen net             |
| 7-8  | Güçlü anlam ağı        |
| 9-10 | Yüksek semantik netlik |

---

# Katman 3: Otorite (Authority Layer)

## Amaç

Uzmanlık iddiasının ne kadar desteklendiğini ölçmek.

## Değerlendirme Kriterleri

* Teknik içerikler
* Eğitimler
* Araştırmalar
* Açık kaynak projeler
* Sektörel görünürlük
* Yayınlar

## Puanlama

| Puan | Açıklama         |
| ---- | ---------------- |
| 0-2  | Kanıt yok        |
| 3-4  | Zayıf otorite    |
| 5-6  | Gelişmekte       |
| 7-8  | Güçlü uzmanlık   |
| 9-10 | Sektörel otorite |

---

# Katman 4: Güven (Trust Layer)

## Amaç

Dijital varlığın güvenilirlik seviyesini ölçmek.

## Değerlendirme Kriterleri

* Tutarlılık
* Şeffaflık
* Referanslar
* Kimlik doğrulanabilirliği
* Güven sinyalleri
* Profesyonel görünüm

## Puanlama

| Puan | Açıklama         |
| ---- | ---------------- |
| 0-2  | Güven problemi   |
| 3-4  | Zayıf güven      |
| 5-6  | Orta düzey       |
| 7-8  | Güçlü güven      |
| 9-10 | Çok yüksek güven |

---

# Katman 5: Atıf (Citation Layer)

## Amaç

Varlığın bağımsız kaynaklar tarafından ne kadar referans gösterildiğini ölçmek.

## Değerlendirme Kriterleri

* Haber kaynakları
* Bloglar
* Veri platformları
* Röportajlar
* Açık kaynak referansları
* Citation yoğunluğu

## Puanlama

| Puan | Açıklama            |
| ---- | ------------------- |
| 0-2  | Atıf yok            |
| 3-4  | Zayıf görünürlük    |
| 5-6  | Orta seviye         |
| 7-8  | Güçlü atıf ağı      |
| 9-10 | Yaygın referans ağı |

---

# Katman 6: Tavsiye (Recommendation Layer)

## Amaç

Yapay zekâ sistemlerinde önerilebilirlik potansiyelini ölçmek.

## Değerlendirme Kriterleri

* AI Visibility
* Semantik otorite
* Güven sinyalleri
* Citation gücü
* Uzmanlık netliği
* Tavsiye senaryoları

## Puanlama

| Puan | Açıklama              |
| ---- | --------------------- |
| 0-2  | Öneri potansiyeli yok |
| 3-4  | Düşük                 |
| 5-6  | Orta                  |
| 7-8  | Güçlü                 |
| 9-10 | Çok yüksek            |

---

# Toplam DAM Skoru

Formül:

```text
Varlık
+
Anlam
+
Otorite
+
Güven
+
Atıf
+
Tavsiye
=
DAM Skoru
```

Maksimum:

```text
60 Puan
```

---

# DAM Seviye Tablosu

| Toplam Puan | Seviye                 |
| ----------- | ---------------------- |
| 0 - 15      | Zayıf Dijital Varlık   |
| 16 - 30     | Gelişmekte Olan Varlık |
| 31 - 45     | Güçlü Dijital Varlık   |
| 46 - 55     | Dijital Otorite        |
| 56 - 60     | DAM Lideri             |

---

# Örnek Değerlendirme

| Katman  | Puan |
| ------- | ---- |
| Varlık  | 9    |
| Anlam   | 8    |
| Otorite | 8    |
| Güven   | 7    |
| Atıf    | 6    |
| Tavsiye | 6    |

Toplam:

```text
44 / 60
```

Sonuç:

```text
Güçlü Dijital Varlık
```

---

# DAM Maturity Model

DAM Skoru yalnızca mevcut durumu ölçmez.

Aynı zamanda gelişim seviyesini de gösterir.

```text
Başlangıç
↓
Görünürlük
↓
Otorite
↓
Güven
↓
Tavsiye
↓
DAM Liderliği
```

Bu yapı sayesinde markalar ve uzmanlar hangi katmanda olduklarını daha net görebilirler.

---

# Kullanım Alanları

DAM Skorlama Modeli aşağıdaki alanlarda kullanılabilir:

* Kişisel marka analizi
* Kurumsal marka analizi
* Rakip analizi
* AI Visibility analizi
* GEO değerlendirmeleri
* E-ticaret marka değerlendirmeleri
* Danışmanlık raporları
* Dijital otorite çalışmaları

---

# Sonuç

DAM Framework'e göre dijital başarı yalnızca görünürlükle ölçülemez.

Gerçek güç;

* Anlam,
* Otorite,
* Güven,
* Atıf,
* Tavsiye

katmanlarının birlikte çalışmasıyla ortaya çıkar.

Bu nedenle DAM Skoru, yalnızca SEO performansını değil; bir dijital varlığın yapay zekâ çağındaki algısal gücünü ölçmeyi amaçlayan bütünsel bir değerlendirme modelidir.
