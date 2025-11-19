# Manual Testing Project - Practice Software Testing

Proyek testing manual pada website e-commerce Practice Software Testing untuk menguji fungsionalitas, keamanan, dan pengalaman pengguna.

## Informasi Proyek

- **Website**: https://practicesoftwaretesting.com/
- **Tipe Testing**: Manual Testing (Black Box)
- **Total Test Cases**: 142
- **Periode**: November 2024
- **Tester**: Erlina Febiola Nainggolan

## Tujuan Testing

Melakukan pengujian menyeluruh pada website e-commerce untuk:
- Memastikan semua fitur berfungsi dengan baik
- Menemukan bug dan masalah pada sistem
- Mengidentifikasi kerentanan keamanan
- Mengevaluasi pengalaman pengguna

## Hasil Testing

| Status | Jumlah | Persentase |
|--------|--------|------------|
| PASS | 135 | 95% |
| FAILED | 4 | 3% |
| OPEN (Security Issues) | 3 | 2% |
| **TOTAL** | **142** | **100%** |

## Cakupan Testing

### 1. Customer Registration (11 test cases)
- Verifikasi tampilan halaman registrasi
- Validasi form input untuk email, password, dan data pribadi
- Indikator kekuatan password
- Penanganan error

### 2. Login (13 test cases)
- Login dengan kredensial yang benar dan salah
- Validasi format email dan password
- Fitur tampil/sembunyikan password
- Login menggunakan Google
- Link navigasi ke halaman registrasi dan lupa password

### 3. My Account Page (12 test cases)
- Tampilan halaman akun pengguna
- Menu Favorites, Profile, Invoices, dan Messages
- Desain responsive
- Link navigasi

### 4. Home - Product Catalog (11 test cases)
- Fitur pencarian produk
- Filter berdasarkan harga dan kategori
- Pengurutan produk berdasarkan nama, harga, dan rating CO2
- Status produk habis

### 5. Categories - Hand Tools (13 test cases)
- Filter berdasarkan merek
- Filter produk ramah lingkungan
- Pengurutan dan pagination

### 6. Categories - Power Tools (18 test cases)
- Filter sub-kategori dan merek
- Kombinasi beberapa filter sekaligus
- Handling ketika tidak ada produk

### 7. Categories - Special Tools (5 test cases)
- Tampilan kategori kosong
- Fungsi filter dan sort

### 8. Categories - Rentals (3 test cases)
- Tampilan produk rental
- Navigasi ke halaman detail

### 9. Product Detail Page - Rentals (10 test cases)
- Informasi produk rental
- Slider durasi dan kalkulasi harga
- Tambah ke keranjang dan favorit
- Produk terkait

### 10. Contact Form (11 test cases)
- Validasi form input
- Validasi upload file
- Pesan error

### 11. Security Testing (12 test cases)
- Testing SQL Injection
- Testing XSS (Cross-Site Scripting)
- Proteksi brute force
- Manajemen session
- Keamanan password

## Bug yang Ditemukan

### Masalah Kritis (Perlu Segera Diperbaiki)

**1. SEC-006: XSS Vulnerability pada Search Field**
- Severity: Critical
- Deskripsi: Script berbahaya dapat dijalankan di fitur search
- Dampak: Penyerang bisa mencuri data pengguna atau menyerang pengguna lain
- Status: OPEN

**2. SEC-007: Tidak Ada Brute Force Protection**
- Severity: Critical
- Deskripsi: Tidak ada batasan percobaan login yang gagal
- Dampak: Sistem rentan terhadap serangan brute force
- Status: OPEN

**3. SEC-004: Stored XSS pada Registration**
- Severity: High
- Deskripsi: Script XSS tersimpan di database tanpa sanitasi
- Dampak: Berpotensi dieksekusi ketika data ditampilkan
- Status: OPEN

### Bug Prioritas Tinggi

**4. CNT-002: Error Message yang Membingungkan**
- Severity: High
- Deskripsi: Muncul error "Currently we only allow empty files" padahal tidak ada file yang di-upload
- Dampak: Pengguna bingung dan tidak bisa mengirim pesan

**5. REG-006 & REG-007: Pesan Error Password Tidak Akurat**
- Severity: Medium-High
- Deskripsi: Pesan error menampilkan "cannot include invalid characters" padahal seharusnya "must include special character"
- Dampak: Pengguna tidak mengerti cara memperbaiki password

### Bug Prioritas Sedang

**6. LGN-010: Tombol Enter Tidak Berfungsi untuk Login**
- Severity: Medium
- Deskripsi: Tombol Enter di keyboard tidak memicu proses login
- Dampak: Pengalaman pengguna kurang baik

**7. REG-011: Tombol Register Tidak Disabled**
- Severity: Medium
- Deskripsi: Tombol Register dapat diklik sebelum form diisi lengkap
- Dampak: Muncul banyak pesan error sekaligus

## Dokumentasi

File dokumentasi test case tersedia dalam format CSV dengan struktur:
- **TC ID**: ID unik untuk setiap test case
- **Test Case Title**: Judul test case
- **Priority**: High / Medium / Low
- **Type**: Functional Positive/Negative, Validation, UI, Security
- **Pre-condition**: Kondisi awal sebelum testing
- **Test Steps**: Langkah-langkah testing
- **Test Data**: Data yang digunakan
- **Expected Result**: Hasil yang diharapkan
- **Actual Result**: Hasil yang didapat
- **Status**: PASS / FAILED / OPEN
- **Note**: Catatan tambahan
- **Severity**: Critical / High / Medium / Low
- **Severity Impact**: Penjelasan dampak bug

## Tools yang Digunakan

- **Browser**: Google Chrome
- **DevTools**: Chrome DevTools untuk memeriksa network request dan identifikasi masalah keamanan
- **Documentation**: Google Sheets / CSV untuk manajemen test case
- **Testing Method**: Manual testing dengan pendekatan black-box

## Metodologi Testing

1. **Test Planning**: Identifikasi fitur-fitur yang akan diuji
2. **Test Case Design**: Membuat test case berdasarkan alur pengguna
3. **Test Execution**: Menjalankan test case satu per satu
4. **Bug Reporting**: Dokumentasi bug dengan detail lengkap
5. **Severity Classification**: Kategorisasi bug berdasarkan dampak

## Statistik

- **Cakupan Testing**: 11 modul utama
- **Tingkat Keberhasilan**: 95%
- **Bug Kritis**: 3
- **Bug Prioritas Tinggi**: 2
- **Bug Prioritas Sedang**: 2

## Kemampuan yang Dipraktikkan

- Manual Testing
- Test Case Design dan Dokumentasi
- Bug Reporting dan Tracking
- Black Box Testing
- Security Testing (SQL Injection, XSS)
- Regression Testing
- User Acceptance Testing

## Kontak

Erlina Febiola Nainggolan
- Email: erlinanainggolan130104@gmail.com
- GitHub: github.com/Erlina130104
- Phone: +62 8971798041

## Lisensi

Proyek ini dibuat untuk keperluan portfolio dan pembelajaran.

---

**Catatan**: Website Practice Software Testing adalah platform publik yang dibuat khusus untuk latihan testing. Semua bug yang ditemukan telah didokumentasikan untuk tujuan pembelajaran.
