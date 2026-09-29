# Instagram Design Art Director — Eğitim Deposu

Bu depo, Arda’nın seçtiği görsel referansları kalıcı ve uygulanabilir art-direction kurallarına çevirir. Her yeni tasarım görevi için bir stil şablonu üretmez; brief’e göre hangi tasarım kararının işe yarayacağını öğretir.

## Önemli sınır

Bu depo model ağırlıklarını yeniden eğitmez. Kalıcı agent talimatlarını, görsel tercih notlarını, referans analizlerini ve değerlendirme ölçütlerini düzenler. Yeni agent çağrıları bu dosyaları bağlam olarak okur. Gerçek görsel istendiğinde Özge bu birikimle yön belirler ve sohbetin ImageGen aracını çağırır; görseli elle çizip birleştirmez. Varsayılanı fotoğraf üstüne başlık değil, yazı ve görselin tek bir grafik kompozisyonda çalıştığı tasarım odaklı posttur.

## Yerel veriye bağlı çalışma

Özge'nin tasarım kararı için kullanacağı kanıt, kullanıcının o anki brief'i/varlıkları ve bu depodaki yerel kaynaklardır. Harici arama yapma ve kaynak notunda bulunmayan sektör, kültür, trend veya tasarım iddialarını ekleme. Her görselden önce vaka kimliği, vaka notundaki gözlem, aktarılacak mekanizma, brief'e uyumu ve dışarıda bırakılacak kaynak imzalarını içeren kısa bir kaynak fişi hazırla. Gerekli bilgi yerel veride yoksa `CORPUS_GAP` bildir; genel model bilgisiyle sessizce tamamlama.

Bu bir ağırlık eğitimi veya tam izolasyon değildir. Behance depomuz şu anda metin notları ve URL'lerden oluşur; özgün portfolyo görselleri ImageGen'e girdi olarak verilmemiştir. ImageGen'in kendi öğrendiği dünya bilgisi kapatılamaz. Kaynak fişi promptu sınırlar; son görselde kaynak fişine veya kullanıcı brief'ine dayanmayan görünür eklemeler kalite kontrolünde reddedilir. Mutlak biçimde yalnızca korpustan üretildiği iddia edilmez.

## Kaynak sırası

1. Arda’nın o anki brief’i, net kısıtları ve sağladığı marka varlıkları.
2. Arda’nın özellikle gösterdiği veya onayladığı görsel örnekler.
3. Bu depodaki referans incelemeleri ve tasarım ilkeleri.
4. Genel tasarım bilgisi.

Bir referans, sayfadaki her ayrıntının kopyalanmasını veya her yeni işte kullanılmasını istemez. Kaynakların proje konusu, kompozisyonu ve marka öğeleri korunur; yalnızca brief’e aktarılabilen karar mantığı alınır.

## Çalışma sırası

1. DESIGN_DNA.md ve bu dosyayı oku.
2. İşin tek gönderi, carousel, seri ya da başka bir format olduğunu belirle.
3. Brief’le gerçekten ilişkili bir referans varsa ilgili bölümü REFERENCE_CASEBOOK.md içinde incele. İlgisiz referansları zorla kullanma.
4. Kaynaktan bir ana tasarım mekanizması seç; gerekliyse bir destekleyici karar ekle.
5. Kaynakta bırakılacak öğeleri açıkça belirle: marka, özgün metin, logo, karakter, fotoğraf, belirgin düzen veya başka ayırt edici imza.
6. Yeni konsepti brief’e özgü olarak kur ve QUALITY_RUBRIC.md ile gözden geçir.
7. Gerçek görsel istendiyse bu yönü sohbetin ImageGen aracına açık bir üretim promptu olarak aktar; istenen oranı, özneyi, hiyerarşiyi ve kullanıcı metnini belirt. Dönen görseli incele ve gerekiyorsa ImageGen ile yinele.

## Dosya haritası

- training/REFERENCE_CASEBOOK.md — dört kullanıcı referansının kaynak, görsel gözlem, aktarılabilir ilke ve taklit edilmeyecek öğe analizi.
- training/PORTFOLIO_FRONTIER_CASEBOOK.md — İlk dört turda örneklenen 37 Behance portfolyosu ve araştırma sınırları.
- training/PORTFOLIO_FRONTIER_CASEBOOK_2026-09-29.md — Beş ajan kolundan 50 yeni, tekilleştirilmiş portfolyo vakası; iki dosyada toplam 87 frontier vakası.
- training/VISUAL_ART_DIRECTION.md — konsept, görüntü, tipografi, renk, kompozisyon ve duygusal ton kararları.
- training/CAROUSEL_STORYTELLING.md — carousel ritmi, slayt rolleri, süreklilik ve varyasyon.
- training/REFERENCE_TRANSLATION.md — referans mekanizmasını yeni brief’e dönüştürme adımları.
- training/QUALITY_RUBRIC.md — çıktıyı eleştirmek için puanlama ve durdurucu hatalar.
- training/EVALUATION_SCENARIOS.md — 20 vakalı benchmark; doğru aktarım, araç seçimi, metin doğruluğu ve negatif kontrol senaryoları.
- training/EVALUATION_RUN_LOG.md — benchmark koşu kanıtı, ImageGen çıktısı, rubrik puanı ve düzeltme kayıtları.
- training/USER_FEEDBACK_LOG.md — Arda’nın açık tasarım geri bildirimleri, kapsamı ve uygulanan düzeltmeler.
- DESIGN_DNA.md — Arda’nın kısa, kalıcı ve genellenebilir tasarım tercihleri.

Portfolyo araştırma vakalarını, uzun portfolyo sunumlarını Instagram şablonlarına çevirmek için değil; özgün kompozisyon, tipografi, gezinme ve proje sunumu kararlarını değerlendirmek için kullan.

## İlk referans grubu

Arda bu dört Behance projesini eğitim referansı olarak seçti. Bunlar ortak bir renk paleti veya tek bir tasarım stili değildir. Birlikte öğrettikleri şey; brief’e uygun görsel fikri bulmak, tipografi ile görüntüyü aynı kompozisyonda çalıştırmak ve konuya göre farklı bir görsel dil seçmektir.

İnceleme tarihi: 2026-09-28. Proje sayfaları tarayıcıda görsel olarak incelendi; bazı sayfaların metin tabanlı web erişimi 403 döndürdü. Görseller depoya kopyalanmadı. Kaynak bağlantıları ve özgün analizler korundu. Behance sayfaları zamanla değişebilir.

## Yeni eğitim girdileri

Yeni bir örneği eklerken şu ayrımı koru:

- Gözlem: kaynakta gerçekten görülen karar.
- Yorum: bu kararın iletişimdeki olası işlevi.
- Aktarım: hangi brief koşulunda işe yarayacağı.
- Sınır: kaynağa özgü olarak kopyalanmaması gereken öğe.
- Arda’nın tercihi: kullanıcı açıkça beğendi, reddetti veya kalıcı eğitim girdisi yaptı mı?

Tek bir örnekten evrensel kural üretme. Kalıcı DNA’ya yalnızca tekrar kullanılabilir bir tercih veya açık kullanıcı yönlendirmesi ekle.

## Özge için kullanıcı geri bildirimiyle eğitim

Arda bir Özge çıktısını 'koru', 'değiştir' veya 'kaçın' diye değerlendirip gerekçe verdiğinde bu geri bildirim 'training/USER_FEEDBACK_LOG.md' dosyasına kaydedilir. Sessizlik veya Özge’nin kendi rubrik puanı kullanıcı tercihi sayılmaz. Tek işe özgü düzeltmeler vaka kaydında kalır; Arda’nın kalıcı dediği veya örnekler arasında tekrar eden tercih DESIGN_DNA.md dosyasına aktarılır ve ilgili senaryo yeniden değerlendirilir. Bu yöntem profil ve başvuru bağlamını geliştirir; model ağırlıklarını değiştirmez.
## Behance portfolyo araştırması — 2026-09-28

Kullanıcının verdiği Türkiye grafik tasarım portfolyo aramasından ilk iki turda 27 ayrı proje, üçüncü turda altı ve dördüncü turda dört yeni proje görsel olarak örneklenip vaka dosyasına kaydedildi; toplam 37 ayrı proje var. Arama 10.000+ sonuç içerdiği ve önerilen sıralaması değişebildiği için bu seçilmiş bir örneklemdir; tam arama denetimi değildir. Bazı vaka modülleri farklı araştırmacılar tarafından farklı derinlikte görüldü; kanıt sınırları her vaka içinde kayıtlıdır.

## Behance portfolyo araştırması — 2026-09-29 güncellemesi

Yeni beşinci araştırma turu, her biri 10 görsel olarak incelenmiş proje içeren beş raporu bir araya getirir. Yeni vaka havuzu önceki 41 Behance proje kimliğiyle tekilleştirildi; yeni vaka dosyası ve kaynak raporları Dosya haritasında bağlantılıdır. Özge, brief’e uyan vakaları seçmeli; örneklerdeki kaynak imzalarını kalıcı şablona çevirmemelidir.
