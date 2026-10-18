# SERİNBOYA: Yerli Barit ve Kalsitle Düşük Maliyetli Radyatif Soğutma Boyası ve İstanbul'da Çatı Saha Testi

**Önerilen proje adı:** Türkiye Kaynaklı Barit (BaSO₄) ve Kalsit (CaCO₃) Pigmentleriyle Gündüz Ortam Altı Radyatif Soğutma Boyalarının Geliştirilmesi, Optik Karakterizasyonu ve Nemli İklimde (İstanbul) Çatı Ölçeğinde Saha Performansının Belirlenmesi

**Kısa ad:** SERİNBOYA
**Alan:** Malzeme bilimi / Bina enerji verimliliği / Pasif soğutma
**Uygun TÜBİTAK programları:** 1001 (Bilimsel ve Teknolojik Araştırma Projeleri), 1002-A (Hızlı Destek Modülü), 3501 (Kariyer), lisans öğrencileri için 2209-A, sanayi ortağıyla 1505 (Üniversite-Sanayi İşbirliği)
**Önerilen süre:** 24 ay (1002-A ve 2209-A için daraltılmış 12 aylık sürüm Bölüm 12'de)

---

## 1. Proje bir cümlede

Türkiye'de çıkarılan **barit ve kalsit cevherlerinden** hazırlanan pigmentlerle, güneş ışığının yaklaşık %95 ve üzerini yansıtan ve ısısını 8-13 µm "atmosfer penceresi" üzerinden uzaya salan, **güneş altında bile ortam sıcaklığının altına inebilen**, ticari boya maliyetine yakın bir çatı boyası geliştirmek ve bu boyayı **İstanbul'da gerçek bir çatıda, nemli iklim koşullarında, en az bir yaz ve bir kış boyunca** ticari beyaz boya ve çıplak çatı yüzeyiyle yan yana test etmek.

## 2. Radyatif soğutma nedir?

Her yüzey sıcaklığına bağlı olarak kızılötesi ışınım yayar. Atmosfer 8-13 µm aralığında büyük ölçüde geçirgendir (**atmosfer penceresi**). Bu aralıkta yayılan ısı doğrudan yaklaşık 3 K sıcaklığındaki uzaya kaçar. Bir yüzey:

1. **Güneşi yansıtırsa** (0,3-2,5 µm aralığında yüksek yansıtma, R),
2. **Atmosfer penceresinde güçlü yayarsa** (8-13 µm aralığında yüksek yayıcılık, ε),

elektrik harcamadan, gündüz bile çevresinden daha soğuk kalabilir.

**Enerji dengesi (birim alan için):**

```
P_net = P_ışınım(T_yüzey) - P_atmosfer(T_ortam) - P_güneş - P_taşınım+iletim

P_ışınım   = ε · σ · T_yüzey⁴
P_atmosfer = ε · ε_gök · σ · T_ortam⁴
P_güneş    = (1 - R) · G
P_taşınım  = h · (T_ortam - T_yüzey)
```

`G` güneş ışınımı (W/m²), `σ` Stefan-Boltzmann sabiti, `h` taşınım katsayısı, `ε_gök` gökyüzünün etkin yayıcılığıdır. `ε_gök` havadaki neme (çiğ noktasına) bağlıdır: hava nemlendikçe atmosfer penceresi kısmen kapanır ve soğutma gücü düşer. **Bu yüzden nemli İstanbul, kuru iklimlere göre zor ama bilimsel olarak değerli bir test sahasıdır.**

Kritik nokta güneş yansıtmasıdır: Öğle saatinde ~900 W/m² güneş altında yansıtmadaki **her 1 puanlık artış ~9 W/m² daha az ısı** demektir. Tipik soğutma gücü 50-120 W/m² olduğu için R'nin 0,90'dan 0,97'ye çıkması, "ısınan beyaz boya" ile "ortamın altına inen boya" arasındaki farktır.

## 3. Neden BaSO₄ ve CaCO₃? Neden TiO₂ değil?

Ticari beyaz boyaların neredeyse tamamı **titanyum dioksit (TiO₂)** kullanır. TiO₂'nin kırılma indisi yüksektir (görünür bölgede çok iyi örtücü), ancak **bant aralığı ~3,0-3,2 eV olduğundan 400 nm altındaki morötesi ışığı soğurur.** Güneş enerjisinin yaklaşık %5-7'si morötesindedir; bu soğurma tek başına gündüz ortam altı soğutmayı imkânsız hâle getirebilir.

| Özellik | TiO₂ (rutil) | BaSO₄ (barit) | CaCO₃ (kalsit) |
|---|---|---|---|
| Bant aralığı | ~3,0 eV (UV soğurur) | ~6 eV (UV'yi yansıtır) | ~6 eV (UV'yi yansıtır) |
| Kırılma indisi | ~2,6 | ~1,64 | ~1,49-1,66 |
| Örtücülük | Çok yüksek | Orta (yüksek dolgu oranı gerekir) | Orta |
| Kızılötesi | Pencerede orta | ~9 µm'de güçlü fonon rezonansı, pencerede yüksek yayıcılık | ~7 µm ve ~11 µm bantları |
| Maliyet | Yüksek, büyük ölçüde ithal | Düşük, **Türkiye'de üretiliyor** | Çok düşük, **Türkiye'de bol** |
| Literatürdeki boya | Ticari beyaz, R ≈ 0,80-0,90 | Purdue 2021, R = 0,981 | Purdue 2020, R = 0,955 |

Düşük kırılma indisini telafi etmek için yüksek pigment hacim oranı (BaSO₄ boyada ~%60) ve **geniş tane boyu dağılımı** kullanılır: farklı boyuttaki taneler farklı dalga boylarını saçar ve yansıtma tüm güneş spektrumunda yükselir.

## 4. Dünyadaki literatür

| Yıl | Çalışma | Malzeme / yaklaşım | Öne çıkan sonuç |
|---|---|---|---|
| 2014 | Raman ve ark., *Nature* 515, 540 | Çok katmanlı fotonik yapı | Doğrudan güneş altında ortamın ~4,9 °C altı; gündüz radyatif soğutmanın ilk güçlü gösterimi |
| 2017 | Zhai ve ark., *Science* 355, 1062 | Cam mikroküre katkılı polimer film | Ölçeklenebilir, rulo üretilebilir film; ~93 W/m² soğutma gücü |
| 2018 | Mandal ve ark., *Science* 362, 315 | Gözenekli P(VdF-HFP) kaplama | Boya gibi sürülebilen gözenekli polimer; R ≈ 0,96 |
| 2020 | Li ve ark., *Cell Reports Physical Science* 1, 100221 | **CaCO₃** akrilik boya | R ≈ 0,955; ticari boyaya benzer formülle gündüz ortam altı |
| 2021 | Li ve ark., *ACS Applied Materials & Interfaces* 13, 21733 | **BaSO₄** akrilik boya (%60 hacim) | R = 0,981, ε = 0,95; öğlen ~4,5 °C ortam altı, ~117 W/m² soğutma gücü; 600'ü aşkın atıf |

> **Sonuç:** Malzemenin kendisi yeni değildir. Özgünlük, **yerli hammadde**, **nemli iklimde uzun süreli saha testi** ve **maliyet/dayanıklılık** ekseninde kurulmalıdır.

## 5. Türkiye'deki durum ve boşluk

- Başlığında "radiative cooling" geçen, Türkiye adresli **yaklaşık 36 yayın** tespit edilmiştir.
- Bu çalışmalar ağırlıkla **ince film, fotonik/optik tasarım ve sayısal modelleme** düzeyindedir.
- **Boya formunda bir radyatif soğutucu ile yapılmış saha testine rastlanmamıştır.**
- **Yerli barit veya kalsit cevherinin radyatif soğutma pigmenti olarak** karakterize edildiği bir çalışma bulunmamıştır.

> **Not:** Başvuru öncesinde Web of Science, Scopus, ULAKBİM TR Dizin ve YÖK Tez veri tabanlarında "radiative cooling", "daytime radiative cooling paint", "BaSO4 paint", "CaCO3 paint", "radyatif soğutma", "pasif soğutma boyası" anahtar kelimeleriyle güncel tarama yapılmalı, 36 yayın sayısı tarih ve sorgu cümlesiyle birlikte raporlanmalı ve bu bölümdeki her iddia künyeli kaynakla desteklenmelidir.

## 6. Yerli hammadde avantajı

Türkiye hem **barit** hem de **kalsit / mikronize kalsit** üretiminde dünyanın önde gelen ülkeleri arasındadır ve bu ürünlerin önemli bir kısmı düşük katma değerle (sondaj çamuru, dolgu malzemesi olarak) ihraç edilmektedir.

| Hammadde | Bilinen başlıca üretim bölgeleri (doğrulanmalı) | Bugünkü ana kullanım | Projedeki rolü |
|---|---|---|---|
| Barit (BaSO₄) | Antalya (Alanya, Gazipaşa), Isparta (Şarkikaraağaç), Muş, Kahramanmaraş, Konya | Petrol/gaz sondaj çamuru | Yüksek performanslı soğutucu pigment |
| Kalsit (CaCO₃) | Niğde, Afyonkarahisar, Kırşehir, Balıkesir, Muğla | Kâğıt, plastik, boya dolgusu | Düşük maliyetli soğutucu pigment |

**Asıl bilimsel soru: Safsızlık.** Laboratuvar çalışmalarında yüksek saflıkta ticari BaSO₄ kullanılmıştır. Doğal cevherde bulunan **demir oksit (Fe₂O₃), SrSO₄, SiO₂ ve kil** gibi safsızlıklar görünür ve yakın kızılötesinde soğurmaya yol açarak yansıtmayı düşürebilir. Proje şu soruyu cevaplar:

> *Hangi saflık seviyesi ve hangi basit zenginleştirme adımı (yıkama, manyetik ayırma, eleme, öğütme) ile yerli cevher, ithal saf pigmentin performansına ne kadar yaklaşır ve bunun maliyeti nedir?*

Bu, hem bilimsel (safsızlık-yansıtma ilişkisi) hem de ekonomik (yerli cevherde katma değer) bir katkıdır.

## 7. Neden İstanbul? Zorluk bir bulgudur

- İstanbul'da yaz çiğ noktası sık sık 18-20 °C'ye çıkar. Bu, gökyüzü yayıcılığını artırır ve soğutma gücünü kuru iklimlere göre belirgin biçimde düşürür.
- Yoğun kentsel kirlilik ve toz, yüzeyin zamanla kirlenmesine ve yansıtmanın düşmesine neden olur.
- Literatürdeki saha testleri ağırlıkla **kuru veya ılıman iklimlerde ve kısa süreli** (birkaç gün) yapılmıştır.

Bu yüzden İstanbul'da yapılacak **en az 6-12 aylık** bir test, "nemli ve kirli kent ortamında bu boyalar gerçekte ne kadar işe yarar?" sorusuna doğrudan cevap verir. Bütçe izin verirse ikinci bir **kuru iklim sahası** (ör. Konya veya Ankara) ile eş zamanlı karşılaştırma yapılması projeyi çok güçlendirir.

## 8. Özgün değer (projeyi farklı kılan 5 nokta)

1. **Yerli cevherden pigment:** Türkiye kaynaklı barit ve kalsitin radyatif soğutma pigmenti olarak ilk sistematik karakterizasyonu; **safsızlık-yansıtma ilişkisinin** nicel olarak ortaya konması.
2. **Nemli iklimde uzun süreli saha testi:** İstanbul'da gerçek bir çatıda, en az bir yaz ve bir kış boyunca, ticari beyaz boya ve çıplak çatı ile **eş zamanlı, yan yana** ölçüm. Türkiye'de boya formunda ilk radyatif soğutma saha testi.
3. **Kirlenme ve yaşlanma verisi:** Kent ortamında yansıtmanın aylık takibi ve hızlandırılmış UV/nem yaşlandırma ile karşılaştırma; temizlenebilirlik (yağmurla kendini temizleme) değerlendirmesi.
4. **Maliyet odaklı formülasyon:** Pigment hacim oranı, tane boyu dağılımı ve bağlayıcı türünün deney tasarımı (DoE) ile optimizasyonu; **m² başına maliyetin ticari boyayla** karşılaştırılması.
5. **Bina ölçeği etki:** Ölçülen optik özelliklerle kalibre edilmiş bina enerji simülasyonu (EnergyPlus vb.) ile İstanbul'daki tipik binalar için soğutma enerjisi tasarrufu ve kentsel ısı adası etkisinin tahmini.

## 9. Araştırma soruları ve hipotezler

| # | Soru | Hipotez |
|---|---|---|
| S1 | Yerli barit ve kalsit cevherindeki safsızlıklar güneş yansıtmasını ne kadar düşürür? | Fe₂O₃ içeriği belirli bir eşiğin altına indirildiğinde R ≥ 0,95 yakalanabilir |
| S2 | Basit zenginleştirme (yıkama, manyetik ayırma, eleme) ile ithal saf pigmente ne kadar yaklaşılır? | Düşük maliyetli adımlarla aradaki fark R'de 0,02'nin altına iner |
| S3 | İstanbul'un nemli yaz koşullarında gündüz ortam altı soğutma mümkün müdür? | BaSO₄ boya açık havalı yaz öğle saatlerinde ortam sıcaklığına yakın veya altında kalır; ticari beyaz boyadan belirgin derecede soğuktur |
| S4 | Kent ortamında kirlenme yansıtmayı ne hızla düşürür? | İlk aylarda hızlı, sonra yağışla dengelenen bir düşüş görülür |
| S5 | Bina ölçeğinde tasarruf ne kadardır? | Yalıtımı zayıf, düz çatılı binalarda soğutma yükünde anlamlı azalma sağlanır |

## 10. Amaç ve hedefler

**Ana amaç:** Yerli barit ve kalsitten düşük maliyetli radyatif soğutma boyaları geliştirmek ve bu boyaların nemli kent iklimindeki gerçek performansını uzun süreli çatı testleriyle ortaya koymak.

**Ölçülebilir hedefler (başarı ölçütleri, hedef değerler):**

| Hedef | Ölçüt |
|---|---|
| H1 | En az 3 barit ve 3 kalsit numunesinin XRD/XRF, tane boyu ve spektral yansıtma ile karakterizasyonu |
| H2 | En iyi yerli BaSO₄ boyada güneş yansıtması R ≥ 0,95 (ASTM E903), atmosfer penceresinde yayıcılık ε ≥ 0,92 |
| H3 | Açık havalı yaz öğle saatlerinde, yüzey sıcaklığının ticari beyaz boyaya göre ≥ 5 °C daha düşük olması |
| H4 | 6 aylık doğal yaşlanma sonunda güneş yansıtma kaybının ≤ 0,03 olması |
| H5 | m² başına malzeme maliyetinin piyasadaki ticari dış cephe/çatı boyası düzeyinde olması |
| H6 | En az 1 SCI/SCI-E makale, 1 ulusal/uluslararası bildiri, açık veri seti; faydalı model veya patent başvurusu değerlendirmesi |

## 11. Yöntem

### 11.1 Hammadde temini ve karakterizasyonu
- Farklı bölgelerden barit ve kalsit numunesi (maden işletmeleri ve MAPEG ruhsat sahipleriyle iletişim)
- **Mineraloji ve kimya:** XRD, XRF (özellikle Fe₂O₃, SrO, SiO₂, Al₂O₃)
- **Tane boyu:** Lazer difraksiyon; SEM ile tane şekli
- **Zenginleştirme denemeleri:** Yıkama, manyetik ayırma, eleme, bilyalı değirmende öğütme; her adımın maliyet ve yansıtma etkisi
- Referans olarak ticari yüksek saflıkta BaSO₄ ve CaCO₃

### 11.2 Boya formülasyonu
- Su bazlı akrilik bağlayıcı (ticari ulaşılabilirlik ve düşük UV soğurması nedeniyle); karşılaştırma için silikon/flor-akrilik bağlayıcı
- Değişkenler: **pigment hacim oranı** (%40-65), **tane boyu dağılımı** (tek boy ve karışık boy), **kaplama kalınlığı** (200-500 µm)
- Taguchi veya yanıt yüzeyi yöntemiyle deney tasarımı (DoE)
- Mekanik testler: yapışma (çapraz kesim), aşınma, esneklik

### 11.3 Optik ölçüm
- **Güneş yansıtması:** Entegre küreli UV-Vis-NIR spektrofotometre, 0,25-2,5 µm, AM1.5 ağırlıklı (ASTM E903 / G173)
- **Kızılötesi yayıcılık:** Altın kaplı entegre küreli FTIR, 2,5-25 µm; 8-13 µm ortalaması
- **Güneş Yansıtma İndeksi (SRI):** ASTM E1980
- Üniversite merkez laboratuvarı, ODTÜ MERLAB, UNAM veya hizmet alımı

### 11.4 Hızlandırılmış yaşlandırma
- UV + nem çevrimi (ASTM G154 / ISO 16474-3)
- Kirlenme simülasyonu ve yıkama testi
- Belirli aralıklarla spektral ölçüm tekrarı

### 11.5 İstanbul çatı saha testi
- Bir üniversite binası çatısında **yan yana test istasyonu**:
  - Yalıtımlı (ekstrüde polistiren) test kutuları, isteğe bağlı rüzgâr kalkanı (ince LDPE film), içlerinde boyalı alüminyum numune plakaları
  - Numuneler: çıplak çatı membranı, ticari beyaz boya, ithal saf BaSO₄ boya, yerli BaSO₄ boya, yerli CaCO₃ boya
- **Ölçümler (1 dk çözünürlük):** T tipi termokupl veya PT100 ile yüzey ve ortam sıcaklığı, piranometre (güneş ışınımı), pirgeometre (gökyüzü uzun dalga ışınımı, bütçe izin verirse), bağıl nem, rüzgâr hızı
- Veri toplama: datalogger veya ESP32 + MAX31865/ADS1115 tabanlı düşük maliyetli sistem
- **Küçük yapı ölçeği:** İki özdeş prefabrik test kabini (veya konteyner): biri ticari beyaz boya, biri yerli BaSO₄ boya ile kaplı; iç sıcaklık ve split klima enerji tüketimi ölçülür
- **Kampanyalar:** En az bir yaz (Haziran-Eylül) ve bir kış dönemi; kışın istenmeyen soğutma (ısıtma yükü artışı) de raporlanır

### 11.6 Modelleme ve bina enerji analizi
- Enerji dengesi modeli (Python, açık kaynak) saha verisiyle kalibre edilir
- Ölçülen R ve ε ile EnergyPlus (veya benzeri) üzerinden tipik İstanbul konutları, okullar ve sanayi yapıları için yıllık soğutma/ısıtma enerji analizi
- Tekno-ekonomik analiz: m² maliyeti, geri ödeme süresi, CO₂ tasarrufu

## 12. İş paketleri ve zaman planı (24 ay)

| İP | Adı | Aylar | Çıktı |
|---|---|---|---|
| İP1 | Hammadde temini, karakterizasyon ve zenginleştirme | 1-6 | Yerli pigment veri seti |
| İP2 | Boya formülasyonu ve DoE optimizasyonu | 4-11 | En iyi 2-3 formül |
| İP3 | Optik ve mekanik karakterizasyon | 5-12 | Spektral R ve ε verisi |
| İP4 | Saha test istasyonunun kurulması | 8-11 | Çalışan çatı istasyonu |
| İP5 | Uzun süreli saha testleri (yaz + kış) ve yaşlandırma | 11-22 | Saha performans ve kirlenme verisi |
| İP6 | Modelleme, bina enerji analizi, tekno-ekonomik analiz | 14-23 | Doğrulanmış model, tasarruf tahmini |
| İP7 | Yaygınlaştırma, makale, sonuç raporu | 18-24 | Makale, açık veri, rapor |

**1002-A / 2209-A (12 ay) için daraltılmış sürüm:** Ticari saf BaSO₄ ile 1 yerli barit ve 1 yerli kalsit numunesi; tek formül ailesi; tek yaz kampanyası ile çatı testi. Sonuçlar, sonraki 1001 başvurusu için ön veri olur.

## 13. Riskler ve B planları

| Risk | Olasılık | B planı |
|---|---|---|
| Yerli cevherde yüksek demir içeriği nedeniyle düşük yansıtma | Orta | Zenginleştirme adımları; karışık pigment (yerli + az miktarda saf); bu ilişkinin kendisi bir bulgudur |
| İstanbul neminde gündüz ortam altı soğutmanın sağlanamaması | Orta | Asıl karşılaştırma ölçütü ticari beyaz boyaya göre sıcaklık farkıdır; gece ve kuru günler ayrı raporlanır; nem etkisi modelle nicelleştirilir |
| Yüksek pigment oranında boyanın tozuması veya çatlaması | Orta | Pigment oranı ve bağlayıcı DoE ile dengelenir; üst kat şeffaf koruyucu kat denemesi |
| Kirlenmeyle hızlı performans kaybı | Yüksek | Aylık ölçüm ve yıkama deneyi; hidrofobik üst kat seçeneği; bulgu olarak raporlanır |
| FTIR/entegre küre erişimi | Orta | Merkez laboratuvar veya hizmet alımı; bütçeye hizmet alım kalemi |
| Kışın istenmeyen soğutma | Düşük-Orta | Kış verisi ayrıca raporlanır; yıllık net etki bina simülasyonuyla hesaplanır |

## 14. Bütçe kalemleri (tahmini kalem listesi)

Rakamlar başvuru anındaki güncel fiyatlarla hesaplanmalıdır.

- **Makine-teçhizat:** Datalogger ve sıcaklık sensörleri, piranometre, küçük meteoroloji istasyonu, bilyalı değirmen, laboratuvar karıştırıcı, film çekme aparatı, iki adet küçük test kabini ve enerji ölçerli split klima
- **Sarf malzemesi:** Akrilik bağlayıcı ve katkılar, ticari referans pigmentler, alüminyum numune plakaları, yalıtım malzemesi, ticari referans boyalar
- **Hizmet alımı:** XRD/XRF, SEM, lazer tane boyu, UV-Vis-NIR (entegre küre), FTIR (altın küre), hızlandırılmış yaşlandırma
- **Seyahat:** Maden sahalarından numune alımı, kongre katılımı
- **Bursiyer:** 1 lisansüstü, 1-2 lisans öğrencisi

## 15. Beklenen çıktılar ve yaygın etki

- **Bilimsel:** Yerli barit/kalsitin radyatif soğutma pigmenti olarak ilk veri seti; nemli kent ikliminde uzun süreli boya saha verisi; SCI makale(ler)
- **Teknolojik:** Yerli pigmentli soğutucu boya formülü; faydalı model/patent potansiyeli
- **Ekonomik:** Ham olarak ihraç edilen barit ve kalsite katma değer; yerli boya üreticileri için ürün fikri (1505, 1507 ile devam)
- **Toplumsal:** Okullar, hastaneler, depolar ve düşük gelirli konutlarda klimasız veya daha az klimayla serinlik; sıcak hava dalgalarına uyum
- **Çevresel:** Soğutma elektriğinde ve kentsel ısı adası etkisinde azalma; iklim değişikliğine uyum politikalarıyla uyum

## 16. Neden şimdi?

Sıcak hava dalgaları sıklaşıyor ve yaz elektrik tüketiminde klimanın payı artıyor. Radyatif soğutma boyaları laboratuvardan ticarileşmeye geçiş aşamasında. Türkiye'de bu konudaki çalışmalar ise ince film ve modelleme düzeyinde kalıyor. **Yerli hammadde + nemli iklimde saha testi** boşluğu, Türkiye'nin barit ve kalsit avantajı sayesinde güçlü bir özgünlük argümanı sunuyor. İlk adım olarak hızlı bir **1002-A** veya **2209-A** ile ön veri toplayıp ardından **1001** ile tam projeye geçmek önerilir.

## 17. Başvuru öncesi yapılacaklar listesi

- [ ] Güncel literatür taraması ve künyeli kaynak listesi (en az 30 kaynak); Türkiye'deki ~36 yayının sorgu ve tarih bilgisiyle tablosu
- [ ] Barit ve kalsit üreticileriyle iletişim; ön numune temini
- [ ] Laboratuvar erişim yazıları (UV-Vis-NIR entegre küre, FTIR, XRD/XRF)
- [ ] Çatı kullanım izni (bina yönetimi / rektörlük yapı işleri)
- [ ] Ekip: malzeme/kimya (formülasyon), makine/enerji (ısı transferi, bina simülasyonu), maden/jeoloji (cevher)
- [ ] Ticari saf BaSO₄ ile küçük bir ön deney: 2 numune, 1 hafta çatı ölçümü, fotoğraf ve grafik
- [ ] Güncel fiyat teklifleriyle bütçe
- [ ] Program çağrı takviminin kontrolü (1001 dönemleri, 1002-A ve 2209-A çağrıları)

## 18. Temel kaynaklar (künyeler başvurudan önce doğrulanmalıdır)

1. Raman, A. P., Anoma, M. A., Zhu, L., Rephaeli, E., Fan, S. (2014). Passive radiative cooling below ambient air temperature under direct sunlight. *Nature*, 515, 540-544.
2. Zhai, Y., Ma, Y., David, S. N., Zhao, D., Lou, R., Tan, G., Yang, R., Yin, X. (2017). Scalable-manufactured randomized glass-polymer hybrid metamaterial for daytime radiative cooling. *Science*, 355, 1062-1066.
3. Mandal, J., Fu, Y., Overvig, A. C., Jia, M., Sun, K., Shi, N. N., Zhou, H., Xiao, X., Yu, N., Yang, Y. (2018). Hierarchically porous polymer coatings for highly efficient passive daytime radiative cooling. *Science*, 362, 315-319.
4. Li, X., Peoples, J., Huang, Z., Zhao, Z., Qiu, J., Ruan, X. (2020). Full daytime sub-ambient radiative cooling in commercial-like paints with high figure of merit. *Cell Reports Physical Science*, 1, 100221.
5. Li, X., Peoples, J., Yao, P., Ruan, X. (2021). Ultrawhite BaSO₄ paints and films for remarkable daytime subambient radiative cooling. *ACS Applied Materials & Interfaces*, 13(18), 21733-21739.
6. Mandal, J., Yang, Y., Yu, N., Raman, A. P. (2020). Paints as a scalable and effective radiative cooling technology for buildings. *Joule*, 4, 1350-1356.
7. Berdahl, P., Martin, M. (1984). Emissivity of clear skies. *Solar Energy*, 32, 663-664. (Gökyüzü yayıcılığı modeli)
8. USGS Mineral Commodity Summaries (Barite) ve MAPEG / MTA maden istatistikleri (güncel yıl). (Türkiye üretim verileri)

---

*Bu doküman bir proje ön taslağıdır. Sayısal değerler (yansıtma, yayıcılık, sıcaklık farkları, hedefler) literatürdeki tipik değerlere dayanan tahminlerdir ve projede ölçülerek doğrulanacaktır. Etkileşimli sayfa (`radyatif-sogutma-boyasi.html`) bu dokümandaki enerji dengesi modelini kullanır.*
