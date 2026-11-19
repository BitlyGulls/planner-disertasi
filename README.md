# Planner Disertasi

Planner disertasi berbasis HTML untuk Satrio Tunggul Satoto Jagad. Antarmuka Indonesia–Inggris, diagram Gantt, subkegiatan, dan checklist tersedia tanpa instalasi atau dependensi eksternal.

## Membuka aplikasi

Buka [Planner Disertasi](https://bitlygulls.github.io/planner-disertasi/) atau buka `index.html` di Chrome atau Edge.

## Penggunaan

- Tambahkan kegiatan dan tonggak melalui tombol di bagian atas.
- Pilih kegiatan, lalu klik **+ Subkegiatan**. Gunakan panah **▸** di samping nama kegiatan untuk membuka atau menutup daftar subkegiatan.
- Centang subkegiatan yang selesai. Persentase induk dihitung otomatis: jumlah yang dicentang dibagi jumlah seluruh subkegiatan, dengan bobot yang sama dan pembulatan ke bilangan terdekat. Induk tanpa subkegiatan bernilai 0%.
- Edit tanggal pada subkegiatan. Rentang tanggal induk mengikuti subkegiatannya. Menggeser batang induk turut menggeser seluruh subkegiatan; perubahan tanggal tidak menjadwalkan ulang kegiatan lain secara otomatis.
- Gunakan tombol **− / +** atau penggeser untuk mengubah tampilan triwulan dan bulanan. Tampilan awal adalah bulanan.
- Tampilan awal menggunakan **tema gelap** dan **bahasa Inggris**. Saklar **Light / Dark** dan **ID / EN** menyimpan pilihan terakhir Anda di browser. Data jadwal dan checklist lama tetap dipertahankan saat pengaturan awal ini diperbarui.
- Gunakan saklar **ID / EN** untuk mengganti bahasa. Nama dan catatan bawaan tersedia dalam dua bahasa. Untuk teks tambahan, isi **Terjemahan opsional**; aplikasi tidak menerjemahkan teks baru secara otomatis.
- Gunakan **Urungkan** untuk membatalkan perubahan terakhir pada sesi yang sedang berjalan.

## Penyimpanan dan cadangan

Perubahan disimpan di penyimpanan lokal browser jika tersedia. Perubahan tersebut **tidak otomatis tersimpan ke GitHub atau tersinkron ke perangkat lain**. Situs tidak mengirim jadwal atau checklist yang diedit ke layanan eksternal.

- **Simpan HTML**: unduh salinan aplikasi lengkap dengan jadwal, checklist, dan bahasa terbaru.
- **Cadangkan data**: unduh JSON berisi data planner.
- **Buka data**: muat JSON cadangan, termasuk format versi pertama planner.

Penyimpanan versi berkas lokal dan situs daring dapat berbeda. Untuk membawa perubahan dari berkas lokal ke situs, gunakan **Cadangkan data**, lalu **Buka data** pada situs. Buat cadangan sebelum mengganti browser, perangkat, atau menghapus data situs. Jika penyimpanan lokal tidak tersedia, gunakan unduhan HTML atau JSON.

## Status jadwal

Jadwal bawaan adalah **rencana kerja sementara**, bukan kalender akademik atau keputusan promotor. Waktu seminar, ujian, dan persyaratan publikasi perlu mengikuti ketentuan prodi. Jadwal artikel menunjukkan target pengiriman, bukan kepastian penerimaan. Persentase awal 0% adalah isian awal aplikasi, bukan penilaian kemajuan penelitian.

## Struktur repositori

- `index.html`: aplikasi mandiri, mencakup tampilan, logika, dan jadwal awal.
- `.nojekyll`: menyajikan aplikasi sebagai berkas statis melalui GitHub Pages.

## English

A standalone bilingual dissertation planner with an editable Gantt chart, expandable subtasks, checklists, monthly/quarterly zoom, and a light/dark theme switch. The initial appearance is dark with English selected. Your later theme and language choices are remembered in the current browser. Parent progress is the equally weighted fraction of completed subtasks. Parent dates follow the subtasks, and dragging a parent shifts them together.

Open `index.html` in Chrome or Edge, or use this repository's GitHub Pages site. Use the ID/EN switch for the interface and built-in content. Additional text can be entered in both languages through Optional translation.

Changes stay in the current browser and are not automatically committed to GitHub or synchronized between devices. Use Save HTML or Back up data to retain your changes, and Open data to restore a JSON backup. The initial academic schedule is provisional and requires supervisory and program confirmation.
