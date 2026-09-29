# Tasarım Eleştiri Rubriği

Taslağı 0–4 arasında puanla. Bu rubrik otomatik “PASS” üretmez; geliştirme alanlarını bulmak ve bariz başarısızlığı durdurmak içindir.

- **0 — Yok/yanlış:** ölçüt sağlanmıyor veya brief’e aykırı.
- **1 — Zayıf:** kısmen mevcut, fakat ana problem sürüyor.
- **2 — Çalışır:** kullanılabilir ancak belirgin geliştirme payı var.
- **3 — Güçlü:** bilinçli, tutarlı ve brief’e uygun.
- **4 — Çok güçlü:** tasarım kararları özgün, net ve birlikte çalışıyor.

## Ölçütler

1. **Brief ve konu doğruluğu:** Sektör, hedef kitle, mesaj, metin ve kullanıcı kısıtları doğru mu?
2. **Özgün ana fikir:** Kompozisyonun bir fikri var mı; fikir yalnızca “güzel renk + büyük başlık”tan ibaret mi?
3. **Görüntünün tasarım görevi:** Görsel içerik atmosfer, kanıt, anlatı veya metafor olarak iş yapıyor mu; tipografi ve grafik yapıyla tek bir tasarım kompozisyonuna dönüşüyor mu?
4. **Tipografi ve hiyerarşi:** İlk bakış, başlık, açıklama ve CTA görevleri ayrılıyor mu; Türkçe ve mobil okunurluk korunuyor mu?
5. **Duygusal ve kültürel uygunluk:** İnsanlar, hassas konular, topluluk ve marka bağlamı özenli temsil ediliyor mu?
6. **Kompozisyon ve ritim:** Ölçek, boşluk, crop, katman ve kontrast kontrollü mü? Carousel ise süreklilik ve varyasyon dengeli mi?
7. **Referanstan özgün aktarım:** Kaynaktan yalnızca aktarılabilir mekanizma mı alınmış, yoksa tanınabilir yüzey/şablon mu kopyalanmış?
8. **Sistem tutarlılığı:** Renk, font rolleri, görsel malzeme ve işaretler bir arada gerekçeli mi?
9. **Üretim ve dosya dürüstlüğü:** Gerçek görsel istenmişse sohbetin ImageGen aracı kullanılmış ve dönen görsel incelenmiş mi? Üretilmeyen asset veya yapılmayan QA iddiası var mı?
10. **Deneyin gerekçesi:** Kullanıcı cesur yön istediğinde ana kompozisyon hamlesi mesajı güçlendiriyor mu; okunurluk ve konu doğruluğu korunuyor mu? Deney istenmediyse tasarım gereksiz karmaşık mı?

## Durdurucu hatalar

Aşağıdakilerden biri varsa yüksek toplam puan taslağı kurtarmaz:

- Kullanıcının sağladığı gerçek metin/logo/tarih/fiyat değiştirilmiş veya uydurulmuş.
- Sektör brief’i, sektörle ilgisiz soyut görsel ile geçiştirilmiş.
- Bir referansın tanınabilir ana düzeni, markası veya görsel varlığı izinsiz yeniden kullanılmış.
- Psikoloji/yas gibi hassas içerikte iyileşme garantisi, istismar edici satış dili veya gerçek olmayan uzmanlık eklenmiş.
- Başlık ya da gerekli içerik telefonda okunmuyor.
- Arda design-forward bir yön isterken sonuç yalnızca bir sahne/fotoğraf ve üzerine yerleştirilmiş başlık olarak kalmış.
- ImageGen yerine görsel elle hazırlanmış veya başka bir araç kullanıcıya söylenmeden tercih edilmiş.
- ImageGen çıktısı alınmadan görsel üretildiği ya da incelenmediği hâlde QA yapıldığı iddia edilmiş.
- Asistan, üretmediği dosya, uygulamadığı düzeltme veya yapmadığı görsel inceleme hakkında başarı iddia etmiş.
- “Deneysel” etiketiyle başka bir referansın imza paleti/yerleşimi kopyalanmış veya zorunlu metin okunamaz hâle gelmiş.

## Yeniden çalışma kuralı

Herhangi bir ana ölçüt 0 veya 1 ise ya da durdurucu hata varsa sunumdan önce düzelt. Düzeltme sırasında her şeyi yeniden tasarlamak yerine başarısız ölçütü hedefle; ancak ana konsept hatalıysa kompozisyonu baştan kur.


## Benchmark için puan eşiği

On ölçütü 0–4 puanla ayrı ayrı değerlendir; toplam en fazla 40 puandır.

- PASS: En az 30/40, hiçbir ölçüt 0 veya 1 değil ve sert hata yok.
- STRONG: En az 34/40, hiçbir ölçüt 0 veya 1 değil ve sert hata yok.
- FAIL: 30 puanın altı, herhangi bir ölçütte 0–1 veya herhangi bir sert hata.
- UNPROVEN: Gerekli fixture, gerçek ImageGen çıktısı ya da görsel inceleme kanıtı yok. Eksik kanıtı PASS kabul etme.

ImageGen'in çağrılmaması gereken vakada aracı çağırmak; görsel beklenen vakada yalnızca prompt verip üretim iddia etmek davranış hatasıdır. Bu durumlar ilgili vakayı FAIL yapar. Tam metin, oran/varlık kontrolü ve doğru araç davranışı gözlenebilir kontrollerdir; özgünlük, kompozisyon ve görsel kalite rubrik yargısıdır.

