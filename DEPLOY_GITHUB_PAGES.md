# 🚀 Deploy Error Page ke GitHub Pages

## ✅ File Sudah Siap!

Branch `gh-pages` sudah dibuat dengan files:
- ✅ `isolir-error-page.html` - Error page utama
- ✅ `index.html` - Landing page
- ✅ `README.md` - Documentation

## 📝 Step-by-Step Deploy

### **Step 1: Create GitHub Repository**

1. Buka https://github.com/new
2. **Repository name:** `wifi-net-isolir` (atau nama lain terserah)
3. **Visibility:** Public ✅
4. **JANGAN centang** "Add README" (udah ada)
5. Klik **Create repository**

### **Step 2: Push ke GitHub**

Copy command dari GitHub (setelah create repo), atau jalanin manual:

```bash
# Set remote (ganti USERNAME dan REPO-NAME!)
git remote add origin https://github.com/USERNAME/wifi-net-isolir.git

# Push branch gh-pages
git push -u origin gh-pages
```

**Example:**
```bash
git remote add origin https://github.com/johndoe/wifi-net-isolir.git
git push -u origin gh-pages
```

### **Step 3: Enable GitHub Pages**

1. Buka repo di GitHub
2. **Settings** → **Pages** (di sidebar kiri)
3. **Source:** Deploy from a branch
4. **Branch:** `gh-pages` → **/ (root)**
5. Klik **Save**
6. Tunggu ~1-2 menit

### **Step 4: Get Your URL**

GitHub Pages akan kasih URL:
```
https://USERNAME.github.io/REPO-NAME/isolir-error-page.html
```

**Example:**
```
https://johndoe.github.io/wifi-net-isolir/isolir-error-page.html
```

### **Step 5: Update Backend Config**

Edit `backend/.env`:

```env
# Ganti dengan URL GitHub Pages lu!
ISOLIR_ERROR_PAGE_URL=https://USERNAME.github.io/REPO-NAME/isolir-error-page.html
```

**Example:**
```env
ISOLIR_ERROR_PAGE_URL=https://johndoe.github.io/wifi-net-isolir/isolir-error-page.html
```

### **Step 6: Restart Backend**

```powershell
# Stop backend (Ctrl+C)
cd E:\Project\RT-RW-NET\cadangan\wifi_net\backend
npm run dev
```

### **Step 7: Setup Isolir Ulang**

1. Buka dashboard
2. **Mikrotik Control Panel**
3. Tab **Isolir**
4. Klik **"Setup Isolir Rule"**
5. ✅ Success message muncul!

### **Step 8: Test!**

1. Isolir IP test
2. Buka browser dari device tersebut
3. Akses google.com
4. **BOOM! Error page muncul!** 🎉

---

## 🔧 Update Error Page Nanti

Kalau mau update tampilan error page:

```bash
# 1. Edit file
notepad isolir-error-page.html

# 2. Commit & push
git add isolir-error-page.html
git commit -m "Update error page"
git push origin gh-pages

# 3. Tunggu ~1 menit, GitHub Pages auto-update!
```

---

## 🐛 Troubleshooting

### **GitHub Pages belum muncul?**

Tunggu 1-2 menit, refresh page Settings → Pages untuk cek status.

### **404 Not Found?**

Pastikan:
- ✅ Branch `gh-pages` sudah di-push
- ✅ Source di Settings → Pages: `gh-pages` + `/ (root)`
- ✅ URL benar (check case-sensitive!)

### **Error page gak update?**

- Clear browser cache
- Tunggu 1-2 menit (GitHub Pages cache)
- Cek commit sudah di-push: `git log`

---

## 📚 Useful Commands

```bash
# Cek branch saat ini
git branch

# Switch ke gh-pages
git checkout gh-pages

# Liat remote
git remote -v

# Push update
git push origin gh-pages

# Liat commit history
git log --oneline
```

---

## 🎯 Benefits GitHub Pages

✅ **HTTPS** built-in (secure!)
✅ **CDN** global (fast dari mana aja!)
✅ **Free** unlimited bandwidth
✅ **Auto-deploy** on push
✅ **No maintenance** required
✅ **Custom domain** support (optional)

---

## 🚀 Next Steps

Setelah deploy:
1. ✅ Test dari multiple devices
2. ✅ Customize error page (logo, kontak, dll)
3. ✅ Share URL ke team
4. ✅ Use for production!

---

**Happy deploying! 🎊**

