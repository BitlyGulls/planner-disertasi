# Planner Disertasi

Planner HTML Indonesia–Inggris dengan diagram Gantt, subkegiatan, checklist, dan tombol simpan ke Google Drive.

Buka [Planner Disertasi](https://bitlygulls.github.io/planner-disertasi/).

## Simpan dan lanjutkan di perangkat lain

1. Klik **Open Google Drive / Buka Google Drive**, lalu pilih akun Google Anda. Planner membuka simpanan terakhir dari akun tersebut.
2. Edit kegiatan, tanggal, dan checklist. Status menunjukkan **Unsaved changes / Perubahan belum disimpan**.
3. Klik **Save to Google Drive / Simpan ke Google Drive**. Tunggu status **Saved to Google Drive / Tersimpan di Google Drive**.
4. Pada PC, laptop, atau HP lain, buka situs yang sama dan klik **Open Google Drive** dengan akun yang sama.
5. Gunakan **Reload from Drive / Muat ulang dari Drive** untuk membuka versi tersimpan terbaru pada tab yang sudah terbuka.

**Tidak ada autosave ke Drive.** Perubahan hanya diunggah saat tombol Save ditekan, termasuk tombol pilihan **Save this version** saat ada perbedaan versi. Pintasan Ctrl+S atau Cmd+S juga menjalankan Save to Google Drive pada situs daring. Tema, bahasa, zoom, dan daftar yang sedang dibuka mengikuti browser masing-masing.

Draf lokal disimpan di browser sebagai bantuan melanjutkan pekerjaan. Draf tersebut belum tersedia di perangkat lain sampai Anda menekan Save. Saat sesi Google berakhir, tekan Save atau Open Google Drive untuk menghubungkan kembali. Jika ada versi berbeda di Drive, pilih **Open Drive version** atau **Save this version**. Jangan menyunting rencana yang sama bersamaan pada banyak perangkat; setelah berpindah, buka simpanan terbaru terlebih dahulu.

Setiap Save yang mengubah data membuat snapshot baru; simpanan sebelumnya tetap ada. Aplikasi memakai yang terbaru berdasarkan waktu pembuatan di Drive. Belum tersedia antarmuka untuk memilih riwayat snapshot. Dua penyimpanan serentak dapat sama-sama tersimpan; versi dengan waktu pembuatan terbaru akan dibuka berikutnya. Buat ekspor JSON untuk cadangan yang mudah Anda kelola.

## Lokasi dan akses data

Simpanan berada di **folder data aplikasi pribadi** di Google Drive (`appDataFolder`). Folder ini tersembunyi dari daftar berkas Drive dan dibuka melalui planner. Aplikasi hanya meminta akses ke data aplikasinya sendiri serta identitas dan email akun; aplikasi tidak meminta akses ke seluruh dokumen Drive Anda. Lihat [penjelasan Google](https://developers.google.com/workspace/drive/api/guides/appdata).

Tidak ada Firebase atau database tambahan dalam alur penyimpanan planner ini. Situs tetap di GitHub Pages. Progres pribadi tidak dimasukkan ke repositori GitHub. Setiap snapshot dibatasi 5 MB. Snapshot menggunakan kapasitas akun Drive, dan pemakaian tetap mengikuti batas layanan Google.

Koneksi memakai Google Identity Services. Token akses hanya ada di memori tab, bukan di HTML, GitHub, atau penyimpanan browser. ID klien yang ada dalam kode adalah identitas publik aplikasi dan bukan kata sandi.

## Kegiatan dan jadwal

- Tambahkan kegiatan, subkegiatan, atau tonggak melalui tombol bagian atas. Buka daftar subkegiatan melalui panah di samping kegiatan.
- Centang subkegiatan yang selesai. Persentase induk = jumlah subkegiatan dicentang dibagi seluruh subkegiatan, berbobot sama dan dibulatkan. Induk tanpa subkegiatan bernilai 0%.
- Subkegiatan baru berdurasi satu hari. Atur tanggal mulai dan selesainya; batang subkegiatan mengikuti tanggalnya sendiri.
- Tanggal induk merangkum rentang subkegiatannya. Menggeser induk turut menggeser seluruh subkegiatan.
- Gunakan zoom untuk tampilan bulanan atau triwulan. Tampilan awal bulanan, tema gelap, dan bahasa Inggris.
- Pada HP portrait, tab **Tasks / Kegiatan** menampilkan daftar dan checklist; tab **Gantt** menampilkan diagram yang dapat digeser. Detail diedit melalui panel bawah.
- Saklar ID/EN mengganti antarmuka dan teks bawaan. Teks tambahan dapat diisi dalam dua bahasa melalui Terjemahan opsional.
- Gunakan Undo untuk membatalkan perubahan pada sesi berjalan.

## Cadangan dan salinan HTML

- **Save HTML / Simpan HTML** mengunduh aplikasi lengkap beserta data terbaru.
- **Back up data / Cadangkan data** mengunduh JSON progres.
- **Open data / Buka data** memuat JSON cadangan. Tekan Save to Google Drive jika ingin mengirim hasil impor ke akun.

HTML yang dibuka sebagai berkas lokal (`file://`) mendukung pengeditan dan draf lokal, tetapi tidak login atau menyimpan ke Google Drive. Untuk melanjutkan melalui Drive, buka situs daring dan impor JSON cadangan. Ekspor cadangan sebelum menghapus data browser.

## Status akademis

Jadwal bawaan adalah rencana sementara untuk dibahas bersama promotor. Tanggal seminar dan ujian mengikuti ketentuan prodi. Jadwal artikel merupakan target pengiriman, bukan kepastian penerimaan. Persentase awal 0% merupakan isian awal, bukan penilaian kemajuan penelitian.

## English

A bilingual dissertation planner with an editable Gantt chart, expandable subtasks, checklist-based progress, monthly/quarterly zoom, and dark/light themes. Dark mode and English are the defaults. Portrait mobile uses a task list with a separate Gantt tab.

Use **Open Google Drive** with the same account on each device. Edit, then press **Save to Google Drive** and wait for the saved status. Changes are never uploaded automatically. A browser-local draft is kept separately. Use **Reload from Drive** to open the latest saved version. If versions differ, choose explicitly which one to keep. Each changed save creates a private app-data snapshot; concurrent saves are retained and the latest is opened. Export JSON for a manageable backup. Local HTML copies support offline editing; Google Drive access requires the online site.
