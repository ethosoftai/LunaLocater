Ay Üzerinde Konumlandırma (FederNet Tabanlı Navigasyon Sistemi) 
Ay yüzeyinde GPS benzeri sistemlerin bulunmaması, klasik konum belirleme yöntemlerini kullanılamaz hale getirir. Bu proje, tam da bu soruna çözüm getirmek için geliştirilmiş yenilikçi bir yaklaşım sunar: FederNet mimarisi. Amaç, yalnızca görsel verilerden yararlanarak  yüksek doğrulukta konum tespiti yapabilmektir.
Sistem Mimarisi
FederNet, üç temel bileşenin birleşimiyle çalışır:

Ay yüzeyine ait  uydu görüntüleri analiz edilir.

⚡Hızlı ve etkili sonuçlar için YOLO (You Only Look Once) modeli kullanılır.

Kraterler otomatik olarak tespit edilir ve işaretlenir.

Krater Eşleştirme (Match)

Yeryüzünden çekilen görüntüler ile uydu verileri karşılaştırılır.

Kraterlerin şekil, boyut ve konum özellikleri analiz edilir.

Görüntünün yaklaşık çekildiği konum belirlenir.

Konum Bulma Algoritması (KalmanFilter & find_position)

Önceki iki aşamanın çıktıları birleştirilir.

Optimizasyon algoritmaları ve Genişletilmiş Kalman Filtresi (EKF) kullanılarak kesin koordinatlar hesaplanır.

Yüksek doğrulukta konum tahmini elde edilir.

Girdi & Çıktı
Girdi:

Ay yüzeyine ait uydu görüntüleri

Yeryüzünden çekilmiş krater görüntüleri

Çıktı:

Tahmini konum bilgisi

Net koordinat verisi (İlgili CSV dosyalarında raporlanır, örn: Pos_Err_...csv)

Nasıl Çalıştırılır? (Kurulum ve Kullanım)
Proje, temel olarak Jupyter Notebook dosyaları üzerinden modüler bir şekilde çalıştırılmaktadır.

Gereksinimler
Python 3.x

Jupyter Notebook veya JupyterLab

İlgili Python kütüphaneleri (Projeyi çalıştırmadan önce YOLO, OpenCV, Pandas, Numpy ve poliastro gibi bağımlılıkların kurulu olduğundan emin olun.)

Çalıştırma Adımları
Projeyi Klonlayın:

Bash
git clone https://github.com/ethosoftai/LunaLocater.git
cd LunaLocater
Ayarları Yapılandırma:

Çalışmaya başlamadan önce hiperparametreleri ve yolları yapılandırmak için settings.ipynb dosyasını kontrol edin.

Veri Seti ve Katalog Hazırlığı (İlk Kurulum):

Veri setini oluşturmak veya düzenlemek için: create_datasets.ipynb

Krater kataloglarını incelemek için: Crater_Catalogs.ipynb

Model Eğitimi (Opsiyonel):

Kendi YOLO modelinizi veya eşleştirme modelinizi sıfırdan eğitmek isterseniz training.ipynb dosyasını çalıştırın.

Ana Testler ve Navigasyon:
Projeyi uçtan uca çalıştırmak ve sonuçları görmek için aşağıdaki ana Notebook'ları kullanabilirsiniz:

Ana Akış: main.ipynb (Sistemin temel çalışma akışı)

Genişletilmiş Kalman Filtresi (EKF) Testi: main_EKF.ipynb (Daha hassas konumlandırma tahmini için EKF algoritmasının çalıştırılması)

Tüm Testleri Koşma: run_all_test.ipynb (Toplu test senaryolarını başlatır)

Not: Spesifik modülleri test etmek için match.ipynb, find_position.ipynb veya kf.ipynb dosyalarını bağımsız olarak da çalıştırabilirsiniz.

Projenin Önemi
Bu sistem:

Gelecekteki Ay görevleri için otonom navigasyon sağlar.

İnsan müdahalesine gerek kalmadan konum belirleyebilir.

Uzay keşiflerinde yeni nesil yön bulma teknolojilerine temel oluşturur.

Referans Çalışma:
ScienceDirect - Article Reference
