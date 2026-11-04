# Kamus data untuk Bob

Format: JSON UTF-8; versi `pss-bob-data-1.0`; tarikh program ISO `YYYY-MM-DD`; mata wang MYR. Tarikh respons lama mengekalkan masa sumber. Tarikh fail bukan tarikh peristiwa atau pengesahan.

## Struktur utama

| Kunci | Jenis | Maksud |
|---|---|---|
| metadata | objek | Tujuan, tarikh, skop dan had penggunaan |
| tab_1_ringkasan | objek | Medan ringkasan, sorotan dan keutamaan |
| tab_2_kpi_pegawai | senarai objek | Sasaran institusi, snapshot kemajuan dan medan individu/terkini yang belum diketahui |
| tab_3_komuniti_alumni | objek | Statistik baris asal dan calon unik; jangan campurkan unit |
| tab_4_aktiviti_dan_impak | senarai objek | Satu rekod bagi satu acara; banyak sumber boleh menyokong acara sama |
| tab_5_kewangan | objek | Penyata, transaksi, kawalan jumlah laporan dan jadual anggaran |
| tab_6_hala_tuju | senarai objek | Fasa dan cadangan blueprint, status keputusan dan sumber |
| tab_7_penglibatan | objek | Penghantaran baharu kosong, respons minat sejarah dan peluang penglibatan |
| profil_alumni_dalaman | senarai objek | 476 kumpulan identiti sementara, nama dan jejak baris sumber |
| rekod_penglibatan_program_dalaman | senarai objek | Nama alumni dalam sumber acara dan beberapa tahun tamat; liputan separa |
| rujukan_jawatankuasa_sejarah | senarai objek | Jawatankuasa menurut slaid lama; bukan pengesahan lantikan semasa |
| rujukan_proses_kerja | senarai objek | Lima proses kerja daripada dokumen pegawai |
| rujukan_daftar_surat | senarai objek | Empat rekod surat; bukan transaksi kewangan |
| isu_perlu_pengesahan | senarai objek | Konflik, kekurangan dan tindakan susulan |
| sumber | senarai objek | ID, lokasi/URL, hash fail dan keadaan bacaan |

## Medan dan peraturan penting

`id` ialah kunci stabil dalam pakej. `program_id` merujuk acara dalam Tab 4. `alumni_id` merujuk profil dalaman apabila padanan nama tepat dan tunggal tersedia; null bermakna belum dipadankan, bukan tiada alumni. `sumber_ids` merujuk satu atau lebih entri daftar sumber. `baris_sumber` menggunakan nombor baris Excel 1-based termasuk baris pengepala.

`null`: nilai tidak diketahui / belum disahkan. `0`: nilai sifar yang dinyatakan sumber, contohnya perbelanjaan Tiada. `false`: jawapan TIDAK atau status negatif yang jelas; bukan ganti nilai yang hilang. Angka wang ialah nombor perpuluhan, bukan teks bertanda RM.

`bil_alumni_dilapor`: bilangan yang dilapor untuk satu acara; belum semestinya senarai unik yang telah diaudit. `alumni_unik_disahkan`: dibiarkan null jika tiada pengesahan. Jangan jumlahkan bilangan peserta beberapa acara untuk menghasilkan alumni unik tahunan.

`perbelanjaan_dilapor_rm` dalam program ialah jumlah kawalan laporan. Butiran transaksi mengandungi pecahan jumlah itu. **Jangan jumlahkan jumlah program dan butiran transaksi sekali lagi.** `amaun_dimohon_rm` bukan bajet diluluskan. `amaun_diluluskan_rm` bukan pembayaran. `amaun_dibayar_disahkan_rm` hanya diisi selepas semakan bukti; semuanya belum diisi dalam pakej ini.

`anggaran_program` ialah jadual permohonan, tidak termasuk dalam jumlah transaksi dibayar. Anggaran RM8,160 dan permohonan RM8,160 merujuk acara sama; tidak boleh dianggap dua pengeluaran.

`peratus_dikira` disimpan dalam skala 0–100. `pecahan_pencapaian_sumber` disimpan dalam skala 0–1, misalnya 0.4. Pencapaian 2/5 ialah snapshot versi sumber, bukan jumlah program yang disahkan oleh pakej.

`status_bekerja_dilapor`, `jawatan_dilapor` dan maklumat minat ialah sejarah sumber. Tiada kadar kebolehpasaran rasmi dikira. Sesi batch/latihan industri tidak ditukar kepada tahun graduasi. Negeri dan bidang pekerjaan tidak diteka daripada alamat atau jawatan.

## Kaedah padanan sementara alumni

Dalam analisis dalaman, digit nombor pengenalan dinormalkan dan dipenuhkan sifar di hadapan sehingga 12 aksara untuk memadankan salinan nombor yang kehilangan sifar. Nombor itu tidak dieksport. Hasilnya 476 kumpulan daripada 547 baris dan 278 kumpulan daripada 314 respons; semua kumpulan borang bertindih dengan data utama. Kaedah ini belum membuktikan identiti atau keahlian.

Nilai sel fail data di akar OneDrive dan salinan backup adalah sama walaupun hash fail berbeza. Kedua-duanya tidak dijumlahkan. Untuk profil berborang, respons dengan timestamp terakhir menjadi nilai profil pilihan. Semua 314 respons minat dikekalkan dengan jejak sumber supaya sejarah dan konflik tidak hilang. Taburan program mengandungi versi baris asal dan versi kumpulan sementara untuk perbandingan.

## Peraturan migrasi

Semak eksport/sandaran asli aplikasi dahulu. Buat sandaran sebelum import; padankan ID dan semak calon pendua berdasarkan acara/tarikh/sumber jika aplikasi sudah mempunyai data. Nilai `null` tidak boleh menimpa nilai sah sedia ada secara automatik. Import berulang fail sama mesti tidak menggandakan rekod. Sediakan ringkasan perubahan dan konflik untuk pegawai selepas pemetaan.
