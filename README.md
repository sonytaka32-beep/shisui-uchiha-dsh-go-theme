# Shisui Uchiha — DSH-Go Native Pet Pack (True 4x HD)

Tema karakter **Shisui Uchiha** untuk **DSH-Go** menggunakan format **Native Pet Pack (`schema: 1`)** yang telah ditingkatkan ke resolusi **4x HD** dengan rendering pixel-art tajam (`pixelArt: true`).

## Pembaruan Versi HD (4x Scale)
- **Scale:** Ditingkatkan dari `2x` ke `4x` (resolusi frame sprite digandakan, mis. `idle` dari `352×362` menjadi `704×724` piksel).
- **Anti-Blur Rendering:** Mengaktifkan `"pixelArt": true` pada `pack.json` agar Android tidak menerapkan filter *bilinear blur* saat ditampilkan pada ukuran **Large**.
- **Logical Layout Preserved:** `canvas` (`192×208`), `anchor` (`95, 205`), `contentBox` (`176×30`), dan `hitBoxes` (`176×181`) tetap presisi pada koordinat dasar.

## Cara Instalasi
1. Unduh atau buat arsip `.zip` berisi `pack.json` beserta seluruh file sprite `.png`.
2. Buka **DSH-Go** → masuk ke menu **Pets → Import**.
3. Pilih file `.zip` tema ini, lalu pilih **Shisui Uchiha**.
4. Atur **Size = Large** untuk tampilan paling tajam.

## Catatan Penting
- Semua file sprite `.png` dalam repositori ini telah di-upscale dari resolusi 2x ke 4x menggunakan nearest-neighbor resampling (menggunakan Pillow `Image.Resampling.NEAREST`) untuk mempertahankan kemurnian pixel art.
- Nilai `frameW` dan `frameH` pada `pack.json` telah dikalikan 2x sesuai dengan perkalian `logical_size × scale`.
- Tidak perlu mengubah `canvas`, `anchor`, `contentBox`, atau `hitBoxes` — nilai-nilai ini tetap sama karena merupakan satuan logis 1x.
- Skema `schema: 1` tetap utuh untuk kompatibilitas dengan DSH-Go.