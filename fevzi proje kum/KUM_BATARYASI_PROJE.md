# KUMSAL-EV: Türkiye'nin Yerel Kumlarıyla Ev Ölçeğinde Güneş Enerjili Kum Bataryası

**Önerilen proje adı:** Yerel Kum Türlerinin Termofiziksel Karakterizasyonu ve Doğrudan PV Beslemeli, Ev Ölçeğinde Bir Kum Bataryası Prototipinin Deneysel Performans Karşılaştırması

**Kısa ad:** KUMSAL-EV
**Alan:** Enerji depolama / Isıl enerji depolama (TES) / Yenilenebilir enerji
**Uygun TÜBİTAK programları:** 1001 (Bilimsel ve Teknolojik Araştırma Projeleri), 1002-A (Hızlı Destek), 3001 (Başlangıç Ar-Ge), lisans öğrencileri için 2209-A
**Önerilen süre:** 24 ay (1002-A için kapsam daraltılmış 12 aylık sürüm aşağıda)

---

## 1. Proje bir cümlede

Çatıdaki güneş panelinden gelen elektriği, inverter kullanmadan doğrudan bir direnç ısıtıcısıyla kuma aktarıp yüzlerce derecede depolayan, bu ısıyı akşam ve gece evin sıcak su ve ısıtma ihtiyacına geri veren **ev ölçeğinde bir kum bataryası** kurmak ve **Türkiye'nin beş farklı yerel kumunu aynı güneş koşulunda, yan yana ve eş zamanlı** test ederek hangisinin en iyi depolama malzemesi olduğunu deneysel olarak ortaya koymak.

## 2. Kum bataryası nedir, ne işe yarar?

Kum bataryası, elektrik yerine **ısı** depolayan bir duyulur ısı depolama (sensible heat storage) sistemidir.

1. **Şarj:** Fazla elektrik (güneş, rüzgâr ya da ucuz saat elektriği) yalıtımlı bir tank içindeki kumu ısıtır. Kum 300 ile 600 °C arasına kadar ısıtılabilir.
2. **Bekletme:** İyi yalıtılmış tankta kum ısıyı saatlerce, büyük sistemlerde haftalarca tutar.
3. **Deşarj:** Kumun içinden geçen hava ya da su borusu ısıyı alır; ev ısıtması, sıcak su veya proses ısısı olarak kullanılır.

**Neden kum?**

| Özellik | Kumun avantajı |
|---|---|
| Maliyet | Çok ucuz, yerel olarak her yerde var |
| Sıcaklık | Su 100 °C'de kaynar; kum 500 °C ve üstüne çıkabilir, birim hacimde çok daha fazla enerji tutar |
| Güvenlik | Yanmaz, zehirsiz, basınç gerektirmez |
| Ömür | Lityum pil gibi döngüyle bozulmaz |
| Çevre | Kritik mineral (lityum, kobalt) gerektirmez |

Temel denklem basittir: **Q = m · c<sub>p</sub> · ΔT**. Örneğin 1 m³ kum (yaklaşık 1.550 kg, c<sub>p</sub> ≈ 0,80 kJ/kg·K), 50 °C'den 400 °C'ye ısıtılırsa yaklaşık **120 kWh ısı** depolar. Bu, ortalama bir dairenin kışın birkaç günlük sıcak su ve ısıtma ihtiyacına denk gelir.

## 3. Güneş enerjisini neden lityum pil yerine kumda saklayalım?

Kısa cevap: **ihtiyaç ısıysa**, elektriği pilde saklayıp sonra ısıya çevirmek pahalı bir dolambaçtır. Kum bataryası güneş elektriğini hemen ısıya çevirir ve çok ucuz bir malzemede tutar. Ama her durumda kazanan değildir; özellikle ısı pompasıyla kıyaslandığında dürüst olmak gerekir.

### 3.1 Artı yönler (+)

| | Kum bataryası | Lityum (LFP) ev pili |
|---|---|---|
| **Depolama malzemesinin maliyeti** | Kumun kendisi kWh ısı başına 1 $'ın çok altında | Hücre ve sistem maliyeti kWh elektrik başına yüzlerce $ |
| **Tüm depo maliyeti (tahmini)** | Küçük ölçekte ~15-60 $/kWh ısı; MW ölçekte 10 $/kWh altı hedefleniyor | Kurulu ev sistemi ~300-600 $/kWh elektrik |
| **Ömür** | Kum döngüyle yıpranmaz; ısıtıcı ve metal parçalar değiştirilebilir, 20+ yıl | ~6.000 döngü, 10-15 yıl; kapasite zamanla düşer |
| **Güvenlik** | Yanmaz, termal kaçak (thermal runaway) yok | Düşük de olsa yangın riski, BMS zorunlu |
| **Kritik mineral** | Yok; tamamen yerel malzeme | Lityum, grafit, (bazı tiplerde) nikel/kobalt; ithal |
| **Yüksek sıcaklık** | 500 °C'ye kadar; radyatör (70-80 °C), sıcak su, kurutma, proses ısısı | Isıyı ancak elektrikli ısıtıcı veya ısı pompasıyla üretir |
| **Uzun süreli depolama** | Hacim büyüdükçe kayıp oranı düşer; günler hatta haftalar | Kendi kendine boşalma düşük ama kapasite pahalı |
| **Geri dönüşüm** | Sorunsuz | Özel geri dönüşüm süreci gerekir |
| **Şebekeden bağımsızlık** | İnvertersiz, doğrudan PV ile çalışabilir | İnverter, şarj kontrol ve BMS gerekir |

### 3.2 Eksi yönler (-)

| Eksi | Açıklama | Projede nasıl ele alınıyor |
|---|---|---|
| **Isı elektriğe kolay dönmez** | Isıdan tekrar elektrik (Stirling, ORC, termoelektrik) ancak %10-35 verimle mümkün. Işıklar, buzdolabı, TV için kum bataryası uygun değildir. | Sistem yalnızca **ısı ihtiyacı** için konumlanır; elektrik yükleri için küçük bir pil veya şebeke kalır. |
| **Isı pompasına göre güneş paneli ihtiyacı fazla** | Direnç ısıtıcı 1 kWh elektrikten 1 kWh ısı verir. Isı pompası ise 2,5-4 kWh ısı verir. Pil + ısı pompası aynı ısı için ~3 kat az PV ister. | Tekno-ekonomik analizde (İP6) bu seçenek açıkça karşılaştırılır. Kum, ısı pompasının zayıf kaldığı yerlerde öne çıkar: yüksek sıcaklık isteyen eski radyatörlü binalar, sıcak su, şebekesiz yerler, proses ısısı. |
| **Isı kaybı** | Kum soğur. Küçük tanklarda yüzey/hacim oranı büyük olduğu için kayıp yüksektir (bkz. Bölüm 4). | Kalın taş yünü + mikro gözenekli yalıtım, merkezde sıcak çekirdek tasarımı, kayıpların ölçülmesi. |
| **Mevsim uyumsuzluğu** | Isı ihtiyacı kışın en yüksek, güneş kışın en zayıf. Ev ölçeğinde kum bataryası günler boyunca depolar, aylarca değil. | Kış için PV fazla boyutlandırılır, yazın fazla ısı sıcak suya gider; gerekirse ucuz gece tarifesiyle destek. |
| **Hacim ve ağırlık** | 1 m³ kum ~1,5 ton; yalıtımla birlikte ~2 m³ yer kaplar. Çatı katı uygun değildir. | Bodrum, bahçe veya kazan dairesi yerleşimi; zemin taşıma kontrolü. |
| **Yavaş tepki** | Kumun ısıl iletkenliği düşük (~0,3 W/m·K); ısıyı hızlı çekmek zordur. | Serpantin aralığı ve hava/su akışı optimize edilir; yerel kumların iletkenliği zaten projede ölçülüyor. |
| **Yüksek sıcaklık güvenliği** | Dış yüzey ve bağlantılar sıcak olabilir. | Termostat, termal sigorta, kilitli muhafaza, dış yüzey sıcaklık sınırı. |

### 3.3 Hangi durumda hangisi?

- **Elektrik yükleri (aydınlatma, cihaz):** lityum pil.
- **Isı ihtiyacı, iyi yalıtılmış yeni bina, düşük sıcaklıklı yerden ısıtma:** ısı pompası (+ gerekirse küçük pil).
- **Isı ihtiyacı + yüksek sıcaklık (radyatör, sıcak su, kurutma, sera, proses), ucuz ve uzun ömürlü depolama, şebekesiz yer:** **kum bataryası**.
- En gerçekçi ev çözümü çoğu zaman **hibrittir:** küçük pil elektrik için, kum bataryası ısı için.

## 4. Kumu 500 °C'ye nasıl çıkarırız? Maliyet ve güneş ışığı açısından

### 4.1 Üç yol

| Yol | Nasıl çalışır | Ulaşılabilir sıcaklık | Güneş ışığı ihtiyacı | Maliyet ve karmaşıklık |
|---|---|---|---|---|
| **A. PV + direnç ısıtıcı** (önerilen) | Panel elektriği nikrom/kanthal ısıtıcıda ısıya döner (Joule ısınması). | Isıtıcı telleri 1.000 °C'nin üstüne dayanır; **sınır güneş değil, enerji dengesi ve yalıtımdır**. 500 °C rahatça mümkündür. | Toplam ışınım (doğrudan + dağınık). Bulutlu havada da azalan güçle çalışır. | En basit ve ucuz; hareketli parça yok, çatıdaki standart panel kullanılır. Dezavantaj: panel verimi ~%20-22, yani güneş ışığının ancak beşte biri ısıya döner. |
| **B. Yoğunlaştırılmış güneş (CSP)** | Fresnel mercek, parabolik çanak veya aynalar güneşi bir noktaya toplar, kumu doğrudan ısıtır. | 500-1.000 °C (düşen parçacık alıcıları ile) | Yalnızca **doğrudan ışınım**. Bulutlu havada neredeyse sıfır; güneş takip sistemi şart. | m² başına ~3 kat daha fazla ısı (optik verim ~%60-75), ama takip mekanizması, göz/yangın güvenliği ve bakım gerekir. Ev çatısı için zor. |
| **C. Vakum tüplü güneş kolektörü** | Güneş ısısını sıvıya/havaya aktarır. | Pratikte 150-250 °C; **500 °C'ye çıkamaz** | Toplam ışınım | Ucuz ve yaygın; ancak yalnızca ön ısıtma için kullanılabilir. |

**Sonuç:** Ev ölçeği için **A yolu (PV + direnç)** en uygunudur ve projede bu kullanılır. B yolu ileride ikinci bir proje konusu olabilir (ör. Konya/Karaman gibi doğrudan ışınımı yüksek bölgelerde).

### 4.2 500 °C'ye ulaşmanın asıl koşulu: enerji dengesi

Direnç ısıtıcıda kumun ulaşabileceği sıcaklığı güneşin "ne kadar sıcak" olduğu değil, **günlük gelen enerji ile yalıtımdan kaçan ısının dengesi** belirler:

- Kum, ısı kaybı günlük girişe eşitlenene kadar ısınır: **T<sub>denge</sub> ≈ T<sub>ortam</sub> + (günlük ortalama güç) / (UA)**
- UA: tankın ısı kayıp katsayısı (yalıtım kalınlığı ve yüzey alanına bağlı).
- Küçük tankta yüzey/hacim oranı büyük olduğu için kayıp görece yüksektir; büyük tank daha verimlidir (Finlandiya tesislerinin büyük olmasının nedeni budur).

**Basit modelle hesaplanan örnekler** (Karapınar kumu, silindir tank, taş yünü yalıtımın iletkenliği sıcaklıkla artırılarak, deşarj yok, PV-doğrudan verim %85):

| Senaryo | Ocak (3,0 tepe güneş saati) | Temmuz (7,3 tepe güneş saati) | 500 °C'de günlük kayıp |
|---|---|---|---|
| 40 L test hücresi, 15 cm yalıtım, 1 panel (0,4 kWp) | En fazla ~220 °C | En fazla ~460 °C | ~3,4 kWh |
| 40 L test hücresi, 30 cm yalıtım, 1 panel (0,4 kWp) | En fazla ~355 °C | ~3,6 günde 500 °C | ~1,8 kWh |
| 0,3 m³ tank, 30 cm yalıtım, 3 kWp | ~14 günde 500 °C | ~3,4 günde 500 °C | ~6,5 kWh |
| 0,8 m³ tank, 15 cm yalıtım, 3 kWp | En fazla ~210 °C | En fazla ~430 °C | ~24 kWh |
| 0,8 m³ tank, 30 cm yalıtım, 3 kWp | En fazla ~350 °C | ~11 günde 500 °C | ~13 kWh |
| 0,8 m³ tank, 30 cm yalıtım, 6 kWp | ~17 günde 500 °C | ~4,4 günde 500 °C | ~13 kWh |

**Bu tablodan çıkan tasarım kuralları:**
1. **Yalıtım her şeydir.** 15 cm'den 30 cm'ye çıkmak kaybı yaklaşık yarıya indirir. 500 °C hedefi için en az 25-30 cm taş yünü veya ince bir mikro gözenekli yalıtım katmanı (yüksek sıcaklıkta iletkenliği taş yününün yarısından az) gerekir.
2. **PV gücü / kum hacmi oranı** belirleyicidir. Ev ölçeğinde kabaca **m³ başına 8-10 kWp** PV, 500 °C'yi yaz aylarında birkaç günde mümkün kılar. Kışın aynı sistem 300-350 °C civarında dengelenebilir.
3. **Test hücreleri için tek panel yetmez.** 500 °C karşılaştırması için hücre başına ~0,8 kWp (2 panel) veya 30 cm yalıtım planlanmalıdır. Bu, İP2 tasarımına yansıtılacaktır.
4. **500 °C'yi sürekli tutmak pahalıdır.** Günlük işletme için 150-400 °C bandı daha ekonomiktir; 500 °C yaz fazlasını depolamak ve kumların üst sınır testleri için kullanılır.
5. **Sıcak çekirdek tasarımı:** Isıtıcıları tankın merkezinde toplayıp çekirdeği 500 °C'ye, dış kabuğu daha düşük sıcaklığa çıkarmak yüzey kaybını azaltır. Bu tabakalaşmanın ölçülmesi, projenin özgün deney çıktılarından biridir.

### 4.3 Güneş ışığı açısından Türkiye

- Türkiye'de yıllık PV üretimi bölgeye göre kabaca **1.200-1.650 kWh/kWp** arasındadır (Karadeniz düşük; İç Anadolu, Akdeniz ve Güneydoğu yüksek). Kesin değerler PVGIS'ten il bazında alınacaktır.
- Kış aylarında (Aralık-Ocak) günlük tepe güneş saati çoğu bölgede **2-3 saate**, yazın **7 saatin üstüne** çıkar. Yani aynı sistem yazın kışın yaklaşık 2,5-3 katı enerji toplar.
- **Isı ihtiyacı ile güneşin ters mevsimde olması** sistemin en büyük zayıflığıdır. Çözümler: PV'yi kış ihtiyacına göre büyütmek (yazın fazla ısı sıcak su ve kurutma için kullanılır), sistemi tam ısıtma değil **ısıtmaya katkı + sıcak su** olarak konumlamak, uygun tarifede gece elektriğiyle destek.
- PV + direnç yolu **dağınık ışınımla da** çalıştığı için bulutlu günlerde tamamen durmaz; CSP ise durur. Bu da Karadeniz gibi bulutlu bölgelerde PV yolunu tek seçenek yapar.

### 4.4 Maliyet açısından kaba karşılaştırma (günde 10 kWh ısı, ocak ayı)

> Rakamlar 2026 için **tahmini aralıklardır** (USD, TL kur etkisinden kaçınmak için). Proje bütçesi güncel tekliflerle yeniden hesaplanmalıdır. Varsayımlar: PV kurulu maliyeti ~0,5-0,9 $/Wp, LFP ev pili ~300-600 $/kWh, ocakta 3,0 tepe güneş saati.

| Seçenek | Gereken PV | Depolama | Diğer | Toplam (kaba) |
|---|---|---|---|---|
| **A. PV + Li-ion pil (11 kWh) + elektrikli ısıtıcı** | ~4 kWp | 3.300-6.600 $ | Isıtıcı (düşük) | ~5.000-10.000 $ |
| **B. PV + Li-ion pil (4 kWh) + ısı pompası** | ~1,5 kWp | 1.200-2.400 $ | Isı pompası 3.000-6.000 $ | ~5.000-9.500 $ |
| **C. PV + kum bataryası (0,3 m³)** | ~5 kWp | 1.000-2.000 $ (tank, yalıtım, ısıtıcı, serpantin) | İnverter yok | ~3.500-6.500 $ |

**Okuma:**
- Kum bataryası, **pil + elektrikli ısıtıcıdan açıkça daha ucuzdur** ve depo ömrü çok daha uzundur.
- **Pil + ısı pompası** ile toplam maliyet benzer aralıktadır; ısı pompası daha az panel ister ama kompresör bakımı, yüksek sıcaklıkta düşen verim ve bina uygunluğu gerektirir. Kum ise daha fazla panel ister ama daha basit ve daha uzun ömürlüdür.
- Kumun en büyük ekonomik avantajı **depolama kapasitesini büyütmenin ucuz olmasıdır:** kapasiteyi ikiye katlamak pilde maliyeti ikiye katlar, kumda ise yalnızca biraz daha kum, tank ve yalıtım ister.
- Bu karşılaştırmanın deneysel verilerle yapılması, projenin İP6 çıktısıdır.

## 5. Isı pompasıyla karşılaştırma ve farklı bina türleri

Hakemin soracağı en güçlü soru şudur: *"Neden kum? Isı pompası aynı ısıyı üç kat az elektrikle üretiyor."* Bu bölüm bu soruyu açıkça cevaplar. Kısa cevap: **ocak ayında enerji verimliliğinde ısı pompası kazanır; kum ise ucuz ve uzun süreli depolamada, yüksek sıcaklıkta, zayıf şebekede ve büyük ölçekte öne çıkar. Çoğu bina için en iyi cevap hibrittir.**

### 5.1 Isı pompası ve kum bataryası: temel farklar

| Ölçüt | Hava kaynaklı ısı pompası | Kum bataryası (PV + direnç) |
|---|---|---|
| **1 kWh elektrikten elde edilen ısı** | 1,8-4,5 kWh (COP). Dış hava soğudukça ve su sıcaklığı yükseldikçe düşer. | 1 kWh (COP = 1), dış havadan bağımsız |
| **Tipik COP değerleri** | Yerden ısıtma (35 °C), +7 °C dışarıda: ~4. Radyatör (55 °C), -7 °C: ~2-2,5. Eski radyatör (70 °C) veya -15 °C altı: ~1,8-2,2 | Sabit 1 |
| **Zamanı kaydırma (depolama)** | Kendi başına depolamaz. Gece ısıtması için pil, şebeke veya su deposu gerekir. | Depolamanın kendisidir; öğlen güneşi gece ısıya döner |
| **Çıkış sıcaklığı** | Yükseldikçe verim düşer; 70 °C üstü özel cihaz ister | Kum sıcaklığına kadar her sıcaklık (500 °C'ye kadar) |
| **Hacim başına depolama** | Su deposu ile: ~20-45 kWh/m³ (20-40 K kullanılabilir fark) | ~120-170 kWh/m³ (yaklaşık 4-6 kat yoğun) |
| **Şebeke bağlantısı** | 5-10 kW'lık kompresör için güçlü bağlantı | İnvertersiz, şebekesiz çalışabilir |
| **Hareketli parça, bakım** | Kompresör, fan, soğutucu akışkan; 15-20 yıl | Yok (yalnızca ısıtıcı ve fan/pompa); kum ömür boyu |
| **İlk yatırım** | Cihaz ~500-800 $/kW + kurulum | Depo düşük; ama aynı ısı için daha fazla PV |
| **Gürültü ve dış ünite** | Dış ünite gerekir; apartmanlarda izin ve gürültü sorunu | Sessiz, içeride (bodrum, kazan dairesi, bahçe) |

**Dürüst sonuç:** Isı pompasının zayıf kaldığı üç durum, kumun güçlü olduğu üç durumla örtüşür: **yüksek çıkış sıcaklığı**, **elektriğin olmadığı saatlerde ısı ihtiyacı (depolama)** ve **zayıf/olmayan şebeke**. Ayrıca düşük sıcaklıkta depolama gerekiyorsa ısı pompası + su deposu, kumun doğrudan rakibidir; kum burada ancak hacim (4-6 kat yoğunluk) ve çok günlük depolama ile ayrışır.

### 5.2 Yedi farklı bina için senaryo karşılaştırması

**Yöntem (basit, tahmini model):** Ocak ayı, aynı çatı/arazi PV kapasitesi her iki seçenekte de kullanılır. Isı pompasında güneş elektriği COP ile çarpılır, gece payı pilden karşılanır. Kumda güneş elektriği direnç ile kuma gider; depo verimi küçük sistemde %75, büyük sistemde %85. Karşılanamayan kısım şebekeden alınır (ısı pompasında COP ile, kumda direnç/gece tarifesi ile). Maliyetler bölüm 4.4'teki varsayımlarla, USD, kaba aralıktır.

| Bina | Ocak ısı ihtiyacı | Çıkış sıcaklığı / COP | Kullanılabilir PV | Isı pompası: güneş payı / şebeke | Kum: güneş payı / şebeke | İlk yatırım: ısı pompası (+pil +PV) | İlk yatırım: kum (+PV) |
|---|---|---|---|---|---|---|---|
| **1. Yeni yalıtımlı müstakil ev** (yerden ısıtma) | 25 kWh/gün | 35 °C / 3,5 | 8 kWp | %100 / 0 kWh | %61 / 9,7 kWh | 5.400-9.500 $ | 4.400-8.200 $ |
| **2. Eski apartman dairesi** (radyatör) | 40 kWh/gün | 70 °C / 2,2 | 1,5 kWp (çatı payı) | %21 / 14,4 kWh | %7 / 37 kWh | 4.100-7.000 $ | 800-1.500 $ |
| **3. Köy evi** (sobalı, şebeke zayıf) | 45 kWh/gün | 60 °C / 2,5 | 10 kWp (arazi) | %100 / 0 kWh (12,6 kWh pil ile) | %43 / 26 kWh (sobadan) | 9.800-17.900 $ | 5.500-10.200 $ |
| **4. Soğuk iklim müstakil** (Erzurum) | 70 kWh/gün | 55 °C, -15 °C dış / 1,9 | 8 kWp | %65 / 13 kWh | %26 / 52 kWh | 12.600-23.000 $ | 4.500-8.300 $ |
| **5. Küçük sera** (200 m², gece ısıtma) | 60 kWh/gece | 40 °C / 3,0 | 15 kWp | %100 / 0 kWh (20 kWh pil ile) | %48 / 31 kWh | 13.000-24.100 $ | 8.500-15.900 $ |
| **6. Okul** (gündüz kullanım) | 300 kWh/gün | 55 °C / 2,8 | 40 kWp | %95 / 5 kWh | %29 / 213 kWh | 44.800-79.400 $ | 20.600-37.500 $ |
| **7. Apartman bloğu, merkezi kazan** (20 daire) | 600 kWh/gün | 70 °C / 2,2 | 25 kWp | %23 / 209 kWh | %9 / 546 kWh | 57.100-99.300 $ | 13.200-24.200 $ |

> Kum sütunundaki ilk yatırım, yalnızca güneşten gelen payı depolayacak kadar depo içerir. Şebeke sütunu ocak ayında günlük ek elektrik ihtiyacıdır; kumda bu, ucuz saat tarifesiyle kuma depolanabilir.

### 5.3 Bina bina karar

1. **Yeni yalıtımlı müstakil ev → Isı pompası.** Düşük sıcaklıklı yerden ısıtmada COP yüksek; ocakta bile 8 kWp ile tamamen güneşten karşılanabilir. Kum yalnızca isteğe bağlı: yaz fazlasını sıcak suya çevirmek için küçük bir depo.
2. **Eski apartman dairesi → Isı pompası veya bina ölçeğinde çözüm.** Çatı payı çok küçük, iki seçenek de güneşten az pay alır. Tek bir daireye ~1 ton kum ve yalıtım koymak döşeme yükü ve yer açısından uygun değil. Doğru ölçek bina ölçeğidir (madde 7).
3. **Köy evi → Kum + mevcut soba (hibrit).** Kâğıt üzerinde ısı pompası daha fazla güneş payı veriyor ama 12,6 kWh pil, güçlü şebeke bağlantısı ve kesintisiz elektrik ister. Kum invertersiz ve şebekesiz çalışır, ocakta ısının ~%40'ını, baharda ve yazın sıcak suyun tamamını karşılar; odun/kömür tüketimini ve hava kirliliğini azaltır. **Projenin en güçlü kullanım alanlarından biri.**
4. **Soğuk iklim (Erzurum) → Hibrit.** -15 °C'de ısı pompası COP'si ~1,9'a düşer ve pahalı bir pil gerekir. Isı pompası baz yükü, kum ise soğuk dalgalarda tepe yükü ve sıcak suyu karşılar. Doğu Anadolu'da kış güneşi ve kar yansıması PV üretimini destekler (projede ölçülecek).
5. **Sera → Kum (veya ısı pompası + kum).** Isı ihtiyacının tamamı gece; ısı pompası 20 kWh pil ister. Kum gece ısısını ucuza depolar, sıcak havayı doğrudan kum yatağından üfleyerek verir; arazi ve hacim sorunu yok.
6. **Okul → Isı pompası.** Kullanım gündüz, güneşle çakışıyor; çok az depolama gerekir. Kum yalnızca hafta sonu PV'siyle pazartesi sabahı binayı ön ısıtmak için küçük bir depo olarak anlamlı.
7. **Apartman bloğu, merkezi kazan → Hibrit; kumun en mantıklı olduğu büyük ölçek.** Kazan dairesinde yer var, büyük tankta yüzey/hacim oranı küçük olduğu için kayıp düşük, 70 °C radyatör sıcaklığı ısı pompasını zorlar. Çatı ihtiyacın ancak ~%10-25'ini karşılar; kum depo gece/ucuz saat elektriğiyle de şarj edilerek doğal gaz kazanının tepe yükünü azaltır.

### 5.4 Projeye yansıması

- **İP6 tekno-ekonomik analiz** bu yedi bina tipini (ve 81 il iklim verisini) temel senaryo seti olarak kullanır; deneyle doğrulanmış modelle yeniden hesaplanır.
- **Ev ölçeği prototip (İP5)** köy evi / müstakil ev senaryosuna göre tasarlanır: invertersiz PV, radyatör veya sıcak hava çıkışı, mevcut soba/kazanla hibrit çalışma.
- Isı pompası ile **gerçek ölçüm karşılaştırması** için, bütçe izin verirse prototip yanına küçük bir hava kaynaklı ısı pompası + su deposu kurulup aynı günlerde ölçülmesi önerilir (hakemler için güçlü bir kanıt olur).

## 6. Problem ve motivasyon

- Türkiye'de konut enerji tüketiminin büyük kısmı **ısınma ve sıcak su** içindir ve bu ihtiyaç ağırlıkla doğal gaz ile karşılanır. Doğal gazın büyük bölümü ithaldir.
- Çatı GES'leri hızla yayılıyor, ancak güneş öğlen bol, ihtiyaç ise akşam ve gece yüksek. Lityum piller pahalı ve elektriği **ısıya** çevirmek için aşırı karmaşık bir çözüm.
- Ev ölçeğinde, ucuz, yerel malzemeyle yapılan bir ısı bataryası bu zaman uyumsuzluğunu çözebilir.

## 7. Literatür durumu ve boşluk

**Dünyada:**
- Finlandiya'da Polar Night Energy firması Kankaanpää (2022) ve Pornainen (2025) kentlerinde MW ölçekli, şehir ısıtma şebekesine bağlı kum/taş bataryaları işletmektedir. Bunlar **endüstriyel ölçeklidir**.
- 2025-26 döneminde güneş enerjili kum bataryası, kum depolamalı PV su ısıtıcısı ve kum ısısıyla çalışan yaklaşık 1 kW'lık Stirling motoru prototipi gibi **deneysel çalışmalar** yayımlanmıştır. Konu hızla ivme kazanmaktadır.

**Türkiye'de:**
- Tespit edilen yaklaşık 5 çalışma, ağırlıkla **sayısal modelleme** (akışkan yatak) veya **çok-üretimli (poligenerasyon) sistem analizi** düzeyindedir.
- **Ev ölçeğinde gerçek bir deney yoktur.**
- **Türkiye'nin yerel kum türlerinin** depolama malzemesi olarak karşılaştırmalı karakterizasyonu yoktur.

> **Not:** Başvuru öncesinde Web of Science, Scopus, ULAKBİM TR Dizin ve YÖK Tez veri tabanlarında "sand battery", "sand thermal energy storage", "kum ısıl enerji depolama" anahtar kelimeleriyle güncel tarama yapılmalı ve bu bölümdeki her iddia künyeli kaynakla desteklenmelidir.

## 8. Özgün değer (projeyi farklı kılan 5 nokta)

1. **Üçüz/beşiz hücre test düzeneği:** Beş yerel kum, aynı PV dizisinden eşit güç alan beş özdeş küçük hücrede **eş zamanlı** test edilir. Böylece hava durumu, ışınım ve ortam sıcaklığı farkı ortadan kalkar; karşılaştırma gerçek anlamda adil olur. Literatürde kumlar genellikle farklı günlerde ya da yalnızca laboratuvar fırınında karşılaştırılmaktadır.
2. **Yerel kumların termofiziksel kataloğu:** Türkiye'nin farklı jeolojik kökenli kumları için özgül ısı, ısıl iletkenlik, yığın yoğunluğu, tane boyu dağılımı ve **yüzlerce ısıl döngü sonrası bozunma** (sinterleşme, topaklanma, kalsinasyon) ilk kez tek bir çalışmada ölçülür.
3. **İnvertersiz doğrudan PV-ısıtıcı bağlantısı:** PV panel çıkışı, panel karakteristiğine uygun seçilmiş direnç ile doğrudan ısıtıcıya bağlanır (inverter ve şebeke yok). Bu, sistem maliyetini düşürür ve kırsal/şebekeden bağımsız kullanım imkânı sağlar. Basit bir yük eşleştirme (direnç kademesi seçimi) stratejisi geliştirilir ve verimi ölçülür.
4. **Deneyle doğrulanmış açık kaynak model:** Basit 1B/2B ısıl model deney verisiyle kalibre edilir ve açık kaynak olarak yayımlanır. Model, PVGIS ışınım verisi ile birleştirilerek **Türkiye'nin 81 ili için uygunluk haritası** çıkarılır.
5. **Ev ölçeği tekno-ekonomik analiz:** Doğal gaz, ısı pompası ve lityum pil + elektrikli ısıtıcı alternatifleriyle karşılaştırmalı maliyet ve geri ödeme analizi yapılır.

## 9. Karşılaştırılacak aday yerel kumlar

| # | Kum | Bölge | Baskın mineral | Neden seçildi | Dikkat edilecek nokta |
|---|---|---|---|---|---|
| K1 | Şile kuvars kumu | İstanbul / Marmara | Kuvars (SiO₂) | Sanayide yaygın, saf, referans malzeme | 573 °C'de kuvars faz geçişi (hacim değişimi) |
| K2 | Karapınar kumul kumu | Konya / İç Anadolu | Kuvars + feldspat | Bol, ucuz, güneşi en yüksek bölgede | Tane şekli, toz içeriği |
| K3 | Kıyı (kalkerli) kumu | Antalya / Akdeniz | Kalsit (CaCO₃) + kuvars | Kıyı bölgelerde kolay erişim | ~600 °C üzeri kalsinasyon riski; üst sıcaklık sınırı belirlenmeli |
| K4 | Bazaltik volkanik kum | Kula (Manisa) / Ege | Bazaltik cam, piroksen | Yüksek sıcaklık dayanımı, koyu renk | Gözeneklilik, nem tutma |
| K5 | Magnetitli kara kum | Doğu Karadeniz kıyıları | Magnetit (Fe₃O₄) + silikatlar | Yüksek yoğunluk, yüksek hacimsel ısı kapasitesi beklentisi | Yüksek sıcaklıkta oksitlenme |

> Kesin numune alım noktaları, izinler ve mineralojik doğrulama (XRD/XRF) İP1'de yapılır. Tablodaki özellikler **beklentidir**; asıl değerler projede ölçülecektir.

## 10. Amaç ve hedefler

**Ana amaç:** Yerel kumların depolama malzemesi olarak performansını deneysel olarak karşılaştırmak ve ev ölçeğinde, doğrudan PV beslemeli bir kum bataryası prototipinin gerçek dış ortam koşullarındaki performansını ortaya koymak.

**Ölçülebilir hedefler (başarı ölçütleri):**

| Hedef | Ölçüt |
|---|---|
| H1 | 5 kum türünün c<sub>p</sub> (25-600 °C), k, ρ değerlerinin ölçülmesi, belirsizlik analiziyle |
| H2 | Her kum için en az 100 ısıl döngü sonrası özellik değişiminin raporlanması |
| H3 | ~0,5-1 m³'lük prototipte ≥ 300 °C şarj sıcaklığına ulaşılması |
| H4 | 24 saatlik bekleme sonunda depolanan enerjinin ≥ %70'inin korunması (hedef değer) |
| H5 | Isıl modelin deney verisini ±%10 içinde öngörmesi |
| H6 | En az 1 SCI/SCI-E makale, 1 ulusal/uluslararası bildiri, açık veri seti ve açık kaynak model |

## 11. Yöntem

### 11.1 Malzeme karakterizasyonu (laboratuvar)
- **Mineraloji:** XRD, XRF
- **Tane boyu:** Elek analizi / lazer difraksiyon
- **Özgül ısı:** DSC (diferansiyel taramalı kalorimetri), 25-600 °C
- **Isıl iletkenlik:** Geçici sıcak tel (transient hot wire) veya hot-disk yöntemi
- **Yığın yoğunluğu ve gözeneklilik**
- **Isıl döngü dayanımı:** Kül fırınında 100+ döngü, ardından SEM görüntüleme ve özelliklerin yeniden ölçümü
- **Termogravimetri (TGA):** Kalsinasyon ve kütle kaybı sınırlarının belirlenmesi

### 11.2 Beşiz hücre deney düzeneği (dış ortam)
- 5 özdeş paslanmaz çelik hücre (her biri ~30-50 L), en az 25-30 cm taş yünü + seramik elyaf / mikro gözenekli yalıtım
- Her hücrede eşit güçte direnç ısıtıcı, her ısıtıcı ~0,8 kWp'lik (2 panel) özdeş PV dizisine doğrudan bağlı (500 °C'ye ulaşabilmek için; bkz. Bölüm 4.2)
- Her hücrede yükseklik ve yarıçap boyunca **en az 9 K-tipi termokupl**
- Piranometre, ortam sıcaklığı, rüzgâr hızı, PV akım ve gerilim ölçümü
- Veri toplama: 1 dakikalık çözünürlük (datalogger veya Arduino/ESP32 + MAX31856 tabanlı düşük maliyetli sistem)
- Deşarj: hücre içinden geçen bakır serpantinde sabit debili su; giriş/çıkış sıcaklığı ve debi ölçülür

### 11.3 Ev ölçeği prototip
- İP2 ve İP4 sonuçlarına göre seçilen **en iyi kum** ile ~0,5-1 m³ tank
- 2-3 kWp PV dizisi, doğrudan direnç bağlantısı, kademeli yük eşleştirme
- Deşarj: sıcak su boyleri ve/veya fan-coil üzerinden oda ısıtması
- **Yaz ve kış kampanyaları**: mevsimsel performans farkını görmek için en az 2 ölçüm dönemi

### 11.4 Sayısal model ve analiz
- Toplu (lumped) ve 1B/2B sonlu farklar ısıl modeli (Python, açık kaynak)
- Deneysel veriyle kalibrasyon ve doğrulama
- PVGIS ışınım verisi ile 81 il için yıllık simülasyon ve uygunluk haritası
- Tekno-ekonomik analiz: seviyelendirilmiş ısı maliyeti (LCOH), geri ödeme süresi, CO₂ tasarrufu

## 12. İş paketleri ve zaman planı (24 ay)

| İP | Adı | Aylar | Çıktı |
|---|---|---|---|
| İP1 | Kum tedariki ve laboratuvar karakterizasyonu | 1-7 | Kum özellik kataloğu (veri seti) |
| İP2 | Hücre ve prototip tasarımı, ön modelleme | 3-8 | Tasarım raporu, ilk model |
| İP3 | Beşiz hücre düzeneğinin imalatı ve devreye alınması | 6-10 | Çalışan test düzeneği |
| İP4 | Karşılaştırmalı dış ortam deneyleri (yaz + kış) | 9-18 | Kum performans sıralaması |
| İP5 | Ev ölçeği prototip imalatı ve deneyleri | 12-21 | Prototip performans verisi |
| İP6 | Model doğrulama, il haritası, tekno-ekonomik analiz, yaygınlaştırma | 16-24 | Makale, açık kaynak model, sonuç raporu |

**1002-A (12 ay) için daraltılmış sürüm:** İP1 (3 kum ile) + İP3 + İP4 (tek mevsim). Ev ölçeği prototip sonraki 1001 başvurusuna bırakılır; 1002-A sonuçları 1001 için ön veri olur.

## 13. Riskler ve B planları

| Risk | Olasılık | B planı |
|---|---|---|
| Kalkerli kumun yüksek sıcaklıkta bozunması | Yüksek | Üst sıcaklık TGA ile belirlenir, K3 düşük sıcaklık (≤ 500 °C) sınıfında test edilir; bu da bir bulgudur |
| Kuvarsın 573 °C faz geçişiyle tank zorlanması | Orta | Maksimum sıcaklık 550 °C ile sınırlanır |
| DSC/hot-disk cihazına erişim | Orta | Üniversite merkez laboratuvarı veya hizmet alımı; bütçeye hizmet alım kalemi eklenir |
| Kış aylarında düşük ışınım | Orta | Düşük ışınım verisi de sonuçtur; ayrıca laboratuvar güç kaynağıyla kontrollü şarj deneyleri yapılır |
| Yüksek sıcaklık güvenliği | Düşük | Termostat ve termal sigorta, kilitli muhafaza, yangın riski değerlendirmesi |

## 14. Bütçe kalemleri (tahmini kalem listesi)

Rakamlar başvuru anındaki güncel fiyatlarla hesaplanmalıdır.

- **Makine-teçhizat:** Datalogger ve termokupllar, piranometre, PV paneller, direnç ısıtıcılar, debimetre, kül fırını (döngü testi)
- **Sarf malzemesi:** Paslanmaz çelik sac/tank, taş yünü ve seramik elyaf yalıtım, bakır boru, kablo ve bağlantı elemanları, kum numuneleri ve nakliyesi
- **Hizmet alımı:** XRD/XRF, DSC, TGA, SEM, ısıl iletkenlik ölçümleri
- **Seyahat:** Kum numune alımı (5 bölge), kongre katılımı
- **Bursiyer:** 1 lisansüstü, 1-2 lisans öğrencisi

## 15. Beklenen çıktılar ve yaygın etki

- **Bilimsel:** Türkiye'nin yerel kumları için ilk karşılaştırmalı termofiziksel veri seti; deneyle doğrulanmış açık kaynak model; SCI makale(ler)
- **Teknolojik:** İnvertersiz, düşük maliyetli ev tipi kum bataryası tasarımı; faydalı model/patent başvurusu potansiyeli
- **Ekonomik:** Doğal gaz ithalatına bağımlılığı azaltacak yerel bir çözüm; KOBİ'ler için üretilebilir ürün fikri (3001/1507 ile devam)
- **Toplumsal:** Kırsal ve şebekeden uzak yerleşimler, seralar, kümesler için ucuz ısı depolama
- **Çevresel:** Kritik mineral gerektirmeyen, geri dönüşümü sorunsuz depolama

## 16. Neden şimdi?

Konu dünyada hızla ısınıyor: 2025-26'da deneysel ev/küçük ölçek çalışmaları yayımlanmaya başladı. Türkiye'deki mevcut çalışmalar ise henüz sayısal düzeyde. **Ev ölçeğinde deney + yerel kum karşılaştırması** boşluğu kısa süre içinde başka gruplarca doldurulabilir. Bu yüzden ilk adım olarak hızlı bir **1002-A** başvurusuyla ön veri toplamak, ardından **1001** ile tam projeye geçmek önerilir.

## 17. Başvuru öncesi yapılacaklar listesi

- [ ] Güncel literatür taraması ve künyeli kaynak listesi (en az 30 kaynak)
- [ ] Kum numune bölgelerinin kesinleştirilmesi ve ön numune alımı
- [ ] Laboratuvar erişim yazıları (DSC, XRD, TGA)
- [ ] Ekip: elektrik/elektronik (PV ve veri toplama), makine (ısı transferi), jeoloji/maden (kum karakterizasyonu)
- [ ] Basit bir ön deney (örneğin 20 L'lik tek hücre) ile fotoğraf ve ön veri
- [ ] Güncel fiyat teklifleriyle bütçe
- [ ] Program çağrı takviminin kontrolü (1001 dönemleri, 1002-A sürekli açık)

---

*Bu doküman bir proje ön taslağıdır. Sayısal değerler (özgül ısı, yoğunluk, hedef verimler) literatürdeki tipik değerlere dayanan tahminlerdir ve projede ölçülerek doğrulanacaktır.*
