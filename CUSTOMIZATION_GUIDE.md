# 💻 Panduan Personalisasi Portfolio Website

## 📝 Daftar Kustomisasi yang Harus Dilakukan

### 1. ✅ Update Profile Information

#### A. Nama dan Tagline
**File**: `portofolio.html` - Baris ~455

```html
<!-- Sebelum -->
<h1 data-aos="fade-up" data-aos-delay="100" data-aos-duration="800">
    Aldo Fernando
</h1>

<!-- Sesudah - Ganti dengan nama Anda -->
<h1 data-aos="fade-up" data-aos-delay="100" data-aos-duration="800">
    [NAMA ANDA]
</h1>
```

#### B. Tagline/Profesi
```html
<!-- Sebelum -->
<h2 data-aos="fade-up" data-aos-delay="200" data-aos-duration="800">
    Software Developer & IT Student
</h2>

<!-- Sesudah -->
<h2 data-aos="fade-up" data-aos-delay="200" data-aos-duration="800">
    [PROFESI ANDA] & [PENDIDIKAN]
</h2>
```

#### C. Deskripsi Singkat
```html
<!-- Sebelum -->
<p class="hero-subtitle" data-aos="fade-up" data-aos-delay="300" data-aos-duration="800">
    Saya adalah developer yang passionate tentang membuat solusi inovatif dengan teknologi terkini. 
    Spesialisasi saya adalah PHP, Java, C#, dan pengembangan aplikasi web yang responsif dan user-friendly.
</p>

<!-- Sesudah - Personalisasi deskripsi -->
<p class="hero-subtitle" data-aos="fade-up" data-aos-delay="300" data-aos-duration="800">
    [DESKRIPSI SINGKAT ANDA - 2-3 kalimat tentang passion dan keahlian Anda]
</p>
```

---

### 2. ✅ Update Foto Profile

#### A. Ganti Foto
Letakkan foto Anda di folder `assets/` dengan nama yang descriptive.

```html
<!-- Sebelum -->
<img src="assets/PasFotoAldo.jpg" alt="Aldo Fernando - Software Developer" 
     loading="lazy" onerror="this.src='https://via.placeholder.com/350x350?text=Profile'">

<!-- Sesudah -->
<img src="assets/foto-profile-anda.jpg" alt="[NAMA ANDA] - [PROFESI]" 
     loading="lazy" onerror="this.src='https://via.placeholder.com/350x350?text=Profile'">
```

**Tips**: 
- Gunakan foto berkualitas tinggi (minimal 350x350px)
- Format: JPG atau PNG
- Ukuran file: < 500KB untuk performa optimal

---

### 3. ✅ Update About Section

```html
<!-- Sebelum -->
<h3>Seorang Developer Bersemangat 🚀</h3>
<p>
    Saya adalah mahasiswa IT yang berdedikasi untuk menjadi software developer profesional. 
    Dengan pengalaman mengerjakan berbagai proyek dari skala kecil hingga sistem enterprise, 
    saya telah mengembangkan keahlian dalam multiple technology stack.
</p>

<!-- Sesudah -->
<h3>[SUBTITLE ABOUT ANDA] 🚀</h3>
<p>
    [PARAGRAPH 1 - TENTANG BACKGROUND DAN PENGALAMAN ANDA]
</p>
```

#### Update Skills Tags:
```html
<!-- Sebelum -->
<span class="skills-tag"><i class="fas fa-check-circle"></i> PHP & Framework</span>
<span class="skills-tag"><i class="fas fa-check-circle"></i> Java & Spring Boot</span>

<!-- Sesudah - Sesuaikan dengan keahlian Anda -->
<span class="skills-tag"><i class="fas fa-check-circle"></i> [SKILL 1]</span>
<span class="skills-tag"><i class="fas fa-check-circle"></i> [SKILL 2]</span>
```

---

### 4. ✅ Update Skills Section

Sesuaikan 6 skill cards dengan keahlian Anda. Untuk setiap card:

```html
<div class="skill-card" data-aos="zoom-in" data-aos-delay="100">
    <div class="skill-icon">
        <i class="fas fa-server"></i>  <!-- Ganti icon -->
    </div>
    <h3>Backend Development</h3>  <!-- Ganti judul -->
    <p>Spesialisasi dalam PHP, Java, C#...</p>  <!-- Ganti deskripsi -->
    
    <!-- Update progress bars -->
    <div class="progress-bar-container">
        <div class="progress-label">
            <span>PHP</span>
            <span>90%</span>  <!-- Update percentage -->
        </div>
        <div class="progress">
            <div class="progress-bar" data-value="90"></div>
        </div>
    </div>
</div>
```

#### Font Awesome Icons:
Lihat [Font Awesome Icons](https://fontawesome.com/icons) untuk pilihan icon:
- `fa-server` - Backend
- `fa-palette` - Frontend/Design
- `fa-database` - Database
- `fa-mobile-alt` - Mobile
- `fa-tools` - Tools
- `fa-sitemap` - Architecture
- `fa-code` - Programming
- `fa-brain` - AI/ML
- `fa-cloud` - Cloud
- `fa-lock` - Security

---

### 5. ✅ Update Projects Section

Ini adalah bagian paling penting. Update dalam JavaScript section:

```javascript
// Cari bagian "PROJECTS DATA & RENDERING"
const projects = [
    {
        title: "Nama Project 1",
        description: "Deskripsi singkat tentang project ini",
        tech: ["Technology 1", "Technology 2", "Technology 3"],
        link: "https://github.com/username/project-repo",
        icon: "fa-network-wired"
    },
    {
        title: "Nama Project 2",
        description: "Deskripsi singkat tentang project ini",
        tech: ["Tech A", "Tech B"],
        link: "https://github.com/username/project-repo-2",
        icon: "fa-mobile-alt"
    },
    // Tambahkan lebih banyak projects...
];
```

**Contoh Lengkap untuk 3 Projects:**

```javascript
const projects = [
    {
        title: "E-Commerce Platform",
        description: "Platform e-commerce lengkap dengan payment gateway dan inventory management.",
        tech: ["Laravel", "Vue.js", "MySQL", "Stripe"],
        link: "https://github.com/yourname/ecommerce-platform",
        icon: "fa-shopping-cart"
    },
    {
        title: "Mobile App - Todo Manager",
        description: "Aplikasi mobile untuk manajemen todo dengan sync cloud real-time.",
        tech: ["React Native", "Firebase", "Node.js"],
        link: "https://github.com/yourname/todo-mobile-app",
        icon: "fa-mobile-alt"
    },
    {
        title: "AI Chatbot Integration",
        description: "Chatbot AI yang terintegrasi dengan website untuk customer service otomatis.",
        tech: ["Python", "TensorFlow", "Flask", "React"],
        link: "https://github.com/yourname/ai-chatbot",
        icon: "fa-robot"
    },
];
```

**Icon Options untuk Projects:**
- `fa-code` - Coding
- `fa-shopping-cart` - E-commerce
- `fa-mobile-alt` - Mobile App
- `fa-robot` - AI/Bot
- `fa-chart-line` - Dashboard/Analytics
- `fa-database` - Database
- `fa-network-wired` - Network/API
- `fa-check-circle` - Verification
- `fa-car` - Automotive
- `fa-hospital` - Medical

---

### 6. ✅ Update Contact Information

Update dengan kontak Anda yang sebenarnya:

```html
<!-- Email -->
<a href="mailto:your-email@example.com">your-email@example.com</a>

<!-- GitHub -->
<a href="https://github.com/your-username" target="_blank">github.com/your-username</a>

<!-- LinkedIn -->
<a href="https://www.linkedin.com/in/your-profile" target="_blank">Your Name</a>
```

---

### 7. ✅ Setup EmailJS untuk Contact Form

**Langkah 1**: Daftar di [EmailJS](https://www.emailjs.com/)

**Langkah 2**: Buat Email Service
- Login ke EmailJS Dashboard
- Go to "Email Services"
- Klik "Add New Service"
- Pilih email provider (Gmail, Outlook, dll)
- Follow instruksi setup

**Langkah 3**: Buat Email Template
- Go to "Email Templates"
- Klik "Create New Template"
- Gunakan template ini:

```
Subject: New Portfolio Message from {{from_name}}

From: {{from_email}}
Name: {{from_name}}

Message:
{{message}}
```

**Langkah 4**: Update di JavaScript

```javascript
// Cari baris ini di JavaScript (sekitar baris 1580)
emailjs.init("_Y_nmyD8rQIubZKjA");  // GANTI dengan Public Key Anda

// Ganti di function setupContactForm (sekitar baris 1680)
await emailjs.send('service_wtt4e66', 'template_vv1u8nq', templateParams);
```

**Dimana cari credentials?**
- Public Key: EmailJS Dashboard > Account > API Keys > Public Key
- Service ID: Email Services > Klik service > Service ID
- Template ID: Email Templates > Klik template > Template ID

---

### 8. ✅ Update Social Links

Update footer dengan social media Anda:

```html
<!-- Footer Social Links -->
<a href="https://github.com/your-username" target="_blank" class="social-link">
    <i class="fab fa-github"></i>
</a>
<a href="https://www.linkedin.com/in/your-profile" target="_blank" class="social-link">
    <i class="fab fa-linkedin"></i>
</a>
<a href="mailto:your-email@example.com" class="social-link">
    <i class="fas fa-envelope"></i>
</a>
```

**Tambahan Social Media (Opsional):**

```html
<!-- Twitter -->
<a href="https://twitter.com/your-username" target="_blank" class="social-link">
    <i class="fab fa-twitter"></i>
</a>

<!-- Instagram -->
<a href="https://instagram.com/your-username" target="_blank" class="social-link">
    <i class="fab fa-instagram"></i>
</a>

<!-- Portfolio/Website -->
<a href="https://your-website.com" target="_blank" class="social-link">
    <i class="fas fa-globe"></i>
</a>
```

---

### 9. ✅ Update Navbar Brand

```html
<!-- Sebelum -->
<a class="navbar-brand" href="#hero">
    <i class="fas fa-terminal"></i> AF.DEV
</a>

<!-- Sesudah - Ganti dengan inisial atau nama Anda -->
<a class="navbar-brand" href="#hero">
    <i class="fas fa-terminal"></i> [INISIAL ANDA]
</a>

<!-- Atau gunakan icon berbeda -->
<a class="navbar-brand" href="#hero">
    <i class="fas fa-code"></i> [NAMA ANDA]
</a>
```

---

### 10. ✅ Update Meta Tags dan Title

```html
<!-- Sebelum -->
<meta name="description" content="Portfolio profesional Aldo Fernando - Software Developer...">
<title>Aldo Fernando | Software Developer Portfolio</title>

<!-- Sesudah -->
<meta name="description" content="Portfolio profesional [NAMA ANDA] - [PROFESI]...">
<title>[NAMA ANDA] | [PROFESI] Portfolio</title>
```

---

## 🎨 Customization Tambahan (Opsional)

### Mengubah Color Scheme

Di bagian CSS (baris ~25-33):

```css
:root {
    --primary-dark: #0a0e27;       /* Warna gelap utama */
    --secondary-dark: #1a1f3a;     /* Warna gelap sekunder */
    --accent-cyan: #00d4ff;        /* Aksen cyan - UBAH INI */
    --accent-purple: #b700ff;      /* Aksen purple - UBAH INI */
    --accent-pink: #ff0080;        /* Aksen pink - UBAH INI */
    --accent-blue: #39b8ff;        /* Aksen biru - UBAH INI */
    --text-light: #e0e0e0;         /* Warna teks */
    --text-muted: #a0a0a0;         /* Warna teks muted */
}
```

**Contoh Color Palettes:**

**Blue & Orange (Modern)**:
```css
--accent-cyan: #0080ff;       /* Blue */
--accent-purple: #ff6b35;     /* Orange */
--accent-pink: #ff8c42;       /* Light Orange */
--accent-blue: #004e89;       /* Dark Blue */
```

**Green & Purple (Tech)**:
```css
--accent-cyan: #00d98e;       /* Green */
--accent-purple: #8b5cf6;     /* Purple */
--accent-pink: #ec4899;       /* Pink */
--accent-blue: #06b6d4;       /* Cyan */
```

---

## 📋 Checklist Final Sebelum Launch

- [ ] Update nama dan profesi
- [ ] Ganti foto profile
- [ ] Update about section
- [ ] Tambahkan 3-6 projects
- [ ] Setup EmailJS contact form
- [ ] Update social media links
- [ ] Update contact information
- [ ] Test responsive di mobile
- [ ] Test form submission
- [ ] Check semua links work
- [ ] Optimize images
- [ ] Test di browser berbeda
- [ ] Deploy ke hosting

---

## 🚀 Cara Test Sebelum Live

1. **Local Testing**:
   ```bash
   # Buka file dengan live server extension di VS Code
   # Atau buka langsung di browser
   ```

2. **Test Responsive**:
   - Press F12 → DevTools
   - Click responsive icon (Ctrl+Shift+M)
   - Test di berbagai ukuran

3. **Test Form**:
   - Isi form contact
   - Verify email sampai ke inbox

4. **Test Links**:
   - Klik semua navigation links
   - Klik semua social media links
   - Klik project links

---

## 📱 Testing Devices

Minimal test di:
- Chrome Desktop
- Firefox Desktop
- Safari (jika punya Mac)
- Mobile Chrome
- Mobile Safari

---

Selesai! Sekarang portfolio Anda siap untuk dipersonalisasi. 🎉

**Happy Customizing! 💻✨**
