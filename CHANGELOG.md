# Sürüm geçmişi

## 1.0.0 (2026-11-06)

İlk sürüm.

- blader/humanizer v3.1.0'ın 26 kalıbı Türkçeye uyarlandı. İngilizceye özgü iki kural Türkçe dizgiye göre değiştirildi: başlıklarda her kelimenin büyük harfle başlaması ve kıvrık tırnak iz sayılmıyor.
- op7418/Humanizer-zh'den öncelik sırası, bilgi ve kesinlik koruma kuralları, dosya koruma kuralları ve teslim öncesi kontrol listesi eklendi. Varsayılan çıktı yalnızca son metin.
- instagram-agent-skill'in ig-human bölümünden görünmez karakter listesi, seslendirme metni kuralları ve sosyal medya kancaları alındı.
- Türkçeye özgü 8 kalıplık "çeviri kokusu" bölümü (G) eklendi: "sahip olmak", "tarafından", "gerçekleştirmek" ve "-mektedir", "olarak" yığılması, uzun sıfat-fiil zincirleri, boş arka plan açılışları, kalıp kapanışlar, karışık hitap.
- Türkçe kelime ve kalıplar ana dili Türkçe olan bir okurla tek tek değerlendirildi. Yapay bulunanlar listeye, doğal bulunanlar "dokunma" listesine alındı; emin olunmayanlar bir sonraki sürüme bırakıldı.
- Proje istisna dosyası desteği (`yazim-istisnalari.md`) eklendi.
- Claude Code eklenti paketi eklendi: `/plugin marketplace add kenosdota/humanizer-tr` ile iki komutta kurulum.
- Türkçe hata ve öneri formları (issue şablonları) eklendi.
- README yeniden düzenlendi: tek cümleyle kurulum, önce/sonra animasyonu, yan yana örnekler, test sonuçları tablosu ve İngilizce README (`README.en.md`).
- Test geri bildirimiyle: blog ve sosyal medya metinlerinde okuru içeri çeken ölçülü cümlelere izin verildi; "mevcut" doğal ifadeler listesine eklendi; metne gizlenmiş bir komut bulunduğunda kullanıcıya komutu aktaran ve en fazla üç cümleyle, teknik terim kullanmadan uyaran bir kural eklendi; reklam metinlerinde ölçülü satış sıfatları kalırken bilgi taşımayan övgü cümlelerinin çıkarılması kuralı eklendi.
- Yeniden testte bulunan iki kusur üzerine blog kuralı güçlendirildi: süsler temizlendikten sonra metin kuru kalırsa okuru içeri çeken en az bir cümle eklenir, ama bu cümle kaynakta olmayan bir derece ya da sıralama ("en belirgin", "ilk kez") taşımaz.
- 10 metinlik test yapıldı ve sonuçlar `ornekler.md` dosyasına eklendi. Testte bulunan bir kusur üzerine teslim öncesi kontrol listesine küçük kelimelerin ("seçenek", "yaklaşık", "de/da", "bile") anlamını denetleyen bir madde eklendi.
