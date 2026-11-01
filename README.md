# HUNTER RACING · GitHub'dan otomatik APK

**Önce [`BURADAN_BASLA.txt`](BURADAN_BASLA.txt) dosyasını oku.**

Bu repo, HUNTER GAMES için çevrimdışı 3D mobil yarış prototipi ve onu Android APK'ya çeviren GitHub Actions iş akışını içerir.

## GitHub'a yükle ve Android APK üret

1. Bu kaynak ZIP'i **aç** ve içindeki **tüm dosyaları** GitHub deposunun köküne yükle (`.github` dahil).
2. `main` veya `master` dalına `Commit changes` yap.
3. **Actions → HUNTER RACING - APK OLUSTUR** iş akışını aç. Otomatik başlamazsa **Run workflow**.
4. Yeşil tikli işin **Artifacts → HUNTER-RACING-debug** çıktısını indir.
5. İndirilen ZIP'in içinde örnekteki gibi **tek `app-debug.apk`** olacaktır.

## İçerik

- `web/`: Tamamen offline WebGL/HTML5 HUNTER RACING oyun prototipi (3 araç, 4 oyun modu, 4 kamera, nitro, drift, garaj, ayarlar ve botlar).
- `app/`: Native Android WebView kabuğu ve ikon; yatay/tam ekran, yerel dosya yüklemesi.
- `.github/workflows/android-apk.yml`: Her push'ta test eder, **debug APK** üretir, artifact ZIP olarak sunar.
- `tests/smoke.js`: JavaScript sürüş/oyun açılış otomatik testi.

## Web sürümünü bilgisayarda aç

`web/index.html` dosyasını Chrome'da aç veya `web` klasöründe `python -m http.server 8080` çalıştır.

## Durum / kapsam

Bu bir **ilk oynanabilir prototiptir**, tamamlanmış bir CarX Street / Asphalt klonu ya da online açık dünya ürünü değildir. APK'nın gerçek cihaz testi ve GitHub derlemesi bu ortamda yapılamadı. GitHub Actions çıktısı **debug APK** olup Play Store için dağıtıma uygun imzalı sürüm değildir.
