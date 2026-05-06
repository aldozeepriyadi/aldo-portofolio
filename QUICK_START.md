# ⚡ QUICK START - 10 Menit Setup

Ikuti panduan cepat ini untuk membuat portfolio Anda hidup dalam 10 menit!

---

## 📌 5 Langkah Cepat

### LANGKAH 1: Update Bio Anda (2 menit)

**Buka**: `portofolio.html`

**Cari dan ganti:**
```
Ctrl+H (Find & Replace)

Cari: "Aldo Fernando"
Ganti: "NAMA ANDA"

Cari: "Software Developer & IT Student"
Ganti: "PROFESI ANDA & PENDIDIKAN"
```

---

### LANGKAH 2: Update Foto (1 menit)

1. Letakkan foto (JPG/PNG) di folder `assets/`
2. Buka `portofolio.html`
3. Cari: `src="assets/PasFotoAldo.jpg"`
4. Ganti dengan: `src="assets/nama-foto-anda.jpg"`

---

### LANGKAH 3: Update Projects (3 menit)

**Cari di JavaScript (Ctrl+F)**: `const projects = [`

**Template:**
```javascript
{
    title: "Project Anda",
    description: "Deskripsi singkat",
    tech: ["Tech1", "Tech2"],
    link: "https://github.com/anda/project",
    icon: "fa-code"
}
```

Ganti 6 projects dengan punya Anda.

---

### LANGKAH 4: Setup Email (2 menit)

1. Daftar: https://www.emailjs.com/
2. Create Email Service (follow instruksi)
3. Create Template Email
4. Copy Public Key dari Account > API Keys
5. Ganti di JavaScript:
   ```javascript
   emailjs.init("YOUR_PUBLIC_KEY_HERE");
   ```
6. Ganti juga Service ID dan Template ID:
   ```javascript
   emailjs.send('SERVICE_ID', 'TEMPLATE_ID', templateParams)
   ```

---

### LANGKAH 5: Update Kontak (2 menit)

**Cari di HTML**:
```
aldo.fernandosupriyadi@gmail.com    →   Email Anda
aldozeepriyadi                      →   GitHub username
aldo-fernando-491634187            →   LinkedIn ID
```

---

## ✅ Test & Launch

```bash
# 1. Test Responsive
Press F12 → Toggle Device Toolbar (Ctrl+Shift+M)

# 2. Test Form
Isi form contact → Send → Check email

# 3. Deploy
Upload ke hosting atau GitHub Pages
```

---

## 🎨 Bonus - Ubah Warna

**Di CSS**, cari `:root {`:
```css
--accent-cyan: #00d4ff;     ← Ubah warna ini
--accent-purple: #b700ff;   ← Ubah warna ini
--accent-pink: #ff0080;     ← Ubah warna ini
```

**Color Ideas:**
- Blue: `#0080ff`
- Green: `#00d98e`
- Orange: `#ff6b35`
- Red: `#ff3b30`

---

## 📋 What's Included

✅ Hero Section dengan animations
✅ About section 
✅ 6 Skills cards dengan progress bars
✅ Projects showcase dari GitHub
✅ Contact form dengan EmailJS
✅ Footer dengan social links
✅ Fully responsive design
✅ Dark mode futuristic theme
✅ Scroll animations
✅ Particle background

---

## 🚀 Deploy Options

### Option 1: GitHub Pages (GRATIS)
```bash
1. Push ke GitHub
2. Settings > Pages > Deploy from branch (main)
3. Done! Akses: username.github.io/repo-name
```

### Option 2: Netlify (GRATIS)
```bash
1. Drag & drop folder ke netlify.com
2. Done! Instant deploy
```

### Option 3: Vercel (GRATIS)
```bash
1. Import repo dari GitHub
2. Deploy
3. Custom domain support
```

---

## 🎓 Struktur File

```
aldo-portofolio/
├── portofolio.html        ← File utama
├── assets/
│   ├── PasFotoAldo.jpg    ← Ganti dengan foto Anda
│   ├── CV_AldoFernandoS.pdf
│   └── PortofolioAldo.pdf
├── README.md              ← Dokumentasi lengkap
├── CUSTOMIZATION_GUIDE.md ← Guide detail
└── QUICK_START.md         ← File ini
```

---

## 🔍 Tips & Tricks

**Keyboard Shortcuts:**
- `Ctrl+Shift+F` - Search in all files
- `Ctrl+H` - Find & Replace
- `Alt+Up/Down` - Move line up/down
- `Ctrl+/` - Comment/uncomment

**VS Code Extensions untuk Lebih Cepat:**
- Live Server (Preview changes real-time)
- HTML Boilerplate
- CSS Peek

---

## ❓ Common Issues & Solutions

**Q: Email form tidak bekerja?**
A: Check console (F12) untuk error. Pastikan EmailJS key benar.

**Q: Animasi lambat?**
A: Reduce particles count di `initParticles()` function.

**Q: Tidak responsive di mobile?**
A: Open DevTools → Toggle responsive. Check media queries di CSS.

**Q: Foto tidak muncul?**
A: Periksa path di `src`. Pastikan file ada di `assets/`.

---

## 📞 Quick Reference

| Elemen | File | Lokasi |
|--------|------|--------|
| Nama | portofolio.html | Baris ~455 |
| Foto | portofolio.html | Baris ~526 |
| About | portofolio.html | Baris ~545 |
| Skills | portofolio.html | Baris ~575 |
| Projects | portofolio.html | Baris ~1580 (JS) |
| Contact | portofolio.html | Baris ~820 |
| Email Setup | portofolio.html | Baris ~1580 (JS) |
| Colors | portofolio.html | Baris ~25-33 (CSS) |

---

## 🎉 Done!

Sekarang portfolio Anda:
- ✅ Profesional & modern
- ✅ Fully responsive
- ✅ Interaktif dengan animations
- ✅ SEO optimized
- ✅ Fast loading
- ✅ Mobile friendly

**Next Step**: Mulai isi projects dan terus update!

---

**Butuh bantuan?**
Lihat `README.md` untuk dokumentasi lengkap
Lihat `CUSTOMIZATION_GUIDE.md` untuk detail lebih

**Happy coding! 🚀**
