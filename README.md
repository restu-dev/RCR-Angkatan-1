# 🚀 Materi Dasar GitHub & Kolaborasi

## 📌 Git & GitHub
- **Git**: sistem kontrol versi untuk melacak perubahan kode.  
- **GitHub**: hosting repositori Git berbasis cloud untuk kolaborasi.

---

## 🔑 Perintah Dasar
```bash
git init                # buat repo baru
git add .               # tambahkan semua file
git commit -m "pesan"   # simpan perubahan
git remote add origin https://github.com/username/repo.git
git push origin main    # kirim ke GitHub
git pull origin main    # ambil update
```


## 👥 Studi Kasus Kolaborasi
repo-kolaborasi/
├── peserta1/ (index.html, style.css, script.js)
├── peserta2/ (index.html, style.css, script.js)
└── README.md


## 📝 Alur Kerja
1. **Clone repo**
```bash
git clone https://github.com/username/repo-kolaborasi.git
```

2. **Buat folder peserta (peserta1/) isi file HTML, CSS, JS.**

3. **Tambahkan & commit**
```bash
git add .
git commit -m "menambahkan folder peserta1"
git push origin main
```

4. **Sinkronisasi sebelum push ulang**
```bash
git pull origin main
```

## 📊 Workflow Diagram
           ┌───────────────┐
           │   GitHub Repo │
           └───────┬───────┘
                   │ clone
                   ▼
            ┌─────────────┐
            │  Lokal Repo │
            └──────┬──────┘
                   │ edit file
                   ▼
            ┌─────────────┐
            │ git add .   │
            └──────┬──────┘
                   │
                   ▼
            ┌─────────────┐
            │ git commit  │
            └──────┬──────┘
                   │ push
                   ▼
           ┌───────────────┐
           │   GitHub Repo │
           └──────┬───────┘
                   │ pull (sinkronisasi)
                   ▼
            ┌─────────────┐
            │  Lokal Repo │
            └─────────────┘


## 💻 Contoh File Peserta
1. **index.html**
```html
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Profil Peserta 1</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>Halo, saya Peserta 1</h1>
  <p>Ini adalah halaman profil sederhana menggunakan HTML, CSS, dan JavaScript.</p>
  <button onclick="showMessage()">Klik Saya</button>
  <script src="script.js"></script>
</body>
</html>
```

2. **style.html**
```css
body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f9;
  color: #333;
  text-align: center;
  padding: 50px;
}

button {
  padding: 10px 20px;
  font-size: 16px;
  background: #007bff;
  color: white;
  border: none;
  border-radius: 8px;
  cursor: pointer;
}

button:hover {
  background: #0056b3;
}
```

2. **script.html**
```js
function showMessage() {
  alert("Halo, ini interaksi dari Peserta 1!");
}
```




