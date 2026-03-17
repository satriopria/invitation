# 💍 Undangan Pernikahan Digital
### Satrio Priambodo & Sherly Regita Putri

> *"Dan di antara tanda-tanda kekuasaan-Nya ialah Dia menciptakan untukmu pasangan hidup dari jenismu sendiri, supaya kamu cenderung dan merasa tenteram kepadanya."*
> — QS. Ar-Rum: 21

---

## 📅 Ahad, 12 April 2026
**Resepsi Pernikahan (Walimatul 'Ursy)**
Jalan Gede III Kavling HVA No. 30, Pare, Kediri

| Sesi | Waktu |
|------|-------|
| Sesi I | 10.30 – 13.00 WIB |
| Sesi II | 13.30 – 15.30 WIB |
| Sesi III | 16.00 – 17.00 WIB |

---

## 🌐 Akses Undangan

**[satriopria.github.io/invitation](https://satriopria.github.io/invitation)**

Link personal per tamu:
```
https://satriopria.github.io/invitation/?t=<token>
```

---

## ⚙️ Stack

| Komponen | Teknologi |
|----------|-----------|
| Hosting | GitHub Pages (gratis) |
| Backend | Google Apps Script |
| Database | Google Sheets |
| Frontend | HTML · CSS · Vanilla JS |

---

## 🗂️ Struktur

```
/
├── index.html        ← Website undangan
└── LICENSE
└── README.md
```

Backend (Google Apps Script) di-host terpisah sebagai Web App — tidak ada di repo ini.

---

## ✨ Fitur

- **Link personal** per tamu dengan nama ter-encode di URL
- **RSVP** langsung dari halaman, tersimpan ke Google Sheets
- **Hitung mundur** menuju hari H
- **Sesi kehadiran** — tiap tamu bisa dialokasikan ke salah satu dari tiga sesi
- **Admin panel** tersembunyi — kelola tamu, generate link, export CSV
- **Password admin** dari Google Sheets — tidak hardcode di HTML
- Animasi parallax & ornamen SVG berputar
- Responsif untuk mobile

---

## 🔒 Keamanan

- Password admin di-hash SHA-256 di browser, dibandingkan dengan hash yang dihitung server dari Sheet
- Token URL menggunakan XOR + Base64 — mencegah edit manual
- Admin token wajib untuk semua operasi admin
- Rate limiting: 1 RSVP per 60 detik per browser

---

*Barakallahu laka wa baraka alaika wa jama'a bainakuma fi khair* 🤍
