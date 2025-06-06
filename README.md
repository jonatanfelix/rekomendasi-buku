# Sistem Rekomendasi Media Interaktif Buku & Manga

Aplikasi ini adalah sistem rekomendasi media interaktif berbasis web yang dibangun dengan Streamlit. Dirancang untuk membantu pengguna mencari, menemukan, dan mengelola daftar bacaan dari berbagai sumber online (Google Books, Open Library, MyAnimeList) serta memanfaatkan kecerdasan buatan (LLM) untuk analisis dan rekomendasi cerdas.

## Fitur Unggulan

- **Pencarian Multi-Sumber**: Cari buku, manga, dan media lain secara langsung dari Google Books, Open Library, dan MyAnimeList dalam satu aplikasi.
- **Rekomendasi AI (LLM)**: Dapatkan saran "Baca/Tonton Jika Suka..." dan ringkasan ulasan otomatis berbasis LLM (Large Language Model) untuk pengalaman rekomendasi yang lebih personal dan cerdas.
- **Terjemahan Otomatis**: Terjemahkan deskripsi dan latar belakang buku/manga ke Bahasa Indonesia secara instan dengan AI.
- **Manajemen Daftar Bacaan Pribadi**: Simpan item favorit ke daftar bacaan kustom Anda, buat dan kelola beberapa daftar sesuai kebutuhan.
- **Antarmuka Modern & Mudah Digunakan**: UI responsif, navigasi tab, dan modal detail yang informatif.
- **Tanpa Database Lokal**: Semua data daftar bacaan disimpan di session browser, tanpa instalasi database tambahan.
- **Login Sederhana**: Cukup masukkan ID unik untuk mengelola daftar bacaan Anda selama sesi berlangsung.
- **Pagination & Load More**: Navigasi hasil pencarian dengan mudah, muat lebih banyak data dari API jika tersedia.
- **Open Source & Mudah Dikembangkan**: Kode Python yang bersih, modular, dan mudah dikustomisasi.

## Cara Instalasi

1. **Clone repository ini**

   ```bash
   git clone <url-repo-anda>
   cd final_project
   ```

2. **Buat dan aktifkan virtual environment (opsional tapi disarankan)**

   ```bash
   python -m venv myenvy
   # Windows:
   myenvy\Scripts\activate
   # Mac/Linux:
   source myenvy/bin/activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **(Opsional) Siapkan API Key**

   - Untuk hasil maksimal, dapatkan API Key Google Books dan OpenRouter (LLM) lalu simpan di file `.streamlit/secrets.toml`:

     ```toml
     GOOGLE_BOOKS_API_KEY = "your_google_books_api_key"
     OPENROUTER_API_KEY = "your_openrouter_api_key"
     ```

5. **Jalankan aplikasi**

   ```bash
   streamlit run final_project.py
   ```

## Cara Penggunaan

1. Masukkan ID pengguna unik Anda di sidebar untuk mulai mengelola daftar bacaan.
2. Gunakan tab "Cari & Temukan" untuk mencari buku/manga dari berbagai sumber.
3. Klik "Lihat Detail" untuk membuka modal detail, terjemahkan deskripsi, dapatkan ringkasan ulasan, atau saran AI.
4. Simpan item ke daftar bacaan pribadi Anda, buat daftar baru sesuai kebutuhan.
5. Kelola daftar bacaan di tab "Daftar Bacaan Saya".

## Teknologi yang Digunakan
- Python 3.10+
- Streamlit
- Pandas, Numpy
- Scikit-learn (untuk fitur lanjutan, jika diaktifkan)
- Requests
- OpenRouter API (LLM)
- Google Books API, Open Library API, Jikan (MyAnimeList) API

## Keunggulan Dibanding Aplikasi Lain
- **Integrasi Multi-Sumber**: Tidak hanya satu API, tapi tiga sumber besar sekaligus.
- **AI-Driven**: Fitur LLM untuk rekomendasi dan ringkasan, bukan sekadar pencarian biasa.
- **User Experience Modern**: Modal detail, expander, dan navigasi tab yang nyaman.
- **Privasi & Simplicity**: Tidak perlu login email/password, cukup ID unik.
- **Mudah Dikembangkan**: Cocok untuk tugas akhir, demo, atau pengembangan lebih lanjut.

## Catatan Penting
- Data daftar bacaan hanya tersimpan selama sesi browser aktif (session-based, bukan cloud/database).
- API eksternal memiliki rate limit, gunakan dengan bijak.
- Untuk fitur AI, pastikan API key OpenRouter valid dan saldo cukup.

## Kontribusi
Pull request, issue, dan saran pengembangan sangat diterima!

## Lisensi
MIT License
