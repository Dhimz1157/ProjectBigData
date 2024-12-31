<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Laporan Proyek Akhir Mata Kuliah</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            color: #333;
        }
        .container {
            max-width: 800px;
            margin: 20px auto;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        h1, h2, h3 {
            color: #2c3e50;
        }
        code {
            background: #eef;
            padding: 2px 4px;
            border-radius: 4px;
        }
        pre {
            background: #f9f9f9;
            padding: 10px;
            border-radius: 4px;
            overflow-x: auto;
        }
        ul {
            margin: 0;
            padding: 0;
            list-style: none;
        }
        ul li {
            padding: 5px 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Laporan Proyek Akhir Mata Kuliah</h1>

        <h2>Pendahuluan</h2>
        <p>Proyek ini bertujuan untuk menganalisis dataset dari dunia nyata menggunakan pendekatan eksplorasi data dan visualisasi. Analisis dilakukan untuk menggali wawasan yang dapat mendukung pengambilan keputusan. Dataset yang digunakan berasal dari Spotify, yang mencakup informasi lagu seperti popularitas, genre, durasi, serta berbagai fitur audio. Cerita yang dihasilkan dari analisis ini akan membimbing kita untuk memahami bagaimana elemen-elemen data berkorelasi dan memengaruhi hasil akhir.</p>

        <h2>Gambaran Umum Dataset</h2>
        <h3>Tipe Data</h3>
        <ul>
            <li>Dataset terdiri dari 23 kolom dengan berbagai tipe data:</li>
            <li>Numerik: <code>int64</code>, <code>float64</code> (contohnya <code>track_popularity</code>, <code>danceability</code>, <code>tempo</code>).</li>
            <li>Kategorikal: <code>object</code> (contohnya <code>track_name</code>, <code>playlist_genre</code>).</li>
        </ul>

        <h3>Ringkasan Statistik untuk Fitur Numerik</h3>
        <ul>
            <li>Rata-rata durasi lagu: 225.800 ms (3,76 menit), dengan rentang dari 4 detik hingga 8,63 menit.</li>
            <li>Popularitas lagu berkisar antara 0 hingga 100, dengan rata-rata 42,48.</li>
            <li>Danceability memiliki rata-rata 0,65 dengan penyebaran standar 0,15.</li>
        </ul>

        <h3>Cek Nilai Null</h3>
        <ul>
            <li>Kolom <code>track_name</code>, <code>track_artist</code>, dan <code>track_album_name</code> memiliki masing-masing 5 nilai null.</li>
            <li>Kolom lainnya tidak memiliki nilai null.</li>
        </ul>

        <h3>Cek Nilai Duplikat</h3>
        <p>Tidak ditemukan baris duplikat dalam dataset, memperkuat keandalan analisis.</p>

        <h2>Eksplorasi dan Analisis Data</h2>
        <h3>Popularitas Genre dan Subgenre</h3>
        <ul>
            <li>Genre terpopuler adalah <code>pop</code> dengan rata-rata popularitas 47,74, diikuti oleh <code>latin</code> dengan 47,03.</li>
            <li>Subgenre terpopuler adalah <code>dance pop</code> dengan rata-rata popularitas 52,08.</li>
        </ul>

        <h3>Lagu-lagu Terpopuler Berdasarkan Artis</h3>
        <ul>
            <li>Lagu paling populer: "Dance Monkey" oleh Tones and I (popularitas 100).</li>
            <li>Lagu "ROXANNE" oleh Arizona Zervas berada di posisi teratas dengan skor popularitas hingga 99.</li>
        </ul>

        <h3>Subgenre Terpopuler Berdasarkan Genre</h3>
        <ul>
            <li>Genre <code>edm</code> memiliki subgenre terpopuler <code>pop edm</code> (popularitas 45,69).</li>
            <li>Genre <code>pop</code> memiliki subgenre terpopuler <code>post-teen pop</code> (popularitas 56,83).</li>
        </ul>

        <h3>Distribusi Lagu Berdasarkan Tahun Rilis</h3>
        <ul>
            <li>Lagu tertua berasal dari tahun 1957.</li>
            <li>Lagu-lagu dari era 1960-an mulai menambah frekuensi.</li>
        </ul>

        <h3>Tren Popularitas Selama Bertahun-tahun</h3>
        <ul>
            <li>Lagu dari tahun 1958 memiliki popularitas rata-rata tertinggi dalam data awal dengan skor 73.</li>
            <li>Tren selanjutnya menunjukkan fluktuasi popularitas.</li>
        </ul>

        <h3>Distribusi Danceability</h3>
        <ul>
            <li>Rata-rata danceability adalah 0,65.</li>
            <li>Sebagian besar lagu memiliki danceability antara 0,56 hingga 0,76.</li>
        </ul>

        <h2>Rangkuman</h2>
        <h3>Kesimpulan</h3>
        <ul>
            <li>Genre <code>pop</code> dan subgenre <code>dance pop</code> mendominasi popularitas.</li>
            <li>Lagu "Dance Monkey" oleh Tones and I menjadi bukti bagaimana viralitas dapat memengaruhi kesuksesan global.</li>
            <li>Popularitas lagu fluktuatif, mencerminkan perubahan preferensi pendengar dari waktu ke waktu.</li>
        </ul>

        <h3>Keterbatasan</h3>
        <ul>
            <li>Data mungkin memiliki bias terhadap genre tertentu atau tidak mencakup seluruh aspek yang relevan.</li>
            <li>Analisis lebih lanjut diperlukan untuk memahami pengaruh variabel lain seperti demografi pendengar.</li>
        </ul>

        <h3>Saran Pengembangan</h3>
        <ul>
            <li>Mengintegrasikan data tambahan seperti data demografi atau interaksi di platform streaming untuk analisis yang lebih kaya.</li>
            <li>Menggunakan model prediktif untuk memperkirakan popularitas lagu berdasarkan fitur audio.</li>
        </ul>

        <h2>Package yang Digunakan</h2>
        <ul>
            <li><strong>Pandas:</strong> Untuk manipulasi data.</li>
            <li><strong>NumPy:</strong> Untuk operasi numerik.</li>
            <li><strong>Matplotlib dan Seaborn:</strong> Untuk visualisasi data.</li>
            <li><strong>Scikit-learn (jika digunakan):</strong> Untuk analisis klaster atau pemodelan prediktif.</li>
        </ul>
    </div>
</body>
</html>

