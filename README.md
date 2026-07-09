# 🧪 Piksel Simyacısı (Pixel Alchemist) V3.1

HTML5 Canvas ve Vanilla JavaScript kullanılarak sıfırdan geliştirilmiş, dış kütüphane bağımlılığı olmayan, 2.5D yoğunluk tabanlı bir hücresel otomat (cellular automata) simülasyonu. 

Klasik "falling sand" (düşen kum) mekaniklerini; kimyasal reaksiyonlar, dahili komut satırı ve oyuncuyu keşfetmeye iten bir **Başarım (Achievement) Sistemi** ile birleştirir.

## ✨ Öne Çıkan Özellikler

* **🏆 Başarım Sistemi:** Oyuncuların yeni element etkileşimlerini keşfetmesini ödüllendiren entegre sistem ("Simyacı", "Patlama Ustası", "Bahçıvan" vb.). Başarımlar tarayıcı hafızasına (`localStorage`) kaydedilir.
* **Fizik ve Yoğunluk Motoru:** Toz, sıvı, gaz ve sabit maddeler kendi yoğunluklarına göre mantıklı bir şekilde yer değiştirir ve birbirlerinin içinden geçebilir.
* **Dinamik Reaksiyonlar:** Tohumların suda filizlenmesi, ateşin kumu cama dönüştürmesi, lav ve suyun buluşmasıyla buhar/taş oluşumu gibi sayısız zincirleme tepkime.
* **2.5D Görsel Derinlik:** Piksellerin sadece düz renklerden ibaret olmaması için ışık/gölge illüzyonu yaratan özel bir kaplama algoritması.
* **Sıfır Dış Kaynaklı Ses:** Tüm ses efektleri (patlama, su sıçraması, başarım kazanımı) hiçbir `.mp3` veya `.wav` dosyası kullanılmadan, tamamen matematiksel olarak **Web Audio API** ile anlık sentezlenir.
* **API Shell (Konsol):** Dahili komut satırı üzerinden simülasyonu yönetebilir, kendi kurallarını belirlediğin "Özel Elementler" (Custom Elements) yaratıp oyuna ekleyebilirsin.

## 🚀 Kurulum ve Çalıştırma

Proje tamamen istemci tarafında (client-side) çalışır. Hiçbir sunucu kurulumuna, Node.js modülüne veya derleyiciye ihtiyacınız yoktur.

1. Bu depoyu klonlayın veya indirin.
2. `index.html` dosyasını favori modern tarayıcınızda (Chrome, Firefox, Edge, Safari) açın.
3. Elementlerinizi seçin, fırça boyutunu ayarlayın ve reaksiyonları izleyin!

## 🎮 Kontroller ve Komut Satırı

Oyun ekranındaki arayüzü kullanarak her şeyi kontrol edebilirsiniz. Ek olarak konsola (API Shell) aşağıdaki gibi komutlar girebilirsiniz:

* `yardim` - Tüm komut listesini gösterir.
* `eleman-ekle [isim] [#renk] [tip] [yogunluk] [yanici]` - Kendi elementini yarat! (Örn: `eleman-ekle civa #c0c0c0 sivi 8 hayir`)
* `bomba 50 50 10` - X:50, Y:50 koordinatlarına 10 yarıçapında bomba yerleştirir.

## 🤝 Geliştirme Süreci

Bu simülasyon motoru, performanslı Canvas çizimi ve Vanilla JS limitlerini test etmek amacıyla oluşturulmuştur. Geliştirme sürecinin mantıksal kurgusu ve algoritmik yapısı oluşturulurken **Claude AI** ile eşli programlama (pair programming) yapılmıştır. Yeni reaksiyon fikirlerine ve performans iyileştirmesi (Pull Request) yapacak herkese açıktır!
