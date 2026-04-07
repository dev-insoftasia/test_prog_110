# test_prog

Testing Programmer (Max 4 hari)
# **Note: Buat dengan laravel + livewire **
```
Buatkan juga LOGIN page sebelum masuk ke homepage.
```

1.	Buatlah halaman CRUD dengan html,css dengan framework yang biasa anda gunakan, untuk api CRUD bisa dilihat di dokumentasi (https://documenter.getpostman.com/view/18291185/2s93sXdFTV)
2. Buat function untuk mengetahui berapa banyak kata/words yang terdapat dalam suatu variable.
3. Buat function untuk menyisipkan satu kata/word ke dalam variable nomor 2 di atas.
4. Buat function pola segitiga:
	Input: Berapa banyak baris
	Output jika input diisi 5 baris, maka output harus menjadi:
	```
 	*
	**
	***
	****
	*****
5. Fungsi untuk mencari huruf yang sering muncul dalam sebuah kata.
	```
 	Input: Makan
	Hasil: a

6. Fungsi untuk mengurutkan sebuah array
   ```
	input: [5,3,6]
	hasil: [3,5,6]

7. Load Balancing
   ```
   Deskripsi singkat:  
	Aplikasi dideploy multi-instance di belakang load balancer. Livewire stateful dan background jobs (image processing) harus berjalan konsisten. Gunakan Redis untuk session dan queue driver; pastikan job balancing, retry/backoff, dan rate-limiting per-user.

	Tugas (implementasi & arsitektur):

	- Jelaskan dua pendekatan untuk session konsisten di lingkungan load-balanced: (1) sticky sessions di LB, (2) centralized session store (Redis). Bandingkan pro/kontra (scalability, failover, cache locality).

	- Berikan config/session.php snippet untuk Redis session store dan contoh langkah migrasi session file → Redis tanpa downtime (checklist).

	- Buat job ProcessImage yang memproses gambar dalam beberapa langkah (thumbnail, convert webp, optimasi, upload CDN) menggunakan job chaining / batching; pastikan idempotency.

	- Rancang strategi queue prioritization: multiple queues (e.g., high, default, low), worker pools terpisah, atau weighted workers; sertakan contoh supervisor/systemd/supervisord config konsep.

	- Jelaskan retry policy, exponential backoff, dead-letter handling, dan cara menggunakan Redis untuk rate-limiting job per user (mis. sorted sets atau token bucket).


Note: buat repository di github dengan isi file dari solusi permintaan diatas, lalu invite dua akun berikut: 
 ```
aldosaputra30 ,dev-insoftasia

