# Portfolio Aikoo — Dark Mode Developer Portfolio

Portfolio website modern dengan dark theme, animasi particles, dan admin panel built-in untuk edit konten tanpa coding.

## Fitur

- **Dark Mode Design** — tema gelap dengan gradient ungu-cyan
- **Particle Animation** — background interaktif dengan canvas
- **Smooth Scroll** — navigasi halus antar section
- **Admin Panel** — login dan edit konten langsung di browser
- **Responsive** — optimal di desktop, tablet, dan mobile
- **Zero Dependency** — single HTML file, tidak perlu install apapun

## Section

1. **Hero** — Nama, tagline, CTA buttons
2. **Tentang** — Bio, statistik (proyek, klien, pengalaman)
3. **Keahlian** — Grid skill dengan emoji
4. **Proyek** — Card proyek dengan tech tags
5. **Pengalaman** — Timeline karier
6. **Kontak** — Email, Telegram, GitHub, Website

## Cara Pakai

### 1. Buka Langsung
Buka `index.html` di browser. Selesai.

### 2. Edit Konten (Admin Panel)
1. Klik tombol **⚙ Admin** di pojok kanan atas
2. Login password: `aikoo2026`
3. Edit konten yang mau diubah
4. Klik **💾 Simpan Perubahan**
5. Refresh halaman untuk lihat hasil

### 3. Ganti Password
Edit di `index.html`, cari:
```javascript
if (pass === 'aikoo2026') {
```
Ganti `aikoo2026` dengan password baru.

## Deploy ke Domain Gratis (northwestregisteredagent.com)

### Opsi A: GitHub Pages (Gratis, Recommended)
1. Buat repo baru di GitHub: `aikoo.github.io` (ganti aikoo dengan username GitHub kamu)
2. Upload `index.html` ke repo tersebut
3. Aktifkan GitHub Pages: Settings → Pages → Source: main branch
4. Domain: `https://aikoo.github.io`

### Opsi B: Cloudflare Pages (Gratis)
1. Push `index.html` ke GitHub
2. Buka [Cloudflare Dashboard](https://dash.cloudflare.com) → Pages
3. Connect repository → Deploy
4. Custom domain: tambahkan domain dari northwestregisteredagent

### Opsi C: Netlify Drop (Paling Cepat)
1. Buka [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag & drop folder `portfolio-site`
3. Langsung dapat URL. Custom domain di settings.

## Custom Domain (northwestregisteredagent.com)

1. Deploy ke salah satu platform di atas
2. Di DNS settings northwestregisteredagent, tambahkan:
   - **CNAME** → `username.github.io` (atau URL platform)
   - atau **A record** → IP platform
3. Tunggu propagasi DNS (5-60 menit)

## Struktur File

```
portfolio-site/
├── index.html    # Portfolio lengkap (single file)
└── README.md     # Dokumentasi ini
```

## Teknologi

- HTML5 + CSS3 (Grid, Flexbox, Custom Properties)
- Vanilla JavaScript (Canvas API, IntersectionObserver, localStorage)
- Font: System UI (Segoe UI, -apple-system)

## Catatan Keamanan

- Konten disimpan di `localStorage` browser — hanya terlihat di device yang sama
- Password admin hardcoded di HTML — jangan share source code kalau ganti password
- Untuk produksi serius, pertimbangkan backend (Firebase, Supabase)

---

Dibuat dengan ❤️ dan kopi.
