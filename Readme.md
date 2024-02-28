<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Panduan Penggabungan Tiga Arah (Three-Way Merge) di Git</title>
</head>
<body>
    <h1>Panduan Penggabungan Tiga Arah (Three-Way Merge) di Git</h1>

    <h2>Deskripsi</h2>
    <p>
        Panduan ini akan membantu Anda memahami langkah-langkah untuk melakukan penggabungan tiga arah (three-way merge) dalam Git. Tiga cara penggabungan umumnya terjadi ketika Anda memiliki dua cabang yang berbeda dan ingin menggabungkan perubahan dari kedua cabang tersebut ke dalam cabang target.
    </p>

    <h2>Langkah-Langkah</h2>
    <ol>
        <li>
            <strong>Pastikan Anda Sudah Terbaru:</strong>
            <p>
                Sebelum Anda mulai penggabungan, pastikan repositori Anda sudah terbaru dengan menjalankan perintah berikut:
            </p>
            <pre><code>git fetch origin
git checkout &lt;cabang_target&gt;
git pull origin &lt;cabang_target&gt;</code></pre>
        </li>
        <li>
            <strong>Mulai Penggabungan:</strong>
            <p>
                Pindah ke cabang target yang ingin Anda gabungkan perubahan ke dalamnya:
            </p>
            <pre><code>git checkout &lt;cabang_target&gt;</code></pre>
            <p>
                Kemudian, gabungkan perubahan dari cabang sumber dengan menggunakan perintah:
            </p>
            <pre><code>git merge &lt;cabang_sumber&gt;</code></pre>
        </li>
        <!-- Sisanya langkah-langkah lainnya -->
    </ol>
</body>
</html>
