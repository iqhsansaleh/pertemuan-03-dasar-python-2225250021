# pertemuan-03-dasar-python-2225250021

Nama: Iqhsan Saleh

NIM: 2225250021

Kelas: 3A

## Tujuan
Menulis program seleksi if, if-else, kondisi majemuk, dan nested if.

## Cara Menjalankan
python3 tugas/analisis_persamaan_kuadrat.py

## Algoritma Tugas
1. Menerima masukan tiga koefisien angka (float) yaitu a, b, dan c dari pengguna.
2. Memeriksa apakah nilai a sama dengan 0. Jika benar, program menampilkan "Bukan persamaan kuadrat."
3. Jika a tidak sama dengan 0, program menghitung nilai diskriminan menggunakan rumus D = b**2 - 4*a*c.
4. Menggunakan struktur nested if untuk mengecek kondisi diskriminan:
   - Jika D > 0, menghitung dan menampilkan dua akar real berbeda (x1 dan x2).
   - Jika D == 0, menghitung dan menampilkan satu akar real kembar (x).
   - Jika D < 0, menampilkan pesan bahwa tidak ada akar real.
5. Menampilkan seluruh hasil numerik dengan format dua angka di belakang koma.

## Hasil Pengujian
| a | b | c | D | Keluaran yang Diharapkan | Keluaran Aktual | Status |
|:-:|:-:|:-:|:-:|---|---|---|
| 1 | -5 | 6 | 1 | Diskriminan = 1.00<br>Dua akar real: x1 = 3.00, x2 = 2.00 | Diskriminan = 1.00<br>Dua akar real: x1 = 3.00, x2 = 2.00 | Berhasil |
| 1 | 2 | 1 | 0 | Diskriminan = 0.00<br>Akar real kembar: x = -1.00 | Diskriminan = 0.00<br>Akar real kembar: x = -1.00 | Berhasil |
| 1 | 0 | 1 | -4 | Diskriminan = -4.00<br>Tidak ada akar real. | Diskriminan = -4.00<br>Tidak ada akar real. | Berhasil |
| 0 | 2 | 3 | - | Bukan persamaan kuadrat. | Bukan persamaan kuadrat. | Berhasil |

## Refleksi
Kesalahan logika yang sempat terjadi pada awal pembuatan kode adalah lupa memberikan tanda kurung pada bagian penyebut rumus kuadrat (menulis `-b + d ** 0.5 / 2 * a` alih-alih `(-b + d ** 0.5) / (2 * a)`). Hal ini menyebabkan operasi matematika mendahulukan pembagian dan perkalian biasa secara keliru. Cara memperbaikinya adalah dengan menambahkan tanda kurung yang jelas pada pembilang dan penyebut agar seluruh bagian $2a$ benar-benar bertindak sebagai pembagi.
