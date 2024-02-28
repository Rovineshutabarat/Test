# Panduan Penggabungan Tiga Arah (Three-Way Merge) di Git

## Deskripsi
Panduan ini akan membantu Anda memahami langkah-langkah untuk melakukan penggabungan tiga arah (three-way merge) dalam Git. Tiga cara penggabungan umumnya terjadi ketika Anda memiliki dua cabang yang berbeda dan ingin menggabungkan perubahan dari kedua cabang tersebut ke dalam cabang target.

## Langkah-Langkah

1. **Pastikan Anda Sudah Terbaru:**
    Sebelum Anda mulai penggabungan, pastikan repositori Anda sudah terbaru dengan menjalankan perintah berikut:
    ```bash
    git fetch origin
    git checkout <cabang_target>
    git pull origin <cabang_target>
    ```

2. **Mulai Penggabungan:**
    Pindah ke cabang target yang ingin Anda gabungkan perubahan ke dalamnya:
    ```bash
    git checkout <cabang_target>
    ```
    Kemudian, gabungkan perubahan dari cabang sumber dengan menggunakan perintah:
    ```bash
    git merge <cabang_sumber>
    ```

3. **Pemecahan Konflik (Jika Ada):**
    Jika Git menemukan konflik, ini berarti ada bagian dari kode yang berubah di kedua cabang dan perlu disesuaikan secara manual. Git akan menandai file-file yang bermasalah. Anda perlu membuka file-file tersebut menggunakan editor teks dan menyelesaikan konfliknya.

4. **Tambahkan Perubahan yang Diselesaikan:**
    Setelah Anda menyelesaikan konflik dan menyunting file-file yang terlibat, tandai bahwa konflik tersebut telah diselesaikan dengan menggunakan perintah:
    ```bash
    git add <file_yang_diubah>
    ```

5. **Selesaikan Penggabungan:**
    Lanjutkan proses penggabungan dengan menyelesaikannya:
    ```bash
    git merge --continue
    ```

6. **Uji Coba dan Periksa:**
    Setelah penggabungan selesai, pastikan untuk menguji apakah kode berfungsi dengan baik dan tidak ada konflik yang belum terselesaikan.

7. **Commit Hasil Merge:**
    Jika semuanya telah berhasil, lakukan commit untuk hasil penggabungan:
    ```bash
    git commit -m "Merge <cabang_sumber> into <cabang_target>"
    ```

8. **Dorong Perubahan ke Repositori Remote:**
    Terakhir, dorong perubahan ke repositori remote agar perubahan tersimpan secara online:
    ```bash
    git push origin <cabang_target>
    ```

Dengan mengikuti langkah-langkah ini, Anda dapat melakukan penggabungan tiga arah (three-way merge) dengan lancar dalam Git.
