# MATRIX BROWSER v0.2 — Android kaynak projesi

Bu bir APK dosyası değil; Android Studio/Gradle ile derlenmek üzere hazırlanmış kaynak projedir.
Bu çalışma ortamında Android SDK ve Gradle kurulu olmadığı için burada APK derlenemedi.

## v0.2 özellikleri
- Android System WebView (Chromium tabanlı) ile gerçek web sayfaları
- Adres çubuğu ve Google araması
- Geri / ileri / yenile
- Birden fazla WebView sekmesi, sekme seçme ve kapatma
- Yer imleri ve basit gezinme geçmişi
- WebView indirme olaylarını Android DownloadManager'a aktarma
- ChatGPT'nin resmî sitesini yeni sekmede açma
- HTTPS odaklı gezinme, karma içerik engeli, dosya erişiminin kapatılması ve Safe Browsing

## Önemli sınırlar
- ChatGPT düğmesi ChatGPT web sitesini açar. Kullanıcı hesabının aboneliğini veya yetkisini başka uygulamaya aktarmaz.
- Bu sürümde sayfaları kendi başına okuyup tıklayan bir AI ajanı YOKTUR. Bunun için ayrı bir AI servisi/API, sayfa içeriği izinleri, güvenli komut katmanı ve kullanıcı onayları eklenmelidir.
- Gizli mod henüz eklenmedi. Bu sürümde geçmiş kaydedilir.
- WebView motoru cihazdaki Android System WebView/Chrome bileşenine bağlıdır.

## APK derleme (tablet üzerinden)
Bu projeyi bir GitHub deposuna yükle:
1. GitHub'da yeni bir repository oluştur.
2. ZIP'i çıkarıp içindeki dosyaları depo köküne yükle.
3. `Actions` sekmesini aç.
4. `Build MATRIX BROWSER APK` iş akışını çalıştır (`Run workflow`).
5. İşlem başarılı olunca `MATRIX-BROWSER-APK` artifact'ini indir.
6. Artifact ZIP'ini çıkar ve `app-debug.apk` dosyasını tabletine kur.

İş akışı GitHub Actions üzerinde Java 17, Gradle 8.9 ve Android SDK kullanır.
