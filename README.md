# Nebula Space Arcade — Android WebView Project

Bu proje **NEBULA HTML TO APK** tarafından üretilmiştir.
%100 Ücretsiz, açık ve reklamsız yerel Android Studio projesidir.

---

## 🚀 APK Nasıl Derlenir? (3 Ücretsiz Yol)

### Yöntem 1: Android Studio ile (Önerilen & Kolay)
1. Bu ZIP arşivini bilgisayarınızda bir klasöre çıkarın.
2. [Android Studio](https://developer.android.com/studio)'yu açın.
3. **Open** butonuna basarak çıkarttığınız `Nebula_Space_Arcade` klasörünü seçin.
4. Gradle senkronizasyonu tamamlandıktan sonra üst menüden:
   **Build > Build Bundle(s) / APK(s) > Build APK(s)**
   seçeneğine tıklayın.
5. Birkaç saniye içinde APK'nız hazır olacak! Sağ alttaki bildirimden **locate** linkine basarak APK dosyanıza ulaşabilirsiniz.

### Yöntem 2: GitHub Actions ile (Bilgisayarınıza Android Studio Kurmadan!)
1. Bu klasörü bir GitHub deposuna yükleyin (Push).
2. İçindeki `.github/workflows/build-apk.yml` dosyası otomatik olarak tetiklenir.
3. GitHub reponuzun **Actions** sekmesine gidin.
4. Derleme tamamlandığında **Artifacts** kısmından doğrudan `Nebula_Space_Arcade-debug-apk` dosyasını indirin!

### Yöntem 3: Komut Satırı / Terminal ile
Klasör dizininde terminali açıp şu komutu çalıştırın:
```bash
# Linux / macOS
./gradlew assembleDebug

# Windows
gradlew.bat assembleDebug
```
Çıktı APK konumu:
`app/build/outputs/apk/debug/app-debug.apk`

---

## 🔑 Google Play Store için İmzalı Sürüm (Release APK / AAB)
Release APK üretmek için bir Keystore oluşturup `./gradlew assembleRelease` çalıştırabilirsiniz:

```bash
keytool -genkey -v -keystore nebula-release.jks -alias com.nebula.spacearcade -keyalg RSA -keysize 2048 -validity 10000
```

---

## ⚙️ Yapılandırma Bilgileri
- **Uygulama Adı:** Nebula Space Arcade
- **Paket Kimliği (Application ID):** `com.nebula.spacearcade`
- **Sürüm:** 1.0.0 (Kod: 1)
- **Min SDK:** 24 (Android 7.0+)
- **Target SDK:** 34 (Android 14)
- **Tema Rengi:** #7c3aed
