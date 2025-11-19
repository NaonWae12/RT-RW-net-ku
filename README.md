# WiFi-Net Isolir Error Page

Halaman error custom untuk sistem isolir WiFi-Net.

## 🌐 Live Demo

**URL:** [https://NaonWae12.github.io/RT-RW-net-ku/isolir-error-page.html](https://NaonWae12.github.io/RT-RW-net-ku/isolir-error-page.html)



## 📋 Description

Error page yang ditampilkan kepada client yang terisolir (internet diblokir karena tagihan belum dibayar).

### Features:
- ⚠️ Tampilan modern & responsive
- 📱 Mobile-friendly
- 🎨 Gradient background yang menarik
- ℹ️ Informasi jelas tentang:
  - Akses internet terbatas
  - Alasan (tagihan belum dibayar)
  - Cara untuk mengaktifkan kembali
  - Kontak admin

## 🚀 Usage

Untuk menggunakan error page ini di sistem WiFi-Net:

1. **Set environment variable** di `backend/.env`:
   ```env
   ISOLIR_ERROR_PAGE_URL=https://USERNAME.github.io/REPO-NAME/isolir-error-page.html
   ```

2. **Restart backend**

3. **Setup isolir** via dashboard

4. **Done!** Client terisolir akan diarahkan ke halaman ini.

## 📝 Customization

Untuk customize error page:
1. Edit `isolir-error-page.html`
2. Commit & push ke GitHub
3. GitHub Pages akan auto-update (tunggu ~1 menit)
4. Client terisolir langsung dapat tampilan baru!

## 🔧 Development

File asli ada di: `backend/public/isolir-error-page.html`

## 📚 Documentation

- [Setup Guide](https://github.com/USERNAME/REPO-NAME)
- [WiFi-Net System Docs](https://github.com/USERNAME/wifi-net)

---

**Built with ❤️ for WiFi-Net RT-RW System**
