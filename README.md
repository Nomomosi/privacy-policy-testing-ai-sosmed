# TESTING AI SOSMED — Pusat Privasi

Website statis berbahasa Indonesia untuk memublikasikan Kebijakan Privasi dan instruksi penghapusan data aplikasi TESTING AI SOSMED. Proyek ini tidak memerlukan backend atau framework dan dapat di-host di GitHub Pages.

## Struktur dan fungsi file

- `index.html` — halaman depan dan navigasi informasi privasi.
- `privacy-policy.html` — kebijakan privasi lengkap, termasuk alur data Meta, Anthropic Claude API, dan penyimpanan di Odoo.
- `data-deletion.html` — instruksi mengajukan permintaan penghapusan data.
- `assets/css/style.css` — gaya responsif untuk seluruh halaman.
- `assets/images/app-icon.svg` — ikon identitas situs dalam format SVG.
- `README.md` — panduan proyek dan publikasi.

## Informasi pengelola yang diisi

Informasi kontak berikut sudah dicantumkan pada halaman kebijakan dan instruksi penghapusan:

- `PT Perut Kembung` — nama pengelola yang diberikan.
- `perutkembung@gmail.com` — email kontak yang diberikan.

Pastikan nama dan alamat email tersebut benar serta emailnya dipantau untuk pertanyaan privasi dan permintaan penghapusan.

Kebijakan saat ini tidak menetapkan periode retensi khusus karena informasinya belum diberikan. Tetapkan kebijakan retensi operasional yang sebenarnya bila sudah diketahui, lalu sesuaikan teks di `privacy-policy.html`. Tanggal pembaruan awal adalah 9 November 2026; perbarui jika konten diubah setelah tanggal tersebut.

## Membuka dan menguji secara lokal

Cara termudah adalah membuka `index.html` langsung di browser. Semua halaman dan aset menggunakan path relatif sehingga juga dapat dibuka sebagai file lokal dan berfungsi dalam subpath GitHub Pages.

Untuk mencoba melalui server statis lokal (opsional), buka terminal di folder proyek dan jalankan salah satu:

```powershell
python -m http.server 8000
```

Lalu buka `http://localhost:8000` di browser. Server lokal hanya untuk pratinjau; situs yang dipublikasikan tidak memerlukan backend.

## Membuat repository dan mengunggah melalui GitHub

1. Pastikan informasi pengelola dan email kontak benar. Tinjau juga deskripsi alur data dan periode retensi agar sesuai dengan konfigurasi aplikasi yang benar-benar digunakan.
2. Masuk ke GitHub dan buat repository baru, misalnya `privacy-policy-testing-ai-sosmed`. Jangan menambahkan README otomatis jika ingin mengunggah folder ini apa adanya (atau gabungkan file dengan hati-hati bila README sudah dibuat GitHub).
3. Unggah isi folder proyek ini ke repository. Anda dapat memakai fitur **Add file → Upload files** di situs GitHub atau GitHub Desktop. Pastikan `index.html` berada di root repository, bukan di dalam folder bertingkat tambahan.
4. Buka **Settings → Pages** pada repository. Di bagian **Build and deployment**, pilih **Deploy from a branch**, pilih branch utama (umumnya `main`) dan folder `/(root)`, lalu simpan.
5. Tunggu GitHub Pages menyelesaikan deployment. URL umumnya berbentuk `https://NAMA-AKUN.github.io/NAMA-REPOSITORY/`. Gunakan URL tepat yang ditampilkan pada Settings → Pages.

## URL untuk Meta Developer

Ganti `NAMA-AKUN` dan `NAMA-REPOSITORY` di contoh berikut dengan nilai repository yang sebenarnya, lalu gunakan URL publik final dari GitHub Pages:

- **Meta Privacy Policy URL:** `https://NAMA-AKUN.github.io/NAMA-REPOSITORY/privacy-policy.html`
- **Meta User Data Deletion Instructions URL:** `https://NAMA-AKUN.github.io/NAMA-REPOSITORY/data-deletion.html`

Untuk halaman depan, alamatnya adalah `https://NAMA-AKUN.github.io/NAMA-REPOSITORY/`. Jangan masukkan URL localhost ke Meta Developer.

## Memperbarui setelah publikasi

Edit file yang sesuai (`privacy-policy.html`, `data-deletion.html`, atau `assets/css/style.css`), simpan perubahan, lalu unggah/perbarui file tersebut pada repository GitHub. GitHub Pages akan menerbitkan ulang situs setelah perubahan diterapkan. Jika isi kebijakan berubah, perbarui tanggal pembaruan pada halaman kebijakan dan tinjau ulang setiap URL di pengaturan Meta Developer.
