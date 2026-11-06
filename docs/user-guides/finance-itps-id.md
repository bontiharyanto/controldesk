# Panduan Pengguna Finance — ControlDesk ITPS

Versi 1.0 • 6 November 2026 • Bahasa Indonesia

Panduan ini ditujukan untuk pengguna Finance, pemegang kas kecil, serta pengelola proyek yang berkoordinasi dengan Finance di tenant ITPS. Langkah-langkah disusun berdasarkan formulir dan alur aplikasi pada saat penyusunan. Menu dan tombol yang muncul mengikuti hak akses, status transaksi, serta pengaturan tenant. Label dapat ditampilkan dalam Bahasa Indonesia atau Bahasa Inggris.

## Daftar isi

1. Masuk dan mengenali menu Finance
2. Pembagian tugas dan persiapan data
3. Anggaran proyek (Budgets)
4. Perubahan anggaran (Budget Requests)
5. Pengeluaran proyek (Expenses)
6. Kas bon (Cash Advances)
7. Kas kecil (Petty Cash)
8. Kontrak (Contracts)
9. Persetujuan dan pemeriksaan dokumen
10. Rutinitas Finance dan contoh latihan
11. Pemecahan masalah
12. Istilah dan catatan versi

## 1. Masuk dan mengenali menu Finance

1. Buka https://itps.controldesk.site/login melalui peramban.
2. Masukkan email akun yang telah diaktifkan oleh administrator dan kata sandi Anda.
3. Setelah masuk, periksa nama akun dan pastikan Anda berada di tenant ITPS.
4. Buka kelompok menu **Finance / Keuangan** pada navigasi aplikasi.
5. Pilih modul sesuai pekerjaan. Buka detail transaksi untuk melihat dokumen, status, dan tindakan yang tersedia.

Jangan mencantumkan kata sandi dalam bukti transaksi atau membagikannya melalui manual ini. Untuk akun baru, kredensial disampaikan secara terpisah oleh administrator.

| Kebutuhan | Menu atau alamat halaman |
| --- | --- |
| Menyusun dan memantau anggaran | Budgets — /finance/budgets |
| Meninjau permintaan perubahan anggaran | Bagian Budget Requests pada detail anggaran |
| Memeriksa biaya yang sudah terjadi | Expenses — /finance/expenses |
| Memeriksa uang muka dan pertanggungjawaban | Cash Advances — /finance/cash-advances |
| Mengelola dana kas kecil | Petty Cash — /finance/petty-cash |
| Membaca informasi kontrak | Contracts — /finance/contracts |
| Melihat pengajuan yang perlu diputuskan | Approvals / Persetujuan — /approvals |
| Memeriksa daftar akun biaya | Chart of Accounts / Bagan Akun — /settings/coa, jika diizinkan |

## 2. Pembagian tugas dan persiapan data

**Finance / Lead Finance** memeriksa kelayakan transaksi, mengambil keputusan pada tahap Finance, mencatat pencairan, memeriksa pertanggungjawaban kas bon, dan menerapkan perubahan anggaran yang telah disetujui sesuai kewenangan.

**Pengaju atau pemilik kas bon** menyiapkan pengajuan dan bukti penggunaan dana. **PM dan pimpinan operasional** memeriksa kebutuhan proyek sesuai tahap persetujuannya. **Director** menangani persetujuan yang membutuhkan kewenangannya. **Custodian / pemegang kas kecil** mencatat penggunaan dana kas kecil sesuai penugasannya. **Tenant Admin** mengelola akun dan konfigurasi tenant.

Memiliki akses menu tidak berarti setiap transaksi dapat disetujui. Tindakan tetap dibatasi oleh peran, tahap persetujuan, penugasan, dan aturan aplikasi. Jika tombol tidak tersedia, minta administrator memeriksa hak akses; jangan memakai akun pengguna lain.

Sebelum memulai, siapkan:

- Proyek dan tahun anggaran yang benar.
- Unit Pengaju yang sesuai dengan proyek, bila kolom tersebut tersedia.
- Kategori biaya dan akun CoA yang tepat.
- Nominal, tanggal transaksi atau kebutuhan dana, serta uraian tujuan.
- Nota, kuitansi, atau dokumen pendukung yang terbaca.
- Persetujuan dan bukti transfer sesuai prosedur internal perusahaan.

Masukkan nominal sesuai petunjuk kolom. Pada kolom angka, gunakan misalnya **1500000** untuk Rp1.500.000. Periksa kembali nominal yang ditampilkan sebelum menyimpan.

## 3. Anggaran proyek (Budgets)

### 3.1 Membuat anggaran

1. Buka **Finance → Budgets**.
2. Pilih tombol tambah anggaran apabila tersedia untuk akun Anda.
3. Pilih proyek, tahun fiskal, judul anggaran, dan Unit Pengaju bila diperlukan. Tambahkan catatan untuk menjelaskan ruang lingkup anggaran.
4. Simpan. Aplikasi membuka detail anggaran dengan status **DRAFT**.
5. Tambahkan rincian biaya. Isi urutan, kategori, uraian, nominal rencana, dan akun CoA bila digunakan.
6. Periksa seluruh rincian serta totalnya sebelum mengajukan persetujuan.

Pembuatan anggaran dapat ditolak jika proyek masih berstatus DRAFT atau telah dihentikan. Pada implementasi saat ini, proyek PLANNING, ACTIVE, atau ON_HOLD dapat menerima anggaran, dengan tetap mengikuti pemeriksaan aplikasi lainnya.

**Contoh ilustratif:** anggaran operasional proyek Rp10.000.000 terdiri atas transport Rp3.000.000, konsumsi Rp2.000.000, dan perlengkapan Rp5.000.000. Gunakan kategori serta kode akun yang benar-benar tersedia di ITPS; contoh ini bukan data transaksi riil.

### 3.2 Mengajukan dan menyetujui anggaran

1. Buka detail anggaran dan periksa rincian yang akan diajukan.
2. Pilih **Submit / Ajukan** jika tombol tersedia.
3. Pada tahap **PENDING_FINANCE**, Finance memeriksa total, kategori, akun, dan kebutuhan proyek.
4. Pilih **Approve / Setujui** atau **Reject / Tolak** sesuai hasil pemeriksaan. Jika menolak, tulis alasan yang dapat ditindaklanjuti.
5. Jika persetujuan Director diperlukan, status berlanjut ke **PENDING_DIRECTOR**. Anggaran selesai disetujui setelah seluruh tahap terpenuhi.

Alur utama: **DRAFT → PENDING_FINANCE → PENDING_DIRECTOR bila diperlukan → APPROVED**. Ambang persetujuan mengikuti konfigurasi tenant dan ketentuan pengajuan. Penolakan anggaran pada implementasi saat ini berakhir sebagai **CANCELLED**, dengan alasan tercatat dalam riwayat.

### 3.3 Memantau penggunaan anggaran

Bandingkan nilai rencana dan realisasi pada rincian anggaran. Tinjau transaksi pendukung sebelum menyimpulkan penyebab selisih. Nilai yang disetujui, dicairkan, dan dipertanggungjawabkan menunjukkan tahapan yang berbeda.

Perubahan anggaran yang sudah disetujui sebaiknya diajukan melalui **Budget Requests**. Jangan membuat anggaran duplikat hanya untuk menghindari alur perubahan.

## 4. Perubahan anggaran (Budget Requests)

### 4.1 Memahami jenis perubahan

| Jenis | Kegunaan | Rincian yang dipilih |
| --- | --- | --- |
| INCREASE | Menambah alokasi | Rincian tujuan yang menerima tambahan |
| DECREASE | Mengurangi alokasi | Rincian sumber yang dikurangi |
| TRANSFER | Memindahkan alokasi antarrincian dalam anggaran | Rincian sumber dan tujuan yang berbeda |

### 4.2 Pengajuan oleh pengguna berwenang

1. Buka detail anggaran, lalu bagian **Budget Requests**.
2. Pilih tambah permintaan jika tersedia untuk peran Anda.
3. Pilih jenis perubahan, rincian sumber atau tujuan, dan nominal yang lebih besar dari nol.
4. Tulis justifikasi minimal **20 karakter**. Jelaskan alasan operasional, dasar perhitungan, dan dampaknya.
5. Ajukan dan pantau tahap persetujuan pada permintaan tersebut.

Jika akun Finance tidak menampilkan tombol pengajuan, koordinasikan dengan PM, OM, atau administrator yang berwenang. Finance tetap dapat menangani tahap pemeriksaan dan penerapan sesuai kewenangan.

### 4.3 Pemeriksaan dan penerapan oleh Finance

1. Periksa permintaan yang sedang menunggu Finance.
2. Cocokkan nominal dan rincian sumber/tujuan dengan kebutuhan proyek.
3. Untuk DECREASE dan TRANSFER, pastikan pengurangan tidak mengganggu biaya yang sudah digunakan atau komitmen proyek.
4. Setujui atau tolak dengan alasan yang jelas. Jika masih ada tahap Director, tunggu sampai selesai.
5. Setelah status **APPROVED**, gunakan **Apply / Terapkan** apabila tersedia.
6. Pastikan status menjadi **APPLIED** dan nominal rincian anggaran telah berubah sesuai permintaan.

**APPROVED** berarti permintaan telah mendapat persetujuan. **APPLIED** berarti perubahan telah diterapkan. Permintaan yang hanya berstatus APPROVED belum boleh dianggap selesai diterapkan.

Contoh: transfer Rp500.000 dari perlengkapan ke transport mengurangi alokasi perlengkapan dan menambah alokasi transport dengan jumlah yang sama. Total anggaran tetap sama.

## 5. Pengeluaran proyek (Expenses)

Expense digunakan untuk mencatat pengeluaran yang telah terjadi. Gunakan kas bon apabila kebutuhan utamanya adalah meminta uang muka sebelum kegiatan.

### 5.1 Menyiapkan pengajuan

1. Buka **Finance → Expenses** dan pilih tambah pengeluaran jika diizinkan.
2. Pilih proyek dan rincian anggaran yang sesuai. Pilih akun CoA bila tersedia.
3. Isi nominal, tanggal kejadian transaksi, metode pembayaran, uraian, dan catatan yang diperlukan.
4. Unggah bukti pengeluaran. Isi alasan keterlambatan jika formulir memintanya.
5. Ikuti pilihan simpan draf atau pengajuan yang tersedia. Pastikan notifikasi berhasil muncul dan periksa status hasilnya.

### 5.2 Pemeriksaan oleh Finance

1. Buka transaksi dari daftar Expenses atau kotak Persetujuan.
2. Cocokkan nominal dengan bukti; periksa tanggal, pihak penerima, tujuan, dan keterkaitan dengan proyek.
3. Periksa kategori, akun CoA, serta kemungkinan pengajuan ganda.
4. Baca riwayat persetujuan. Ambil keputusan saat transaksi berada pada tahap Finance dan tombol tersedia.
5. Tulis alasan spesifik jika menolak, misalnya “Nominal pengajuan Rp750.000, sedangkan bukti yang dilampirkan Rp570.000.”
6. Periksa status setelah keputusan. Pengajuan dapat berlanjut ke tahap berikutnya sesuai alurnya.

Status **APPROVED** menunjukkan penyelesaian persetujuan. Cocokkan pembayaran aktual dengan bukti transfer dan prosedur kas perusahaan; jangan menganggap persetujuan sebagai bukti bahwa bank telah memindahkan dana.

## 6. Kas bon (Cash Advances)

Kas bon merupakan uang muka kegiatan yang harus dipertanggungjawabkan. Aplikasi menyediakan jenis **GENERAL** dan **FIELD_OPS**; formulir serta tahap persetujuannya mengikuti jenis yang dipilih.

### 6.1 Pengajuan kas bon

1. Pengaju membuka **Finance → Cash Advances** dan memilih tambah kas bon atau formulir Field Ops yang tersedia.
2. Pilih jenis, proyek, nominal, tanggal kebutuhan, tujuan, Unit Pengaju, serta akun CoA jika digunakan.
3. Untuk Field Ops, lengkapi rincian kegiatan lapangan yang diminta formulir.
4. Periksa data dan dokumen, lalu ajukan menggunakan tindakan yang tersedia.
5. Pantau status serta alasan penolakan jika pengajuan tidak disetujui.

### 6.2 Pemeriksaan dan pencairan oleh Finance

1. Buka detail kas bon yang menunggu tahap Finance.
2. Periksa tujuan, nominal, dokumen, proyek, dan riwayat persetujuannya.
3. Ambil keputusan pada tahap Anda. Tunggu seluruh persetujuan selesai sebelum mencairkan.
4. Setelah **APPROVED**, lakukan pembayaran sesuai prosedur internal.
5. Gunakan **Disburse / Cairkan** dan isi informasi yang diminta sesuai pencairan aktual.
6. Pastikan status menjadi **DISBURSED**. Periksa tanggal dan nominal pencairan serta tenggat pertanggungjawaban yang tercantum.

Pencatatan pencairan di aplikasi tidak menggantikan proses transfer bank atau penyerahan uang.

### 6.3 Pertanggungjawaban (settlement)

1. Pemilik kas bon membuka transaksi yang telah dicairkan.
2. Pemilik melengkapi total penggunaan, keterangan, dan bukti melalui panel pertanggungjawaban yang tersedia.
3. Finance meninjau pertanggungjawaban yang telah diajukan.
4. Cocokkan jumlah bukti, total penggunaan, dan nominal pencairan. Periksa selisihnya.
5. Gunakan tindakan review yang tersedia untuk menerima atau meminta perbaikan/menolak pertanggungjawaban, disertai alasan.
6. Setelah diterima dan diselesaikan sesuai alur, pastikan kas bon berstatus **SETTLED**.

| Kondisi | Tindak lanjut operasional |
| --- | --- |
| Penggunaan lebih kecil daripada pencairan | Verifikasi pengembalian sisa dana sesuai prosedur perusahaan |
| Penggunaan sama dengan pencairan | Pastikan seluruh penggunaan memiliki bukti yang sesuai |
| Penggunaan lebih besar daripada pencairan | Verifikasi selisih dan proses penggantian sesuai kebijakan perusahaan |

Contoh ilustratif: dana dicairkan Rp2.000.000 dan bukti penggunaan sah Rp1.750.000. Sisa Rp250.000 perlu ditindaklanjuti sebagai pengembalian. Catat dan simpan bukti pengembalian sesuai prosedur ITPS.

## 7. Kas kecil (Petty Cash)

Kas kecil digunakan untuk pengeluaran operasional kecil dari dana yang dikelola pemegang kas. Pisahkan pencatatan voucher pengeluaran dari pengajuan isi ulang dana.

### 7.1 Membuat dana kas kecil

1. Buka **Finance → Petty Cash**.
2. Pilih tambah dana jika diizinkan.
3. Isi lokasi/nama dana, custodian, nilai imprest atau target dana, batas saldo minimum, serta saldo awal bila diperlukan.
4. Pastikan saldo awal dan saldo minimum tidak lebih besar daripada nilai imprest.
5. Simpan dan cocokkan saldo aplikasi dengan dana awal yang benar-benar diserahkan.

### 7.2 Mencatat voucher

1. Buka detail dana yang benar, kemudian pilih tambah voucher.
2. Isi nominal, kategori, tanggal transaksi, uraian, Unit Pengaju, akun CoA, dan bukti bila digunakan.
3. Periksa dana dan transaksi sebelum mencatat.
4. Pastikan voucher muncul dengan status **RECORDED**, lalu periksa saldo dana.
5. Jika voucher salah dan tindakan **Void / Batalkan** tersedia, isi alasan pembatalan dan periksa hasilnya. Status voucher menjadi **VOIDED**.

Pada validasi formulir saat penyusunan panduan, nominal voucher harus berupa rupiah bulat yang positif dan **kurang dari Rp1.000.000**; maksimum Rp999.999. Ikuti pesan validasi aplikasi jika ketentuan berubah. Jangan membagi transaksi menjadi beberapa voucher untuk menghindari batas tersebut.

### 7.3 Mengajukan dan mencairkan isi ulang

1. Buka dana kas kecil lalu pilih permintaan **Replenishment / Isi Ulang**.
2. Isi nominal dan dokumen yang diminta. Cocokkan dengan kebutuhan dana serta voucher yang mendasarinya.
3. Finance memeriksa permintaan berstatus **PENDING_FINANCE**, kemudian menyetujui atau menolak.
4. Setelah **APPROVED**, lakukan pembayaran sesuai prosedur dan catat pencairannya melalui tindakan yang tersedia.
5. Pastikan status **DISBURSED** dan periksa saldo dana setelah pencairan.

Alur utama isi ulang: **PENDING_FINANCE → APPROVED → DISBURSED**. Pengajuan yang ditolak menjadi **REJECTED**.

Lakukan pencocokan berkala antara saldo aplikasi, uang fisik, voucher, dan bukti isi ulang. Jika terdapat selisih, telusuri transaksi serta laporkan kepada penanggung jawab sebelum membuat koreksi.

## 8. Kontrak (Contracts)

1. Buka **Finance → Contracts** jika menu tersedia.
2. Pilih kontrak untuk memeriksa klien, nomor kontrak, periode, status, dan nilai MRR yang tercantum.
3. Cocokkan kontrak dengan proyek dan dasar perencanaan keuangan.
4. Jika memiliki kewenangan membuat atau mengubah kontrak, lengkapi formulir sesuai dokumen kontrak yang sah.
5. Jika hanya memiliki akses baca, mintakan perubahan kepada administrator yang berwenang.

**MRR** adalah nilai pendapatan berulang bulanan yang dicatat pada kontrak. Informasi ini tidak membuktikan bahwa invoice telah diterbitkan atau pembayaran klien telah diterima.

## 9. Persetujuan dan pemeriksaan dokumen

### 9.1 Menggunakan kotak Persetujuan

1. Buka **Approvals / Persetujuan**.
2. Buka pengajuan yang memerlukan tindakan Anda.
3. Periksa detail dan lampiran sebelum memutuskan.
4. Gunakan tombol persetujuan yang tersedia, isi komentar atau alasan, lalu konfirmasikan.
5. Pastikan notifikasi berhasil dan status berubah. Jika tampilan belum berubah, muat ulang sebelum mencoba kembali.

Jumlah tahap dan batas nominal dapat berbeda menurut modul serta konfigurasi tenant. Gunakan tahap pada transaksi sebagai acuan; satu persetujuan Finance belum tentu merupakan tahap terakhir.

### 9.2 Daftar periksa sebelum persetujuan

- Tenant, proyek, dan unit sesuai.
- Nominal, tanggal, dan uraian cocok dengan dokumen.
- Akun CoA dan rincian anggaran sesuai tujuan biaya.
- Bukti terbaca, lengkap, dan tidak diajukan ulang pada transaksi lain.
- Selisih pencairan dan pertanggungjawaban telah dijelaskan.
- Tindakan yang dipilih sesuai tahap transaksi dan kewenangan pengguna.

Lampiran umum pada fitur unggah terkait mendukung **JPEG, PNG, WebP, dan PDF**, dengan batas bawaan **10 MB per berkas**. Ikuti petunjuk pada formulir apabila fitur tertentu menerapkan ketentuan tambahan. Jika tautan bukti kedaluwarsa, buka ulang detail transaksi untuk memperoleh tautan baru.

## 10. Rutinitas Finance dan contoh latihan

### Rutinitas harian

1. Periksa kotak Persetujuan dan transaksi yang menunggu Finance.
2. Periksa kas bon yang sudah disetujui tetapi belum dicairkan.
3. Tinjau pertanggungjawaban yang masuk dan tenggat kas bon yang tercantum.
4. Periksa permintaan perubahan anggaran yang telah APPROVED tetapi belum APPLIED.
5. Pantau saldo kas kecil dan permintaan isi ulang.
6. Cocokkan transaksi yang dicatat dengan bukti pembayaran aktual.

### Rutinitas berkala

Bandingkan anggaran dengan realisasi, tindak lanjuti dokumen yang belum lengkap, cocokkan saldo kas kecil dengan uang fisik, dan tinjau kas bon yang belum selesai. Gunakan hasil pemeriksaan sebagai bahan koordinasi dengan PM serta pimpinan.

### Latihan di lingkungan uji

Gunakan data contoh hanya pada lingkungan uji atau proyek latihan yang disetujui administrator.

1. Buat anggaran contoh Rp10.000.000 dengan tiga rincian, lalu periksa jumlahnya.
2. Ajukan anggaran dan amati perubahan tahap persetujuannya menggunakan akun penguji yang sesuai.
3. Buat permintaan transfer Rp500.000 antarrincian. Setelah disetujui dan diterapkan, pastikan total anggaran tidak berubah.
4. Uji kas bon Rp2.000.000 dengan pertanggungjawaban Rp1.750.000 dan identifikasi sisa Rp250.000.
5. Catat voucher kas kecil contoh Rp50.000, lalu periksa pencatatannya dan perubahan saldo.

Hasil yang diharapkan: pengguna dapat membedakan persetujuan, pencairan, penerapan perubahan anggaran, dan penyelesaian pertanggungjawaban.

## 11. Pemecahan masalah

| Masalah | Pemeriksaan dan tindakan |
| --- | --- |
| Menu Finance atau tombol tidak muncul | Periksa akun, tenant, hak akses, penugasan, dan status transaksi bersama administrator |
| Proyek tidak tersedia atau anggaran tidak dapat dibuat | Periksa akses proyek dan statusnya; proyek DRAFT atau dihentikan tidak menerima anggaran baru |
| Unit Pengaju tidak tersedia | Pilih proyek yang benar; pilihan unit dapat dibatasi per proyek. Minta administrator memeriksa master unit dan izin proyek |
| Akun CoA tidak muncul | Periksa apakah akun aktif, dapat digunakan untuk pencatatan, dan termasuk tenant ITPS |
| Permintaan anggaran disetujui tetapi nilai belum berubah | Periksa apakah permintaan sudah APPLIED; lakukan Apply bila berwenang |
| Voucher kas kecil ditolak karena nominal | Periksa batas formulir; gunakan jalur biaya atau kas bon yang tepat sesuai prosedur |
| Berkas gagal diunggah | Periksa format, ukuran, koneksi, dan apakah sesi masih aktif |
| Bukti tidak dapat dibuka | Buka ulang detail transaksi; jika tetap gagal, laporkan kepada administrator |
| Tombol persetujuan tidak tersedia | Transaksi mungkin belum pada tahap Anda, telah diputuskan, atau berada di luar kewenangan akun |
| Terjadi error setelah menyimpan atau saat keluar akun | Catat pesan lengkap dan waktu kejadian. Muat ulang lalu periksa hasil transaksi sebelum mengulang tindakan |

Saat melaporkan kendala, sertakan alamat halaman, nomor atau identitas transaksi, waktu kejadian, langkah yang dilakukan, serta pesan kesalahan. Jangan menyertakan kata sandi atau membagikan dokumen sensitif kepada pihak yang tidak berkepentingan.

## 12. Istilah dan catatan versi

| Istilah | Arti dalam penggunaan sehari-hari |
| --- | --- |
| DRAFT | Data masih berupa draf |
| PENDING | Menunggu tindakan atau persetujuan pada tahap tertentu |
| APPROVED | Seluruh persetujuan untuk proses tersebut telah terpenuhi |
| DISBURSED | Pencairan telah dicatat |
| SETTLED | Pertanggungjawaban kas bon telah diselesaikan |
| APPLIED | Perubahan anggaran telah diterapkan |
| REJECTED | Pengajuan ditolak |
| CANCELLED | Proses dibatalkan; pada anggaran juga digunakan sebagai hasil penolakan |
| CoA | Chart of Accounts atau bagan akun untuk klasifikasi biaya |
| Imprest | Nilai acuan dana kas kecil |
| Custodian | Pemegang atau penanggung jawab dana kas kecil |

Panduan ini menjelaskan penggunaan aplikasi, bukan ketentuan pajak atau kebijakan akuntansi perusahaan. Aturan pencairan, pembayaran, dan pengembalian dana mengikuti prosedur internal ITPS. Dokumen tidak memuat kata sandi dan tidak mengubah data transaksi.

Sumber penyusunan: halaman dan formulir Finance ControlDesk; validasi Budgets, Budget Requests, dan Petty Cash; alur status anggaran dan perubahan anggaran; tindakan kas kecil; konstanta lampiran; serta dokumentasi modul Finance dan hak akses. Implementasi aplikasi diutamakan ketika dokumentasi lama berbeda. Pengaturan tenant dan versi yang terpasang dapat memengaruhi hasil di layar.
