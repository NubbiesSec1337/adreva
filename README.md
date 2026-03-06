# 🚀 Adreva Farmer Bot v4.0

Auto farming points untuk Adreva — mendukung multi-akun, auto captcha solver, proxy support, dan sistem lisensi.

## ✨ Features

- 🔄 **Multi-Account** — Jalankan banyak akun sekaligus
- 🧩 **Auto Captcha Solver** — Math, emoji, dan counting captcha
- 🌐 **Proxy Support** — Rotasi proxy per akun
- 🔐 **License System** — Aktivasi dengan license key
- ⚡ **Auto Loop** — Otomatis farming ulang setiap cycle
- 📊 **Point Tracking** — Realtime session & total points

## 📋 Requirements

- **Node.js** v18+ 
- **npm**

## ⚙️ Setup

### 1. Install Dependencies

```bash
npm install
```

### 2. Aktivasi License

Masukkan salah satu license key saat pertama kali menjalankan bot:

| License Key | Durasi |
|---|---|
| `ADR-5F86-8F80-ADDA` | 10 hari |
| `ADR-9797-C2D4-9AE5` | 10 hari |
| `ADR-ED46-E8D3-F4C9` | 10 hari |
| `ADR-9C7A-4D08-5A7E` | 10 hari |
| `ADR-C2BB-4BDE-AAE0` | 10 hari |

> ⚠️ **1 license key = 1 device/IP.** Jangan share key-mu ke orang lain.

### 3. Jalankan Bot

```bash
node adreva.js
```

### 4. Tambah Akun

Pilih menu `1` → paste **refresh token** dari akun Adreva-mu.

Cara ambil refresh token:
1. Login di extension 
2. Buka DevTools → Application → Local Storage / copy di console chrome.storage.local.get('refreshToken', r => console.log(r.refreshToken)) 
3. Copy value dari `refreshToken`

### 5. Proxy (Opsional)

Buat file `proxy.txt` dan isi dengan format:

```
http://user:pass@ip:port
http://user:pass@ip:port
```

## 🎮 Penggunaan

```
  adreva farmer v4.0 (public)
  ──────────────────────────────

  1  add account
  2  run bot
  3  remove account
  4  change license key
  5  exit
```

- **Add account** — Tambah akun baru dengan refresh token
- **Run bot** — Mulai farming (auto loop)
- **Remove account** — Hapus akun yang tersimpan
- **Change license key** — Ganti license key

## 📁 File Structure

```
├── public_protected.js    ← Bot utama (jalankan ini)
├── package.json           ← Dependencies
├── proxy.txt              ← Daftar proxy (opsional)
├── akun.json              ← Akun tersimpan (auto-generated)
└── license.key            ← License key tersimpan (auto-generated)
```

## ❓ FAQ

**Q: Bot error "license not valid"?**  
A: License key mungkin sudah expired atau sudah dipakai di device lain. Hubungi admin untuk key baru.

**Q: Bot error "cannot reach license server"?**  
A: Cek koneksi internet. Jika tetap error, server lisensi mungkin sedang maintenance.

**Q: Berapa lama bot farming?**  
A: Bot akan farming semua campaign yang tersedia, lalu sleep ~24 jam sampai campaign berikutnya.



---

