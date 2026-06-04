# Mechanism Master v0.2 - Iyilestirme Onerileri

Hazirlayan: Codex  
Tarih: 2026-06-02  
Kopya kaynak: https://sahinyavuzz.github.io/mechanism-master/

## Kisa Degerlendirme

Mechanism Master v0.2, Steam/desktop icin anlamli bir cekirdege sahip. En guclu yani, gercek makina muhendisligi bilgisini oyun mekanigine cevirmesi: dort cubuk mekanizma, Grashof kosulu, kuplor egrisi ve hedef egri eslestirme oyunun kimligini netlestiriyor.

v0.1'e gore buyuk ilerleme var:

- 15 seviye
- TR/EN dil secimi
- Tutorial
- Goruntu kaydetme
- Daha temiz teknik gorsel kimlik

Ancak Steam'de ilgi cekmesi icin oyun hissi ve ilerleme duygusu daha gorunur olmali.

## Strateji

Once Steam/desktop demo hedeflenmeli. Mobil daha sonra ayri bir UI tasarimi olarak ele alinmali.

Neden:

- Buyuk cizim alani ve hassas slider kontrolu desktopta daha dogal.
- Steam kitlesi Poly Bridge, Opus Magnum, Kerbal Space Program gibi muhendislik/puzzle oyunlarina daha yakin.
- Mobilde mevcut UI tasiyor ve ayar yaparken mekanizmayi ayni anda takip etmek zor.
- Steam demosu, oyunun gercek pazar ilgisini olcmek icin daha dogru kanal.

## Oncelik 1 - Steam Demo Icin Kritik Isler

### 1. Basari ve Yildiz Sistemi

Mevcut uyum olcumu iyi, ama oyuncuya daha oyun gibi donmeli.

Oneri:

- 70% ve ustu: 1 yildiz
- 82% ve ustu: 2 yildiz
- 93% ve ustu: 3 yildiz
- Seviye gecisinde kisa bir sonuc karti
- "Yeni rekor", "mukemmel sentez", "Grashof bonusu" gibi mikro oduller

Beklenen etki:

- Tekrar oynama motivasyonu artar.
- Steam sayfasinda gif/video icin daha guclu anlar olusur.

### 2. Tutorial'i Etkilesimli Hale Getirme

Mevcut tutorial aciklayici, fakat oyuncu okumadan gecerse ne yapacagini kacirabilir.

Oneri:

- Ilk seviyede zorunlu mini adimlar:
  - "Krank r2 sliderini saga cek"
  - "Mavi izin nasil degistigini izle"
  - "Uyumu Olc butonuna bas"
- Tutorial metni daha kisa, eylem daha fazla olsun.

Beklenen etki:

- Oyuncu ilk 60 saniyede oyunu kavrar.
- Teknik korkutuculuk azalir.

### 3. Seviye Seciminde Ilerleme Haritasi

Su an seviyeler sayi butonlariyla veriliyor. Bu islevsel ama biraz arac hissi veriyor.

Oneri:

- Seviye listesi "Atolye Defteri" veya "Mekanizma Katalogu" gibi sunulabilir.
- Her seviyenin kucuk hedef egri ikonu olsun.
- Tamamlanan seviyelerde yildizlar gorunsun.
- Kilitli/onerilen seviye akisi eklenebilir.

Beklenen etki:

- Oyuncu "simulator" degil "puzzle campaign" oynadigini hisseder.

### 4. Seviye Cesitliligi ve Zorluk Egrisi

15 seviye demo icin iyi. Fakat ilk 5 seviye cok dikkatli ayarlanmali.

Oneri:

- Seviye 1: kolay daire/oval, tek sliderla fark gorulsun.
- Seviye 2: yumurta formu, kuplor noktasi tanitilsin.
- Seviye 3: Grashof kosulu ilk kez anlam kazansin.
- Seviye 4-5: oyuncu gercek optimizasyon hissi alsin.
- Demo sonu: "Steam wishlist" veya "tam surumde 60+ seviye" mesaji.

### 5. Geri Bildirim Efektleri

Uyumu olcunce sayi degisiyor, ama duygu daha guclendirilmeli.

Oneri:

- Uyum skoru artinca mavi iz kisa sure parlasin.
- Hedefe yaklasan bolgelerde noktasal vurgu olsun.
- Kazanma aninda mekanizma bir tur daha temiz animasyonla donsun.
- Basarisiz olcumde "P noktasini uzaklastirmayi dene" gibi ipucu verilsin.

## Oncelik 2 - Kalite ve Yayina Hazirlik

### 6. Mobil Tasmanin Simdilik Kontrol Altina Alinmasi

Mobil ikinci faz olsa bile web demo acildiginda kirpik gibi batmamali.

Mevcut sorun:

- 390px genislikte sayfa 477px'e kadar tasiyor.
- "Uyumu Olc" butonu sagdan kesiliyor.

Oneri:

- Mobilde `.action-row` tek sutun olmali.
- Body yatay tasma gercekten sifirlanmali.
- Canvas ve kontroller mobilde akordeon veya sekme ile ayrilmali.

Bu is Steam oncesi ana hedef degil, ama web demo icin kucuk bir temizlik olarak yapilmali.

### 7. Kayit ve Ilerleme

Oneri:

- LocalStorage ile seviye yildizlari kaydedilsin.
- En iyi skor/uyum orani saklansin.
- "Tum ilerlemeyi sifirla" butonu ayarlara konabilir.

### 8. Steam Sayfasi Icin Medya

Oneri:

- 6-8 saniyelik gifler:
  - slider degisince egrinin hareketi
  - hedefe yaklasma
  - 3 yildiz tamamlama
- Kisa trailer akisi:
  - "Design the linkage"
  - "Trace the curve"
  - "Master real mechanism theory"

### 9. Konumlandirma Metni

Steam kisa aciklama onerisi:

> Design four-bar linkages, trace target curves, and solve elegant mechanical puzzles built on real engineering principles.

Turkce kisa aciklama:

> Dort cubuk mekanizmalarini ayarla, hedef egrileri yakala ve gercek makina muhendisligi prensipleriyle tasarlanmis bulmacalari coz.

## Oncelik 3 - Tam Surum Fikirleri

- 60+ el yapimi seviye
- Cams, gears, Geneva drive, slider-crank gibi yeni mekanizma aileleri
- Level editor
- Workshop destegi
- "Professor's Challenge" zor seviye paketi
- Makina muhendisligi terimlerini oyun ici mini kartlarla ogreten koleksiyon sistemi

## Uygulama Sirasi

1. Mobil tasma icin kucuk CSS duzeltmesi
2. Yildizli sonuc sistemi
3. Ilerleme kaydi
4. Etkilesimli tutorial
5. Seviye secim ekranini kampanya hissine yaklastirma
6. Steam demo metinleri ve medya hazirligi

## Net Karar

Mechanism Master v0.2, Steam demo yoluna girmeye deger. Su an "egitimsel simulator" ile "puzzle oyunu" arasinda duruyor. Bir sonraki gelistirme dalgasi oyunu simulator tarafindan biraz cekip, puzzle campaign tarafina tasimali.

