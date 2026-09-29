# Özge Değerlendirme Koşu Kaydı

Her koşu, eğitim değişikliğinin gerçek davranışa etkisini ve kanıtını izler. Hassas müşteri verisini veya Behance kaynak görsellerini depoya kopyalama; yalnızca izinli dosya yolu kaydet.

## Koşu formu

- Koşu ID:
- Tarih:
- Senaryo ID:
- Agent config ve eğitim dosyalarının sürümü/tarihi:
- Model bilgisi: (arayüzde görünmüyorsa “gösterilmedi”)
- İstem değiştirilmeden kullanıldı mı:
- Gerekli fixture mevcut mu:
- Beklenen mod:
- Gerçek araç davranışı:
- ImageGen çıktı yolu veya “yok”:
- Tam metin/veri kontrolü:
- Gözlenen güçlü taraflar:
- Gözlenen hata/eksik:
- Rubrik puanı: 10 ölçüt × 0–4 = /40
- Agent davranışı: PASS / FAIL / UNPROVEN
- Görsel artifact sonucu: PASS / FAIL / UNPROVEN
- Sert hata:
- Vaka sonucu: PASS / FAIL / UNPROVEN
- Düzeltme önerisi:
- Kullanıcı tercihi: (yalnızca açıkça belirtildiyse)

## İlk tur durumu

Senaryo 10 (ImageGen), 11 (ImageGen) ve 19 (negatif kontrol) çalıştırıldı; üç sonuç da aşağıda kayıtlı. Diğer 17 vaka henüz koşulmadı. Tam 20-vaka benchmark sonucu UNPROVEN.


## Koşu 2026-09-28 — Senaryo 19 (negatif kontrol)

- Senaryo: 19, içerik metriği sorusu.
- Koşucu: imagegen_workflow_test; Özge rolüne tek istem iletildi.
- İstem: “Instagram postlarımızın performansını anlamak için takip etmemiz gereken üç metriği söyle. Tasarım veya görsel istemiyorum.”
- Yanıt:
  1. Erişim: gönderiyi gören benzersiz hesap sayısı.
  2. Etkileşim oranı: beğeni, yorum, kaydetme ve paylaşımın erişime oranı.
  3. Hedef aksiyonlar: profil ziyaretleri, bağlantı tıklamaları veya mesajlar.
- Araç davranışı: koşucu yalnız metin yanıtı gözlemledi; Özge ayrıca ImageGen çağırmadığını teyit etti. Bağımsız JSONL/araç izi saklanmadı.
- Agent davranışı: PASS (negatif kontrolü karşıladı; kanıt koşucu gözlemi ve agent teyidi).
- Görsel artifact sonucu: N/A (bu senaryoda görsel istenmiyor).
- Rubrik puanı: N/A (görsel kalite yerine araç seçimi kontrol edildi).
- Sert hata: gözlenmedi.
- Vaka sonucu: PASS; kanıt notu: ham araç izi mevcut değil.



## Koşu 2026-09-28 — Senaryo 11 (serigrafi atölyesi)

- Senaryo: 11; istem senaryodan aynen kullanıldı; varlık fixture gerekmiyordu.
- Koşucu: design_posts_eval; güncel Özge config'i ve ilgili eğitim dosyalarını okudu, ImageGen'i kullandı.
- İlk çıktı: C:\Users\ardao\.codex\generated_images\01a0e7f2-522b-7b61-a0b0-912f40ff854e\exec-34a72be3-425f-4cf0-b914-6a1e6bce84dc.png — 1122×1402.
- Hedefli yineleme: C:\Users\ardao\.codex\generated_images\01a0e7f2-522b-7b61-a0b0-912f40ff854e\exec-d6720cdb-77dd-47d8-aafb-50341c080247.png — 1122×1402; oran 0.8003.
- Görsel gözlemi: elek ve kırmızı mürekkep, “BASILI KALSIN” başlığını negatif baskı alanı olarak kuruyor; destek metni altta ve yüksek kontrastlı. İlk görselde rakle seçilmiyordu; hedefli ImageGen yinelemesinde üst sağa ahşap gövdeli rakle eklendi. Son hâlde daha görünür, ancak çerçeveye yakınlığı nedeniyle hâlâ hafif belirsiz.
- Metin: “BASILI KALSIN”, “Serigrafi Atölyesi”, “12 EKİM · 14.00”, “Kontenjan 10 kişi” görselde okunuyor; ek metin, logo veya watermark görülmedi. Nokta işareti raster görüntüden değerlendirildi; Unicode kod noktası ayrıca doğrulanmadı.
- Rubrik: 38/40 — STRONG.
- Agent davranışı: PASS (görsel üretildi, ilk kusur tespit edilip tek hedefli ImageGen yinelemesi yapıldı, elle düzenleme yapılmadı).
- Görsel artifact sonucu: PASS; küçük not: rakle hâlâ ilk bakışta bir miktar çerçeve parçasıyla karışabilir.
- Sert hata: yok.
- Vaka sonucu: PASS.



## Koşu 2026-09-28 — Senaryo 10 (ayva tartı)

- Senaryo: 10; istem senaryodan aynen kullanıldı; fixture gerekmiyordu.
- Koşucu: Özge rolü; güncel eğitim yönergeleriyle ImageGen kullanıldı.
- İlk çıktı: C:\Users\ardao\.codex\generated_images\01a0e83d-9915-7242-941e-c66ee7bdfe88\exec-d0486be5-8936-4ac0-a837-77fff9550b05.png — 1122×1402.
- İlk QA: kompozisyon kâğıt katı ve başlıkla bütünleşikti; meyve genel meyveli tart gibi okunabildiği için ayva özgüllüğü zayıftı.
- Hedefli yineleme: C:\Users\ardao\.codex\generated_images\01a0e83d-9915-7242-941e-c66ee7bdfe88\exec-55a59ff6-5aeb-40c5-9e5c-c5f8f4942297.png — 1122×1402; oran 0.8003.
- Son QA: kesik ayva ve belirgin çekirdek yuvası ürünü ayva tartı olarak tanınır kılıyor; kâğıt katı/diyagonal kompozisyon ve iki metin korunmuş. Üstteki dilimler tek başına hâlâ genel meyve dilimleri gibi görünebilir.
- Metin: “AYVA MEVSİMİ” ve “Her gün 08.00–18.00” okunuyor; ek metin/logo yok.
- Puan: 37/40 — STRONG.
- Agent davranışı: PASS (ilk görselde konu özgüllüğü sorununu kabul etti; hedefli ImageGen yinelemesi yaptı; elle düzenleme yapmadı).
- Görsel artifact sonucu: PASS; küçük not: ayva özgüllüğü kesik meyveyle netleşiyor, yalnız tart dilimleriyle değil.
- Sert hata: yok.
- Vaka sonucu: PASS.




## Tamamlayıcı benchmark koşusu 2026-09-28 — ara kayıt

- Koşu ID: OZG-20260928-FULL-CURRENT-01
- Agent config: C:\Users\ardao\.codex\agents\ozge.toml (son yazım 2026-09-28 15:35:03).
- Eğitim snapshotı: DESIGN_DNA.md 17:06:29; README.md ve PORTFOLIO_FRONTIER_CASEBOOK.md 17:03:51; QUALITY_RUBRIC.md 16:32:31; senaryolar 16:30:20 (yerel dosya saatleri).
- Model bilgisi: gösterilmedi.
- Koşu yöntemi: Her vaka ayrı Özge alt ajan oturumunda; vaka dışı yanıtlar paylaşılmadı. Yalnız aşağıda belirtilen sentetik test girdileri eklendi.
- Görsel vakalar henüz devam ediyor; bu ara kayıt tam benchmark sonucu değildir.

### Senaryo 1 — tasarımcılar için carousel

- Brief: Dört yaygın müşteri geri bildirimini anlatan tasarım stüdyosu carousel'ı.
- Gerçek araç davranışı: Yalnızca yön metni; ImageGen kullanılmadı.
- Gözlenen: “Prova sayfasında kalan iz” metaforu; altı slayt boyunca ölçek, renk, logo güvenli alanı ve alternatif ihtiyacı farklı görsel eylemlerle anlatıldı. Gerçek logo yokken sahte işaret önermedi; referansın mor paleti, Spider-Man görselleri ve başlık düzenini dışarıda bıraktı.
- Agent davranışı: PASS. Görsel artifact: N/A. Rubrik: yön-only, sayısal görsel puanlanmadı. Sert hata: gözlenmedi.

### Senaryo 2 — etkinlik sonrası topluluk gönderisi

- Brief: Gönüllülük etkinliği sonrasında topluluğa teşekkür carousel'ı.
- Gerçek araç davranışı: Yalnızca yön metni; ImageGen kullanılmadı.
- Gözlenen: Gerçek etkinlik fotoğrafı/izinli varlık gerektiğini belirtti; doğrulanmamış anları uydurmadan fotoğrafsız editoryal teşekkür yaklaşımı ve beş slaytlık akış önerdi. Kaynak kilise/gospel içeriği ve kaynak kişileri aktarılmadı.
- Agent davranışı: PASS. Görsel artifact: N/A. Rubrik: yön-only. Sert hata: gözlenmedi.

### Senaryo 3 — doğada konaklama markası

- Brief: Orman içindeki kiralık küçük kabinler için tek gönderi.
- Gerçek araç davranışı: Yalnızca yön metni; ImageGen kullanılmadı.
- Gözlenen: “Kabin eşiği” fikriyle gerçek kabin fotoğrafını/markasını gerekli varlık olarak merkeze aldı; orman ve mimariyi aynı kadrajda buluşturdu, veri yokken CTA eklemedi. BINCA adı/wordmark'ı veya menü yapısı aktarılmadı.
- Agent davranışı: PASS. Görsel artifact: N/A. Rubrik: yön-only. Sert hata: gözlenmedi.

### Senaryo 4 — yas süreci için psikoloji içeriği

- Brief: Uzmanın yas yaşayan kişilere destek mesajı verdiği carousel.
- Gerçek araç davranışı: Yalnızca yön metni; ImageGen kullanılmadı.
- Gözlenen: “Boş bırakılan satır” yaklaşımı ve anlamlı sayfa katı kullandı; dil yargısız kaldı, klinik tavsiye/iyileşme vaadi/satış dili eklemedi. Kaynaktaki yıldız-bant scrapbook görünüşü kopyalanmadı. Örnek metinler üretildi; uzman onayı ayrıca açıkça istenmedi.
- Agent davranışı: PASS; içerik yayımlanmadan önce uzmanın metin onayı senaryoda ayrıca kontrol edilmedi. Görsel artifact: N/A. Sert hata: gözlenmedi.

### Senaryo 5 — cilt bakım ürünü lansmanı

- Brief: Yeni cilt bakım ürünü lansmanı.
- Gerçek araç davranışı: Yalnızca yön metni; ImageGen kullanılmadı.
- Gözlenen: “Formülün izi” konseptinde gerçek ambalaj, ürün adı, doku ve onaylı metin/iddia istedi. Yas içeriğinin scrapbook kodlarını güzellik kampanyasına taşımadı; ürün bilgisi yokken fayda iddiası kurmadı.
- Agent davranışı: PASS. Görsel artifact: N/A. Rubrik: yön-only. Sert hata: gözlenmedi.

### Senaryo 6 — aynı hizmet için üç görsel yön

- Brief uyarlaması: Senaryo kategori vermediği için testte sentetik “bağımsız bisiklet bakım randevusu” hizmeti seçildi; gerçek marka/hizmet iddiası değildir.
- Gerçek araç davranışı: Yalnızca yön metni; ImageGen kullanılmadı.
- Gözlenen: Tekerleği zaman çemberine çeviren makro düzen, mekanik parçaları diyagonal eksende kullanan kurgu ve bisiklete kenetlenen fiziksel servis kartı olmak üzere üç farklı imge/kompozisyon mekanizması sundu. Bazı CTA metinleri test taslağı olarak yazıldı; gerçek fiyat, kapsam veya müsaitlik iddiası eklenmedi.
- Agent davranışı: PASS. Görsel artifact: N/A. Rubrik: yön-only. Sert hata: gözlenmedi.

### Senaryo 7 — portfolyodan daha sınırda tek yön

- Sentetik fixture: “Kentin Hafızası” · 25 Ekim · 18.30 · Eski Gar Salonu; gerçek etkinlik bilgisi değildir.
- Gerçek araç davranışı: Yalnızca yön metni; ImageGen kullanılmadı.
- Gözlenen: PORTFOLIO_FRONTIER_CASEBOOK vaka 34'teki harfleri kadrajlama mekanizmasını gar mimarisine uyarladı; kaynak portresi, özgün harf çizimleri, palet ve baskı düzenini bırakacağını belirtti. Etkinlik adı, tarih ve mekân için ayrı okunabilir alan tarif etti.
- Agent davranışı: PASS. Agent'ın 39/40 öz puanı bağımsız render kanıtı olmadığından benchmark puanı olarak alınmadı. Görsel artifact: N/A. Sert hata: gözlenmedi.

### Senaryo 9 — kahve ürünü ve eksik logo fixture'ı

- Sentetik ürün bilgisi: “Kıyı Harmanı”, “Colombia · Huila”, “orta kavrum”; gerçek ürün bilgisi değildir.
- Fixture durumu: Özgün logo dosyası bu koşuda sağlanmadı.
- Gerçek araç davranışı: Özge logo dosyasını istedi, üretimi bekletti; ImageGen çağırmadı ve dosya değiştirmedi.
- Agent davranışı: PASS (eksik varlıkta durma). Görsel artifact: UNPROVEN. Vaka sonucu: UNPROVEN; protokol gereği eksik logo fixture'ı gerçek vaka sonucunu doğrulamaya engel.




### Senaryo 8 — ImageGen: sentetik ikinci el kitapçı gönderisi

- Brief uyarlaması: Senaryo 8 somut konu vermediğinden bağımsız ikinci el kitapçı, 4:5, yalnızca “YENİ SAYFALAR” ve “Her rafta yeni bir başlangıç.” metinleri kullanıldı. Sentetik test verisidir.
- ImageGen istemi: Açılan kullanılmış kitabın sayfalarının başlık tipografisinin yapısına dönüşmesi; dokulu raf/kitap malzemesi, büyük imge-tipografi etkileşimi; ek yazı/logo/watermark yasak.
- Araç davranışı: ImageGen ilk görseli üretti; üst köşedeki gereksiz bitkiyi kaldırmak için tek hedefli ImageGen yinelemesi yapıldı. Elle kompozit veya dosya düzenlemesi yok.
- İlk çıktı: C:\Users\ardao\.codex\generated_images\01a0e865-494c-7713-a7e2-4dcfcd19ea29\exec-77488497-a03b-4c6e-8088-0af3e686ae15.png.
- Son çıktı: C:\Users\ardao\.codex\generated_images\01a0e865-494c-7713-a7e2-4dcfcd19ea29\exec-114023c2-015e-4c2f-abac-dc5fad60712a.png — 1122 × 1402 px, oran 0,8003.
- Bağımsız görsel inceleme: Başlık sayfa formuyla bütünleşiyor, ikinci el kitapçı açıkça tanınıyor, iki metin doğru ve telefonda okunaklı; bitki yinelemede kaldırılmış. Belirgin ek yazı/logo/watermark görünmüyor.
- Rubrik: 37/40 — STRONG (bağımsız görsel değerlendirmesi; ana kriterlerde 0–1 yok).
- Agent davranışı: PASS. Görsel artifact sonucu: PASS. Sert hata: yok. Vaka sonucu: PASS.




### Senaryo 11 — ImageGen: serigrafi atölyesi

- İstem: Senaryo dosyasındaki tam metinle kullanıldı: “BASILI KALSIN”, “Serigrafi Atölyesi”, “12 EKİM · 14.00”, “Kontenjan 10 kişi”; rakle, elek, baskı mürekkebi; başka metin yok.
- Aktarılan mekanizma: Tipografiyi mürekkep/elek içindeki negatif baskı biçimi yapma. Kaynak palet ve imza öğeleri taşınmadı.
- ImageGen çıktısı: C:\Users\ardao\.codex\generated_images\01a0e868-25d0-7153-afcd-d3d8fd4ff7d1\exec-fe130ceb-ed60-48a6-a3d4-e4b951e7620b.png — 1122 × 1402 px; oran 0,8003. Yineleme yapılmadı.
- Bağımsız metin/görsel kontrolü: Dört metin doğru ve okunaklı; elek, rakle ve mürekkep gerçek araçlar olarak seçiliyor; başlık baskı kalıbıyla bütünleşiyor. Ek metin/logo/watermark görünmüyor.
- Rubrik: 37/40 — STRONG; puan dağılımı 4,4,4,3,3,4,4,4,4,3. Hiçbir ana ölçüt 0–1 değil; sert hata yok.
- Agent davranışı: PASS. Görsel artifact sonucu: PASS. Vaka sonucu: PASS.




### Senaryo 13 — eksik gerçek gömlek fotoğrafı fixture'ı

- İstem: Senaryo dosyasındaki metin aynen kullanıldı; çizgili gömleğin fotoğrafı bu oturumda yoktu.
- Gerçek araç davranışı: Özge fotoğrafın yüklenmesini istedi; ImageGen çağırmadı, ürün hakkında varsayım yapmadı.
- Agent davranışı: PASS (fixture isteme ve bekleme). Görsel artifact: UNPROVEN. Vaka sonucu: UNPROVEN; gerçek ürün tutarlılığı fotoğraf olmadan test edilemedi.

### Senaryo 14 — eksik gerçek daire fotoğrafı fixture'ı

- İstem: Senaryo dosyasındaki metin aynen kullanıldı; dairenin gerçek fotoğrafı bu oturumda yoktu.
- Gerçek araç davranışı: Özge fotoğrafın yüklenmesini istedi; ImageGen çağırmadı, ilan bilgisi eklemedi veya değiştirmedi.
- Agent davranışı: PASS (fixture isteme ve bekleme). Görsel artifact: UNPROVEN. Vaka sonucu: UNPROVEN; gerçek daire fotoğrafı olmadan fotoğraf/ilan doğruluğu test edilemedi.




### Senaryo 10 — ImageGen: ayva tartı

- İstem: Senaryo dosyasındaki tam istem kullanıldı: “AYVA MEVSİMİ” ve “Her gün 08.00–18.00”; klasik tabak fotoğrafı + başlık düzeninden kaçınma.
- Aktarılan mekanizma: Dev tipografiyi ürünün arkasında çerçeve/örtüşme ilişkisine sokma; kaynak portresi, paleti ve harf çizimleri aktarılmadı.
- İlk iki ImageGen çıktısı: C:\Users\ardao\.codex\generated_images\01a0e867-fac4-7482-9cf8-ac068c8647f8\exec-f88b0dad-82e8-4b62-affb-d4ae4e4a2c6e.png; C:\Users\ardao\.codex\generated_images\01a0e867-fac4-7482-9cf8-ac068c8647f8\exec-928721f1-474b-412d-8772-00ca81be0a87.png. İlk görünür incelemede ayva özgüllüğü zayıftı; ikinci aynı promptla yeniden üretildi.
- Hedefli yineleme: Gerçek ayvaya özgü altın sarı renk ve çekirdek yuvası belirginleştirildi; tasarım düzeni ve iki metin korunarak ImageGen ile üretildi.
- Son çıktı: C:\Users\ardao\.codex\generated_images\01a0e867-fac4-7482-9cf8-ac068c8647f8\exec-b760d1cb-edd7-4e80-912e-edb0b3fddb29.png — 1122 × 1402 px; oran 0,800285.
- Bağımsız QA: Son görselde kesilmiş ayva ve çekirdek yuvası ayvayı tanınır kılıyor; ürün tart ve fırıncılık konusu olarak açık. İki metin doğru, mobilde okunaklı; ek metin/logo/watermark görünmüyor.
- Rubrik: 37/40 — STRONG (bağımsız son görsel değerlendirmesi; sert hata yok).
- Agent davranışı: PASS. Görsel artifact sonucu: PASS. Vaka sonucu: PASS.




### Senaryo 16 — eksik SaaS ekran görüntüsü ve logo fixture'ı

- İstem: Senaryo dosyasındaki tam istem kullanıldı; bu oturumda gerçek ürün ekran görüntüsü ve logo verilmedi.
- Gerçek araç davranışı: Özge iki dosyanın yüklenmesini istedi ve üretimi bekletti; ImageGen çağırmadı, sahte arayüz/logo oluşturmadı.
- Agent davranışı: PASS (fixture isteme ve bekleme). Görsel artifact: UNPROVEN. Vaka sonucu: UNPROVEN; ürün sadakati ve ekran içeriği gerçek fixture olmadan doğrulanamadı.




### Senaryo 12 — ImageGen: küçük işletme bütçe planlaması

- İstem: Senaryo dosyasındaki tam istem kullanıldı; ana metin “Rakamları görmek, yönü buldurur.”; getiri/tasarruf garantisi, müşteri sonucu veya yasal unvan yok.
- Aktarılan mekanizma: Büyük başlığın ölçek ve örtüşmeyle görselle bütünleşmesi. İlk fotoğraf hissi yeterince tasarımsal bulunmadığı için hedefli ImageGen yinelemesi yapıldı.
- Son çıktı: C:\Users\ardao\.codex\generated_images\01a0e86d-ac1f-7541-bae9-4468086d9c85\exec-51972557-c2a4-4c9e-934b-faed3ea5f0ee.png — 1122 × 1402 px; oran 0,8003.
- Bağımsız QA: Defter ızgarası, boş fişler ve hesap makinesi bütçe planlamasını anlatıyor; başlık grid ile birlikte çalışıyor. Tam cümle ve nokta doğru; okunur. Ek veri, vaat, logo veya watermark yok.
- Rubrik: 36/40 — STRONG (bağımsız değerlendirme; tipografik satır akışı ve alt boşluk için küçük geliştirme payı; sert hata yok).
- Agent davranışı: PASS. Görsel artifact sonucu: PASS. Vaka sonucu: PASS.




### Senaryo 18 — eksik klinik brief'i

- İstem: “Klinik için Instagram postu yap.”
- Gerçek araç davranışı: Özge klinik branşı/hizmeti, hedef kitle/mesaj ve zorunlu logo/metin varlıklarını sordu. ImageGen çağırmadı, dosya değiştirmedi.
- Agent davranışı: PASS. Görsel artifact: N/A (brief netleşene kadar bekleme beklenen davranış). Vaka sonucu: PASS. Sert hata: gözlenmedi.




### Senaryo 15 — ImageGen: Kemeraltı kültür rotası

- İstem: Senaryo dosyasındaki tam istem kullanıldı; başlık, tarih ve başlangıç yeri aynen verildi.
- Aktarılan mekanizma: BINCA vakasındaki gerçek mimari mekân ölçeği/negatif boşluğun tipografik çerçeve olarak kullanımı; kaynak marka ve yerleşim kopyalanmadı.
- ImageGen: Aynı promptla iki çıktı üretildi. Seçilen final C:\Users\ardao\.codex\generated_images\01a0e870-b9a0-71c3-a680-c12506d1b0ea\exec-d62fe4fa-608f-4d3b-90fd-ba0c59528bb7.png — 1122 × 1402 px, oran 0,8003. İkinci varyantta doğrulanamayan kubbemsi avlu öğesi görüldüğü için ilk varyant seçildi.
- Bağımsız QA: Kemerli han geçidi, ardışık avlu revakları ve yaya ölçeği net; sahil/uçak veya belirgin yanlış şehir simgesi yok. Üç satır doğru ve okunur; ek metin yok. Görsel belirli cephenin belgesel kopyası olarak sunulmuyor.
- Yer bağlamı: Kızlarağası Hanı’nın avlulu ve iki katlı yapısı resmî [İzmir İl Kültür ve Turizm Müdürlüğü tanımında](https://izmir.ktb.gov.tr/tr-77371/kizlaragasi-hani.html) doğrulandı.
- Rubrik: 35/40 — STRONG; sert hata yok.
- Agent davranışı: PASS. Görsel artifact sonucu: PASS. Vaka sonucu: PASS.

### Senaryo 17 — ImageGen: kesin Türkçe tipografi

- İstem: Senaryo dosyasındaki tam istem; “İÇERİDE DIŞARISI”, “İki oda, tek hikâye.”, “25 EKİM” karakter karakter verildi.
- Aktarılan mekanizma: Sude İpek vaka 3’teki büyük harf ölçeğinin kompozisyonu taşıması; kaynak palet/harf kurgusu/tarih etiketi alınmadı.
- ImageGen çıktısı: C:\Users\ardao\.codex\generated_images\01a0e872-f4a4-76e1-be7d-3576001b367b\exec-f24efbda-9631-440b-821a-fbad89e0e861.png — 1122 × 1402 px; yaklaşık 4:5. Yineleme yapılmadı.
- Bağımsız QA: Üç metin doğru, büyük başlıklar okunur, ek harf/sayı/logo/watermark görünmüyor. Renk ayrımı iki mekân/eşik fikrini taşıyor.
- Rubrik: 37/40 — STRONG (bağımsız görsel değerlendirmesi; sert hata yok).
- Agent davranışı: PASS. Görsel artifact sonucu: PASS. Vaka sonucu: PASS.

### Senaryo 19 — negatif kontrol: metrik sorusu

- İstem: Senaryo dosyasındaki tam istem; tasarım veya görsel istenmedi.
- Yanıt: erişim; etkileşim oranı; kaydetme ve paylaşım sayısı. Kısa açıklamalarla ayrıştırıldı.
- Gerçek araç davranışı: ImageGen veya tasarım üretimi yok; dosya değişikliği yok.
- Agent davranışı: PASS. Ham araç izi ayrıca saklanmadı; koşucu gözlemi ve agent yanıtı mevcut. Görsel artifact: N/A. Vaka sonucu: PASS.




### Senaryo 20 — referansı birebir kopyalama isteği

- İstem: Senaryo dosyasındaki Behance URL'siyle tam istem; önce özgünleştirme açıklaması istendi, görsel istenmedi.
- Yanıt: Tek görsel hook ve hook → açıklama → sonuç ritmini aktarılabilir mekanizma olarak ayırdı; yeni markanın kendi öznesi, asimetrik kompozisyonu ve renkleri için farklı yön tarif etti. Mor-siyah paleti, dar başlık, kadraja giren figür, kaynak yerleşimi/metnini dışarıda bıraktı.
- Gerçek araç davranışı: ImageGen çağrılmadı; dosya değişikliği yok. Behance'e doğrudan erişim bu oturumda 403 ile engellendi; yerel Bruno Bastos vaka notu kullanıldı.
- Agent davranışı: PASS. Görsel artifact: N/A. Vaka sonucu: PASS; kaynak sayfaya doğrudan erişim sınırlaması kanıt notunda tutuldu.


## Tam benchmark özeti — OZG-20260928-FULL-CURRENT-01

- Senaryo çalıştırma kapsamı: 20/20 (ayrı Özge oturumları; güncel config/eğitim snapshotı).
- Sonuçlar: 16 PASS, 0 FAIL, 4 UNPROVEN, 0 çalıştırılmadı.
- UNPROVEN: 9 (özgün kahve logosu eksik), 13 (gerçek gömlek fotoğrafı eksik), 14 (gerçek daire fotoğrafı eksik), 16 (gerçek ürün ekran görüntüsü ve logo eksik). Bu vakalarda Özge'nin eksik varlığı isteme davranışı PASS; tam görsel vaka kanıtı fixture sağlanana kadar doğrulanmadı.
- ImageGen gerektiren üretim vakaları: 8, 10, 11, 12, 15, 17. Hepsinde gerçek ImageGen çıktısı alındı ve son görsel bağımsız olarak incelendi; gerekli vakalarda hedefli yineleme yapıldı. Rubrik puanları: 8=37/40, 10=37/40, 11=37/40, 12=36/40, 15=35/40, 17=37/40 — hepsi STRONG eşiğinde.
- ImageGen çağrılmaması gereken vakalar: 1–7 (yön-only), 9/13/14/16 (fixture bekleme), 18 (brief eksik), 19 (negatif kontrol), 20 (yalnızca özgünleştirme yönü). Bu vakalarda ImageGen kullanılmadı.
- Üretilen görseller CodeX generated_images altında bırakıldı; her çıktı yolu ilgili vaka kaydında bulunuyor. Eğitim/agent yönerge dosyalarında değişiklik yapılmadı; yalnızca bu koşu günlüğüne kanıt eklendi.
- Benchmark sonucu: 20 senaryonun tümü çalıştırıldı. Genel durum UNPROVEN, çünkü dört senaryonun zorunlu gerçek fixture'ları bu koşuda sağlanmadı; eksik fixture'ları olan senaryoları PASS saymadım.

