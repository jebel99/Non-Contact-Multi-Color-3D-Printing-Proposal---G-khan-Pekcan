📜 Açık Kaynak Teknik Önerisi: Yüzey Dokulandırma ve Çift Püskürtmeli Kaplama Yöntemiyle Temassız Çok Renkli FDM Baskı
Mucit / Yazar: Gökhan Pekcan

İletişim: pekcan4@hotmail.com / jebelwot@gmail.com

Yayın Tarihi: 26 Ekim 2026

Lisans: MIT Lisansı

1. Yönetici Özeti
Mevcut çok renkli FDM çözümleri, yüksek atık miktarına, yavaş baskı sürelerine ve mekanik karmaşıklığa yol açan, takım değiştirme veya filament geri çekme mekanizmalarına (örneğin, Bambu AMS, Prusa MMU) büyük ölçüde bağımlıdır.

Bu öneri, Gökhan Pekcan tarafından tasarlanan, atık miktarını tamamen ortadan kaldıran, temassız, düşük maliyetli, çok renkli bir son işlem sistemini sunmaktadır. Algoritmik yüzey mikro dokulandırmayı (Dilimleyici seviyesi) soğuk bölge çift püskürtmeli dağıtım sistemiyle (Pigment + Stabilizatör) birleştirerek, herhangi bir standart tek ekstrüderli FDM yazıcı çok renkli çıktı elde edebilir.

2. Sistem Mimarisi ve 3 Adımlı İş Akışı
[ Adım 1: Mikro Doku Oluşturma ] ---> [ Adım 2: Pigment Püskürtme ] ---> [ Adım 3: Sıvı Sızdırmazlık ]
(Dilimleyici Bulanık Yüzey / Gözenek) (Soğuk Bölge Püskürtme / Kılcal)  (Temassız Stabilizatör Vernik)
Adım 1: Algoritmik Yüzey Doku Oluşturma (Lazer Gerekmez)
Mekanizma: Karmaşık lazer ablasyonu kullanmak yerine, dilimleyici mikro titreşimler (özelleştirilmiş Bulanık Yüzey / alt ekstrüzyon algoritmaları) kullanarak dış çevre yollarını değiştirir.

Amaç: Pigmentler için mekanik bir alıcı görevi görecek şekilde taze plastik duvarda mikro gözenekli dokular ve kılcal kanallar oluşturur.

Adım 2: Soğuk Bölge Pigment Püskürtme (Temassız)
Termal İzolasyon: Pigment rezervuarları ve mikro jet vanaları, termal bozulmayı ve nozul tıkanmasını önlemek için ısı bariyerinin arkasındaki Soğuk Bölgeye yerleştirilir.

Biriktirme: Yüksek hızlı mikro jetler, sıvı pigmenti (veya uçucu çözücü bazlı mürekkebi) doğrudan hedef mikro gözenekli yüzeye uygular.

Kılcal Emilim: Gözenekli plastik, kılcal etki yoluyla pigmenti anında emer. Baskılı duvardan gelen ısı, çözücünün hızlı buharlaşmasını tetikler.

Adım 3: Temassız Sıvı Stabilizasyonu (Sızdırmazlık)
Mekanizma: Baskı deformasyonunu ve sürtünmeyi önlemek için mekanik ütüleme araçlarını ortadan kaldırır.

Uygulama: İkinci bir mikro jet, ultra ince, hızlı kürlenen şeffaf bir stabilizatör (akrilik/poliüretan vernik tabakası) bırakır.

Sonuç: Pigment parçacıklarını mikro gözeneklerin içinde kalıcı olarak kilitler ve pürüzsüz (parlak, saten veya mat) bir dış yüzey bırakır.

3. Mevcut Sistemlere Göre Başlıca Avantajlar
Özellik	Geleneksel Sistemler (AMS / MMU)	Bu Öneri (Gökhan Pekcan)
Atık Arındırma	Son Derece Yüksek (Arındırma Kuleleri)	Sıfır (%0)
Takım Kafası Ağırlığı	Ağır (Birden fazla motor/ekstrüder)	Hafif (2x Mikro-Jet Valf)
Baskı Hızı	Yavaş (Sürekli geri çekme/değiştirme)	Hızlı (Sürekli ekstrüzyon yolu)
Mekanik Aşınma	Yüksek (Filament taşlama)	Sıfır Temas (Akışkan Dinamiği)
Maliyet ve Uyarlama	Yüksek ($300 - $1000+)	Düşük (Standart yazıcılar için eklenti)
4. Topluluk İşbirliği Çağrısı (Açık Yol Haritası)
Geliştiricileri, üreticileri ve araştırmacıları aşağıdaki konularda denemeler yapmaya teşvik ediyoruz:

Dilimleme Eklentileri: Optimum kılcal pigment emilimi için Bulanık Cilt (Fuzzy Skin) parametrelerinin ince ayarı.

Pigment Kimyası: Sıcak PLA/PETG yüzeylerinde yüksek uçuculuklu solvent mürekkepleri ile mikro pigment süspansiyonlarının test edilmesi.

Püskürtme Entegrasyonu: Açık kaynaklı baskı kafalarına mikro piezo veya solenoid valflerin monte edilmesi (örneğin Voron Stealthburner).
