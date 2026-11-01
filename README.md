# HUNTER RACING | GitHub'a direkt yükleme

Bu ZIP bir üst HUNTER_RACING_V1 klasörü içermez. Çıkardığınız dosyalar doğrudan GitHub deposunun ana dizinine konulacaktır.

## 1) Oyun kaynakları
ZIP'i açın. `app/`, `web/`, `tests/`, `build.gradle`, `settings.gradle`, `gradle.properties` ve diğer dosyaları GitHub'a yükleyin. Android için gerekli alt klasörleri birleştirmeyin.

## 2) YML dosyası ayrı verildi
Ayrıca indirilen `android-apk.yml` dosyasını GitHub'da şu **tam yola** koyun:

`.github/workflows/android-apk.yml`

GitHub'da **Add file > Create new file** deyip dosya adı olarak `.github/workflows/android-apk.yml` girin ve ayrı YML dosyasının içeriğini yapıştırıp kaydedin.

## 3) APK alma
Actions > HUNTER RACING - APK OLUSTUR > Run workflow. Başarılı derlemenin `HUNTER-RACING-debug` artifact'ini indirin. GitHub, `app-debug.apk` dosyasını içeren ZIP verecek.

Bu ZIP bir APK değildir. GitHub'da Android SDK ile gerçek derleme yapılacak. İlk sürüm 3D tek oyunculu prototiptir; online mod henüz bulunmaz.
