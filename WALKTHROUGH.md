# Mechanism Master — Walkthrough (Geliştirici Referansı)

Her seviyenin hedef parametre değerleri aşağıdadır.  
**r₁** sabittir (oyuncu değiştiremez). Diğer beş parametre slider ile ayarlanır.  
**α** değerleri slider'da derece (°) olarak gösterilir.

---

## Seviye Listesi

| No | TR Adı | EN Adı | r₁ | r₂ | r₃ | r₄ | Lp | α (°) |
|----|--------|--------|-----|-----|-----|-----|-----|--------|
| 01 | Daire | Circle | 200 | 70 | 220 | 220 | 110 | 0° |
| 02 | Yumurta | Egg | 220 | 60 | 200 | 240 | 130 | 29° |
| 03 | Sekiz | Figure 8 | 240 | 95 | 200 | 180 | 210 | 32° |
| 04 | Yay | Arc | 200 | 50 | 240 | 180 | 150 | 57° |
| 05 | Fasulye | Bean | 220 | 80 | 180 | 220 | 190 | 46° |
| 06 | Yengeç | Crab | 260 | 75 | 200 | 220 | 240 | −43° |
| 07 | Elips | Ellipse | 200 | 80 | 240 | 180 | 90 | 74° |
| 08 | Çiçek | Flower | 220 | 90 | 180 | 220 | 230 | 29° |
| 09 | Kalp | Heart | 230 | 85 | 165 | 215 | 195 | −34° |
| 10 | Damla | Teardrop | 210 | 70 | 230 | 190 | 160 | 17° |
| 11 | Köpekbalığı | Shark | 260 | 70 | 235 | 190 | 220 | −52° |
| 12 | Yaprak | Leaf | 210 | 65 | 205 | 195 | 170 | 63° |
| 13 | Dümen | Helm | 250 | 105 | 190 | 180 | 215 | 43° |
| 14 | Hilal | Crescent | 200 | 55 | 255 | 185 | 140 | −63° |
| 15 | Kelebek | Butterfly | 250 | 120 | 200 | 180 | 240 | 11° |

---

## Seviye Notları

**01 — Daire (Circle)**  
En kolay giriş seviyesi. r₃ = r₄ ve α = 0° simetrisi nedeniyle coupler noktası daireye yakın bir yol çizer. r₂ değeri küçük tutularak düzgün rotasyon sağlanır.

**02 — Yumurta (Egg)**  
Daireden biraz daha uzun, asimetrik oval. α = 29° ile coupler noktası eksenden hafifçe kaydırılmıştır.

**03 — Sekiz (Figure 8)**  
Büyük Lp (210) ve yakın r₃/r₄ oranı birlikte çift döngü üretir. Grashof marjı 45 ile orta zorlukta.

**04 — Yay (Arc)**  
r₃ uzun (240), r₄ kısa (180) asimetrik yapı geniş yay eğrisi verir. α = 57° coupler noktasını üst konuma taşır.

**05 — Fasulye (Bean)**  
Lp = 190 ile coupler noktası büyük bir fasulye şekli çizer. α = 46° asimetriyi belirler.

**06 — Yengeç (Crab)**  
Negatif α (−43°) coupler noktasını aşağıya iter; büyük Lp ile yengeç pençesine benzer girintili eğri oluşur.

**07 — Elips (Ellipse)**  
Küçük Lp (90) ile yakın pivot noktası, büyük α (74°) ile dikeysel uzama — oval ama daireden belirgin biçimde yassı.

**08 — Çiçek (Flower)**  
Büyük Lp (230 > r₃ = 180). Coupler noktası bağlantı uzunluğunu aştığında iç döngüler oluşur; çiçek yapraklarına benzer form.

**09 — Kalp (Heart)**  
r₃ = 165 kasıtlı kısa; negatif α (−34°) ile coupler noktası sol alta kaymış. Büyük Lp kombinasyonu kalp benzeri asimetrik eğri üretir.

**10 — Damla (Teardrop)**  
Orta büyüklükte Lp ve küçük pozitif α. r₃ uzun (230), r₄ orta (190) → yukarıda yuvarlak, aşağıda sivri damla formu.

**11 — Köpekbalığı (Shark)**  
r₁ en büyük (260), negatif α (−52°) belirgin. Büyük Lp ve asimetrik kol oranları köpekbalığı yüzgecini andıran çıkıntılı eğri verir.

**12 — Yaprak (Leaf)**  
α = 63° yüksek açılı. r₃ ≈ r₄ ≈ r₁ dengeli oranı Lp ile birleşince kapalı, ince yaprak biçimi çıkar.

**13 — Dümen (Helm)**  
Grashof marjı = 15 (kasıtlı sınıra yakın). r₂ = 105 büyük krank; büyük Lp ile karmaşık, dümen çarkı benzeri döngülü eğri.

**14 — Hilal (Crescent)**  
α = −63° ile en büyük negatif açı. Küçük r₂ (55), uzun r₃ (255) kombinasyonu açık ay/hilal formu üretir.

**15 — Kelebek (Butterfly)**  
Grashof marjı = 10 (en zorun seviye). r₂ = 120 maksimuma yakın, Lp = 240 büyük. İki simetrik döngü → kelebek kanadı.

---

## Parametre Aralıkları (Slider)

| Parametre | Min | Max | Adım |
|-----------|-----|-----|------|
| r₂ (krank) | 20 | 130 | 1 |
| r₃ (bağlantı) | 100 | 300 | 1 |
| r₄ (salıcı) | 100 | 300 | 1 |
| Lp (coupler uzunluğu) | 0 | 280 | 1 |
| α (coupler açısı) | −90° | 90° | 1° |

---

*Bu dosya yalnızca geliştirici referansı içindir. Oyunun içinde çözümler gösterilmez.*
