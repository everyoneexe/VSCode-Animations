# VSCode Animasyonları - Kurulum Rehberi

<p align="center"><img src="./static/logo.png" height=120 /></p>

**VSCode Animasyonları**, Visual Studio Code editörüne temiz ve özelleştirilebilir animasyonlar ekleyen bir eklentidir.

<img src="./static/gifs/Demo.gif" />

## Kurulum Adımları

### 1. Ana Eklentiyi Kurun

Şu yöntemlerden birini kullanın:

- [VSCode Marketplace](https://marketplace.visualstudio.com/items?itemName=BrandonKirbyson.vscode-animations)'den indirin
- VSCode içinde Extensions sekmesine gidin ve `VSCode Animations` arayın

### 2. Enjeksiyon Eklentisini Kurun

Animasyonların çalışması için bir enjeksiyon eklentisi gereklidir. **Önerilen** seçenekler:

#### A) Custom CSS and JS Loader (Önerilen)
1. [Custom CSS and JS Loader](https://marketplace.visualstudio.com/items?itemName=be5invis.vscode-custom-css) eklentisini kurun
2. VSCode yeniden başlayacaktır

#### B) Custom UI Style (Alternatif)
1. [Custom UI Style](https://marketplace.visualstudio.com/items?itemName=subframe7536.custom-ui-style) eklentisini kurun
2. VSCode yeniden başlayacaktır

### 3. Animasyonları Aktifleştirin

1. Enjeksiyon eklentisi kurulduktan sonra, VSCode Animations otomatik olarak kurulum önerisinde bulunacaktır:

   <img src="static/images/installPrompt.png" height=100/>

2. Kurulum onayını kabul edin:

   <img src="static/images/install.png" height=100/>

3. VSCode son kez yeniden başlayacaktır

### 4. Tamamlandı!

Animasyonlar artık aktif! VSCode'unuzda yumuşak geçişler ve animasyonlar göreceksiniz.

## Hızlı Ayarlar

- **Ayarlara erişim:** `Ctrl+,` → "animations" ara
- **Komutlar:** `Ctrl+Shift+P` → "Animations" ara

### Temel Komutlar

| Komut | Açıklama |
|-------|----------|
| `Animations: Enable Animations` | Animasyonları aç |
| `Animations: Disable Animations` | Animasyonları kapat |
| `Animations: Install Animations` | Animasyonları yeniden kur |
| `Animations: Open Animation Settings` | Ayarları aç |

## Sorun Giderme

### "VSCode installation is corrupt" Uyarısı
Bu normal bir uyarıdır:
1. Uyarıdaki ayarlar simgesine tıklayın
2. "Don't show again" seçeneğini işaretleyin

### Animasyonlar Çalışmıyor
1. `Ctrl+Shift+P` → `Animations: Install Animations` komutunu çalıştırın
2. VSCode'u yeniden başlatın
3. Hem VSCode Animations hem de enjeksiyon eklentisinin kurulu olduğundan emin olun

### Windows Sorunları
Eğer Windows kullanıyorsanız ve sorun yaşıyorsanız:
1. Ayarlarda `Animations: Install Method` seçeneğini kontrol edin
2. Farklı bir enjeksiyon eklentisi deneyebilirsiniz

## Desteklenen Enjeksiyon Eklentileri

1. **Custom CSS and JS Loader** ✅ (Önerilen)
2. **Custom UI Style** ✅ (Yeni özellikler)
3. **Apc Customize UI++** ❌ (Şu anda sorunlu)

---

### Animasyonların keyfini çıkarın! 🎉

*Daha fazla bilgi için orijinal [İngilizce README](README.md) dosyasına bakabilirsiniz.*