# -court-on-the-island
# ⚖️ Adalı Mahkeme Maliyet Analizi

Bu proje, karmaşık bir hukuk senaryosu üzerinden beraat kararını garanti altına almak için en düşük maliyetli stratejiyi hesaplayan interaktif bir web simülatörüdür. Uygulama, algoritmik verimlilik ile kullanıcı dostu tasarımı birleştirerek 15 farklı senaryoyu saniyeler içinde analiz eder.

##  Proje Amacı ve Kapsamı
Projenin temel amacı, 5 farklı hâkimin rüşvet eğilimleri ve jüri oylama kuralları ışığında, sanığın beraat etmesini sağlayacak en ekonomik yolu bulmaktır. Yazılım, girilen parametrelere göre hem jüriyi hem de hâkimi ikna etme maliyetlerini optimize eder.

##  Teknik Özellikler
* **Dil:** Saf JavaScript (Vanilla JS), HTML5, CSS3.
* **Tasarım:** Modern, minimalist ve mobil uyumlu (Responsive) arayüz.
* **Algoritma:** Her bir hâkim için üç ana strateji (Beraat, Çekimserlik, Suç Kararı) üzerinden toplam 15 farklı maliyet olasılığı hesaplanır.

##  Hesaplama Mantığı ve Kurallar
Uygulama, beraat sonucuna ulaşmak için şu üç yolu analiz eder:

1.  **Doğrudan Beraat:** Hâkime rüşvet verilerek doğrudan beraat kararı alınması (Sadece Hâkim Bedeli).
2.  **Çekimserlik:** Hâkimin çekimser kalması sağlanır ve jüri üyelerinin %50'den fazlası (n/2 + 1) beraat için ikna edilir (Hâkim + Jüri Bedeli).
3.  **Suçlu Kararına Direnme:** Hâkim suçlu dese dahi jürinin %100'ü ikna edilerek beraat sağlanır (Sadece 100% Jüri Bedeli).

##  Dosya Yapısı
* `index.html`: Uygulamanın temel iskeleti ve veri giriş alanları.
* `css/styles.css`: Indigo/Lacivert temalı, kullanıcı deneyimi odaklı görsel tasarım.
* `js/app.js`: Tüm matematiksel hesaplamaları ve DOM manipülasyonunu yürüten ana motor.
* `README.md`: Proje dokümantasyonu.

##  Başlatma ve Kullanım
1.  Projeyi yerel bilgisayarınıza indirin.
2.  `index.html` dosyasını herhangi bir modern web tarayıcısı ile açın.
3.  **Jüri Sayısı** ve **Jüri Başına Rüşvet** bedelini girin.
4.  Hâkimlerin beraat ve çekimserlik bedellerini belirleyin.
5.  **"En Ucuz Yolu Hesapla"** butonuna basarak optimum stratejiyi görüntüleyin.
