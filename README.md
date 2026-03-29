

4)Ay Üzerinden Yer Bulunması:
Ay üzerinde GPS vb. yol bulma servisleri bulunmadığı için. Ayın Doğrudan lokasyonunun bulunulmaıs gerekmektedir. Bu Sebepten Ötürü FederNet mimarisi tercih edilmiştir. Bu Mimarinin başlıca kısımları şunlardır
3.1)Krater Tespit
Öncelikle uydu Görüntülerinin tespiti gerekmektedir. Bunun için 1 içinde bahsedilen Yolo Modeli kullanılmıştır

3.2)Krater Eşleştirme Algoritması
Yeryüzünden Çekilen görselde bulunan Kraterler ile Gökyüzünden çekilen görseller eşleştirilir. Böylece Görselin nereden çekildiğine dair genel bir bilgi edinilir

3.3)Konum Bulma Algoritması
Bu İki kısım birleştirilerek Net kordinat bulunur


Veri setini oluşturan kurum(lar)= Nan

Veri seti/çalışma makalesi=https://www.sciencedirect.com/science/article/pii/S1389128626000071




Buna uygun 350 Desription yaz githuba

Ay üzerinde GPS benzeri konumlandırma sistemlerinin bulunmaması, alternatif ve yenilikçi çözümleri zorunlu kılmaktadır. Bu proje, Ay yüzeyinde konum belirleme problemini çözmek amacıyla geliştirilen FederNet mimarisine dayanmaktadır. FederNet yaklaşımı, farklı veri kaynaklarını ve algoritmaları bir araya getirerek yüksek doğrulukta konum tahmini yapmayı hedefler. Sistem üç temel bileşenden oluşmaktadır: krater tespiti, krater eşleştirme ve konum bulma algoritmaları.

İlk aşamada, Ay yüzeyine ait uydu görüntüleri üzerinde kraterlerin tespiti gerçekleştirilir. Bu işlem için derin öğrenme tabanlı YOLO (You Only Look Once) modeli kullanılmıştır. YOLO modeli, hızlı ve doğru nesne tespiti yapabilme yeteneği sayesinde kraterleri yüksek başarı oranıyla belirleyebilmektedir. Bu sayede Ay yüzeyine ait önemli coğrafi işaretler otomatik olarak çıkarılır.

İkinci aşamada, yeryüzünden elde edilen görüntüler ile uydu görüntülerindeki kraterler arasında eşleştirme yapılır. Bu eşleştirme süreci, görüntüler arasındaki benzerlikleri analiz ederek çekim noktasının yaklaşık konumunu belirlemeyi sağlar. Kraterlerin şekil, boyut ve konum özellikleri bu süreçte kritik rol oynar.

Son aşamada ise, krater tespiti ve eşleştirme sonuçları birleştirilerek kesin koordinat hesaplaması yapılır. Bu konum bulma algoritması, elde edilen verileri optimize ederek mümkün olan en doğru sonucu üretir.

Bu çalışma, Ay üzerinde otonom navigasyon sistemlerinin geliştirilmesine katkı sağlamayı amaçlamakta olup, gelecekteki uzay görevleri için önemli bir temel oluşturmaktadır. Veri seti ve metodoloji, ilgili akademik çalışma üzerinden incelenebilir.


Olm biraz daha Güzel yaz estetik girdili çıktılı emojili

🚀 Ay Üzerinde Konumlandırma (FederNet Tabanlı Navigasyon Sistemi) 🌕

Ay yüzeyinde 🌍 GPS benzeri sistemlerin bulunmaması, klasik konum belirleme yöntemlerini kullanılamaz hale getirir. Bu proje, tam da bu soruna çözüm getirmek için geliştirilmiş yenilikçi bir yaklaşım sunar: FederNet mimarisi. Amaç, yalnızca görsel verilerden yararlanarak 📍 yüksek doğrulukta konum tespiti yapabilmektir.

🧠 Sistem Mimarisi
FederNet, üç temel bileşenin birleşimiyle çalışır:

🔍 1) Krater Tespiti
Ay yüzeyine ait 🛰️ uydu görüntüleri analiz edilir

⚡ Hızlı ve etkili sonuçlar için YOLO (You Only Look Once) modeli kullanılır

📌 Kraterler otomatik olarak tespit edilir ve işaretlenir

🔗 2) Krater Eşleştirme
📸 Yeryüzünden çekilen görüntüler ile uydu verileri karşılaştırılır

🧩 Kraterlerin şekil, boyut ve konum özellikleri analiz edilir

📍 Görüntünün yaklaşık çekildiği konum belirlenir

📐 3) Konum Bulma Algoritması
🔄 Önceki iki aşamanın çıktıları birleştirilir

🧮 Optimizasyon algoritmaları kullanılarak kesin koordinatlar hesaplanır

🎯 Yüksek doğrulukta konum tahmini elde edilir

⚙️ Girdi & Çıktı
📥 Girdi:

Ay yüzeyine ait uydu görüntüleri

Yeryüzünden çekilmiş krater görüntüleri

📤 Çıktı:

📍 Tahmini konum bilgisi

🎯 Net koordinat verisi

🌌 Projenin Önemi
Bu sistem:

🚀 Gelecekteki Ay görevleri için otonom navigasyon sağlar

🤖 İnsan müdahalesine gerek kalmadan konum belirleyebilir

🛰️ Uzay keşiflerinde yeni nesil yön bulma teknolojilerine temel oluşturur

📚 Referans Çalışma:
https://www.sciencedirect.com/science/article/pii/S1389128626000071

✨ Bu proje, uzay teknolojileri ve yapay zekânın birleşimiyle, Ay’da “GPS’siz navigasyon” problemini çözmeyi hedefleyen güçlü bir adımdır.



