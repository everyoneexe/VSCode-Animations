# VSCode Animasyonları - Kurulum Rehberi

<p align="center"><img src="./static/logo.png" height=120 /></p>

**VSCode Animasyonları**, Visual Studio Code editörüne temiz ve özelleştirilebilir animasyonlar ekleyen bir eklentidir.

<img src="./static/gifs/Demo.gif" />

## Kurulum Yöntemleri

### Yöntem 1: Hazır VSIX Dosyası (Önerilen)

1. **VSIX dosyasını indirin:**
   - Bu repodan `vscode-animations-x.x.x.vsix` dosyasını indirin

2. **VSCode'a kurun:**
   ```bash
   code --install-extension vscode-animations-x.x.x.vsix
   ```
   
   Veya VSCode içinden:
   - `Ctrl+Shift+P` → `Extensions: Install from VSIX...`
   - İndirdiğiniz `.vsix` dosyasını seçin

### Yöntem 2: Kaynak Koddan Derleme

1. **Repoyu klonlayın:**
   ```bash
   git clone https://github.com/everyoneexe/VSCode-Animations.git
   cd VSCode-Animations
   ```

2. **Bağımlılıkları kurun:**
   ```bash
   npm install
   ```

3. **Eklentiyi derleyin:**
   ```bash
   npm run package
   ```

4. **Oluşan VSIX'i kurun:**
   ```bash
   code --install-extension vscode-animations-x.x.x.vsix
   ```

## Enjeksiyon Eklentisini Kurun

Animasyonların çalışması için bir enjeksiyon eklentisi gereklidir:

### Seçenek A: Custom CSS and JS Loader (Önerilen)
```bash
code --install-extension be5invis.vscode-custom-css
```

### Seçenek B: Custom UI Style (Alternatif)
```bash
code --install-extension subframe7536.custom-ui-style
```

## Aktivasyon

1. **VSCode'u yeniden başlatın**

2. **Kurulum önerisini kabul edin:**

   <img src="static/images/installPrompt.png" height=100/>

3. **Animasyonları kurun:**

   <img src="static/images/install.png" height=100/>

4. **VSCode son kez yeniden başlayacaktır**

## Manuel Kurulum (İleri Seviye)

Eğer otomatik kurulum çalışmazsa:

1. **Script yolunu alın:**
   - `Ctrl+Shift+P` → `Animations: Get Script Path`

2. **Enjeksiyon eklentinizin ayarlarına ekleyin:**
   - Custom CSS and JS Loader: `vscode_custom_css.imports` ayarına ekleyin
   - Custom UI Style: İlgili ayarlara script yolunu ekleyin

## Hızlı Komutlar

| Komut | Açıklama |
|-------|----------|
| `Animations: Install Animations` | Animasyonları kur/yeniden kur |
| `Animations: Enable Animations` | Animasyonları aç |
| `Animations: Disable Animations` | Animasyonları kapat |
| `Animations: Open Animation Settings` | Ayarları aç |

## Sorun Giderme

### "VSCode installation is corrupt" Uyarısı
Bu normal bir uyarıdır:
1. Uyarıdaki ayarlar simgesine tıklayın
2. "Don't show again" seçeneğini işaretleyin

### Animasyonlar Görünmüyor
1. Enjeksiyon eklentisinin kurulu olduğundan emin olun
2. `Ctrl+Shift+P` → `Animations: Install Animations`
3. VSCode'u tamamen kapatıp yeniden açın

### Derleme Sorunları
```bash
# Node modüllerini temizleyin
rm -rf node_modules package-lock.json
npm install

# TypeScript sorunları için
npm run compile

# Temiz derleme
npm run clean
npm run package
```

## Geliştirme

### Gereksinimler
- Node.js 16.x+
- VSCode 1.64.0+
- TypeScript 4.x+

### Geliştirme Komutları
```bash
# Geliştirme modunda çalıştır
npm run watch

# Test et
npm run test

# Lint kontrolü
npm run lint

# Üretim paketi oluştur
npm run package
```

---

### Animasyonların keyfini çıkarın! 🎉

*Orijinal proje: [VSCode Animations](https://github.com/BrandonKirbyson/VSCode-Animations)*
