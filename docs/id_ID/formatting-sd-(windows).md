# Memformat kartu SD (Windows)

## Bacaan Penting

Ini adalah laman lebihan untuk memformat kartu SD agar terbaca di 3DS.

Jika 3DS sudah bisa membaca kartu SD, panduan ini tidak perlu.

Laman ini khusus pengguna Windows. Jika tidak menggunakan Windows, lihat laman [Memformat kartu SD (Linux)](formatting-sd-(linux)) atau [Memformat kartu SD (Mac)](formatting-sd-(mac)).

## Apa yang Perlu

- The latest version of [guiformat](https://nintendohomebrew.com/guiformat)

## Instruksi

1. Jalankan `guiformat.exe`

2. Pilih huruf kandar kartu SD Anda di kolom "Drive"

   ::: danger

   Pastikan pilih huruf kandar (_drive_) yang benar, **jangan memformat _drive_ yang salah**!

   :::

3. Pilih ukuran di "Allocation unit size"
   - Jika ukuran kartu SD 64GB, pilih 32768
   - Jika ukuran kartu SD lebih dari 64GB, pilih 65536

4. Ketik apa saja di "Volume label"

5. Pastikan "Quick Format" sudah dipilih

6. Pencet "Start" (Mulai)

7. Pencet "OK"

8. Tunggu selesai memformat

9. Pencet "Close" (Tutup)

10. Jika tadi kartu SD ada berkas dan folder sebelum memformat, **salin balik semuanya dari komputer**

## Sidik Gangguan

- guiformat muncul galat "Failed to open device: GetLastError()=32"
  - Tutup semua aplikasi yang membaca kartu SD, seperti jendela File Explorer.
  - Jika masih ada isu, coba format ulang kartunya ke NTFS di File Explorer, tutup jendelanya saat selesai, dan coba lagi dengan guiformat.

- guiformat muncul galat "GetLastError()=1117"
  - Perlindungan-tulis pada kartu SD mungkin [aktif](/images/sdlock.png). Pengunci harus di posisi atas agar bisa menulis ke kartu SD (termasuk memformat).

- Kartu SD tetap tidak terbaca konsol atau daya tampungnya salah setelah diformat
  - Kartu SD mungkin dipartisi atau ada ruang tak dialokasikan. Ikuti [instruksi ini](https://wiki.hacks.guide/wiki/SD_Clean/Windows) untuk memformat ulang kartu SD.
