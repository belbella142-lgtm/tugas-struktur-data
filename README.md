# tugas-struktur-data
1. Analisis Ringkas: Array vs. List
Bayangkan sebuah lemari penyimpanan:
- Array: Seperti loker permanen. Ukurannya sudah ditentukan dari awal (misal: 10 pintu). Anda tidak bisa menambah pintu loker di tengah jalan, tapi sangat efisien karena tidak ada ruang yang terbuang.
- List: Seperti tas ransel yang bisa melar. Anda bisa terus memasukkan barang (ukuran berubah-ubah). Namun, karena "bisa melar", tas ini sebenarnya memakan ruang lebih besar dari yang terlihat untuk berjaga-jaga jika ada barang baru masuk.
Kapan pakai Array? Saat jumlah data sudah pasti dan kita ingin menghemat memori.
Kapan pakai List? Saat jumlah data bisa berubah-ubah dan kita butuh banyak fitur seperti hapus/tambah otomatis.

2. Implementasi Game of Life (Sesimpel Mungkin)
Dalam dokumen tersebut, Game of Life adalah simulasi sel hidup/mati pada papan kotak-kotak.
Aturan Utama:
- Tetangga: Dihitung dari 8 kotak di sekeliling sel.
- Bertahan Hidup: Sel hidup tetap hidup jika punya 2-3 tetangga hidup.
- Mati: Terlalu sepi (0-1 tetangga) atau terlalu ramai (>=4 tetangga).
- Lahir: Sel mati jadi hidup jika punya tepat 3 tetangga hidup.
Logika Sederhana Menggunakan ADT Array:
Jika kita ingin membuat simulasi ini secara manual di Python menggunakan konsep Array yang kaku (sesuai dokumen):
- Buat Array 2D (grid) dengan ukuran tetap.
- Gunakan fungsi getitem() untuk cek status sel dan setitem() untuk mengubahnya.
- Setiap "detik" (generasi), hitung tetangga tiap sel dan tentukan nasibnya untuk generasi berikutnya.
