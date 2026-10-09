# Kıvanç Kuyumculuk Müşteri Takip Uygulaması

Bu klasör Flutter kaynak projesidir. Android APK üretmek için `.github/workflows/build-apk.yml` GitHub Actions iş akışı eklenmiştir.

## APK nasıl alınır?
1. ZIP dosyasını bilgisayarınıza çıkarın.
2. İçeriği yeni bir GitHub deposuna yükleyin.
3. GitHub deposunda **Actions** sekmesini açın.
4. **Android APK Build** iş akışını seçip **Run workflow** düğmesine basın (veya `main` dalına push edin).
5. İşlem tamamlanınca çalıştırmanın altındaki **Artifacts** bölümünden `kivanc-musteri-takip-apk` dosyasını indirin. ZIP içinden `app-release.apk` çıkar.

## Özellikler
- Müşteri formundaki alanları elle kaydetme ve düzenleme
- Kameradan fotoğraf çekme veya galeriden form seçme
- Cihaz üzerinde metin tanıma (Google ML Kit Latin metin tanıma; fotoğraf OCR servisine gönderilmez)
- Müşteri kayıtlarını cihazda tutma
- Arama, Excel (.xlsx) aktarımı
- Doğum günü, evlilik yıl dönümü ve eşin doğum günü için 7 gün önceden yerel bildirim planlama

## Önemli notlar
- Bu kaynak proje burada derlenmiş/test edilmiş bir APK değildir. Bulut derlemesi ve gerçek cihaz testi gerekir.
- OCR el yazısını veya bulanık fotoğrafları hatalı okuyabilir; kaydetmeden önce kontrol edin.
- Bildirimler izinlere ve Android pil optimizasyonlarına bağlıdır.
- Veriler uygulamanın özel alanında tutulur. Uygulamayı kaldırmak yerel kayıtları silebilir. Düzenli Excel yedeği alın.
- Android projesi GitHub Actions sırasında `flutter create` ile oluşturulur. iPhone derlemesi için macOS ve Xcode gerekir.
