# Program dan data yang tersedia

Status mengikut kekuatan sumber; semua pengesahan akhir kekal untuk pegawai. Jemputan/tentatif tidak dikira automatik sebagai pelaksanaan.

| ID | Program | Tarikh | Status | Belanja dilapor RM |
|---|---|---|---|---|
| PRG-2022-01 | Program Hari Kerjaya | 2022-06-08 | Dilaksanakan menurut laporan | Belum diketahui |
| PRG-2022-02 | Program Selangkah ke Alam Kerjaya | 2022-06-17 hingga 2022-06-18 | Dilaksanakan menurut laporan | Belum diketahui |
| PRG-2023-01 | Pertandingan Futsal Sesi 1 2023/2024 | 2023-11-25 hingga 2023-11-26 | Dilaksanakan menurut laporan | 0.00 |
| PRG-2023-02 | Mesyuarat Agung Persatuan Alumni PSS Tahun 2023 | 2023-12-02 | Dilaksanakan menurut laporan | 0.00 |
| PRG-2024-01 | Majlis Dialog Bersama Industri dan Alumni Road to POLYCC | 2024-01-14 | Dilaksanakan menurut laporan | 500.00 |
| PRG-2024-02 | PSS Alumni Road Tour 2024 | 2024-05-15 hingga 2024-05-16 | Dilaksanakan menurut laporan | 9,000.40 |
| PRG-2024-03 | Slot Alumni Minggu Suai Kenal Sesi 1 2024/2025 | 2024-07-31 | Dilaksanakan menurut laporan | 0.00 |
| PRG-2024-04 | Bicara Alumni dan Sukan Bersama Alumni 2024 | 2024-11-05 hingga 2024-11-06 | Dilaksanakan menurut laporan | 641.00 |
| PRG-2025-01 | Slot Perkongsian Alumni MSK Sesi II 2024/2025 | 2025-01-08 | Jemputan / bahan tersedia; pelaksanaan belum disahkan | Belum diketahui |
| PRG-2025-02 | Slot Perkongsian Alumni MTS Sesi I 2025/2026 | 2025-07-30 | Jemputan dan tentatif tersedia; pelaksanaan belum disahkan | Belum diketahui |
| PRG-2025-03 | Jamuan Makan Malam Pra Konvokesyen PSS | 2025-09-13 | Disebut dalam permohonan; perlu laporan pelaksanaan | Belum diketahui |
| PRG-2025-04 | Bicara Alumni: Jalan Dua Haluan | 2025-11-19 | Dilaksanakan menurut laporan | Belum diketahui |
| PRG-2025-05 | Retreat Kompas Alumni 2026: Satu Team, Satu Hala | 2025-12-17 | Jemputan; bukti pelaksanaan perlu pengesahan | Belum diketahui |
| PRG-2026-01 | Slot Perkongsian Alumni MTS Sesi II 2025/2026 | 2026-01-08 | Jemputan dan sijil penghargaan tersedia; pengesahan akhir diperlukan | Belum diketahui |
| PRG-2026-02 | Focus Group Dialogue Sempena Hari Kerjaya dan Kolaborasi Strategik Industri 2026 | 2026-04-02 | Dilaksanakan menurut laporan | Belum diketahui |
| PRG-2026-03 | Perjumpaan Persatuan Alumni Bersama Pengarah | 2026-05-06 | Panggilan perjumpaan; minit / kehadiran belum disahkan | Belum diketahui |
| PRG-2026-04 | Bengkel Pengurusan Alumni | 2026-05-12 | Jemputan; pelaksanaan belum disahkan | Belum diketahui |
| PRG-2026-05 | Inspirasi Alumni: Dari Kampus Menuju Impian | 2026-08-19 | Jemputan; pelaksanaan belum disahkan | Belum diketahui |

## Isu yang perlu disahkan

**DQ01 — Komuniti Alumni**

547 baris data utama mempunyai pendua; 476 kumpulan diperoleh dengan menormalkan digit ID dalaman kepada 12 aksara. Ini padanan sementara, bukan pengesahan ahli.

Tindakan: Semak identiti asal dan sahkan keahlian. Jangan campur 547 + 314 atau paparkan 476 sebagai ahli rasmi.

Sumber: LROOT, L001, L023

**DQ02 — Komuniti Alumni**

Nombor pengenalan dalam Excel kehilangan sifar di hadapan; panjang asal 8–12 digit. Tiada ID asal, nombor telefon, e-mel, akaun bank, alamat penuh atau gaji dieksport dalam pakej ini.

Tindakan: Rujuk fail asal dengan akses pegawai untuk pengesahan. Jangan minta Bob meneka identiti/tahun tamat.

Sumber: LROOT, L023

**DQ03 — Penglibatan**

314 respons termasuk respons berulang; angka 171 dan 134 ialah bilangan respons YA, bukan orang unik.

Tindakan: Gunakan angka calon unik daripada respons terkini untuk senarai hubungi semula; jangan cipta pelantikan atau borang baharu.

Sumber: L023

**DQ04 — KPI Pegawai**

Pelan Tindakan 2026 menyatakan sasaran 5 dan fail pemantauan menyatakan 2 (40%), tetapi tarikh kemajuan sebenar dan kelulusan individu tidak dinyatakan.

Tindakan: Kemas kini nota Tab 2: sasaran institusi 2026 ditemui; sahkan sasaran individu secara berasingan. Jangan guna 40% sebagai kemajuan hingga 4 November tanpa semakan.

Sumber: GD_1aO_DkP5CU0Ui3hQRN0SucZ2ml7bUPP0L, GD_1EjxN0IqRO6MFceecoQ41ps2d903fUjXe

**DQ05 — Aktiviti & Impak**

Bicara/Sukan 2024: bilangan peserta, kluster dan senarai alumni berlainan antara slaid dan laporan.

Tindakan: Sahkan versi muktamad; nilai peserta gabungan dibiarkan null.

Sumber: L030, L043, L044

**DQ06 — Aktiviti & Impak**

Road Tour 2024: konflik tarikh pada muka depan/tentatif dan bahagian tarikh.

Tindakan: Sahkan 15–16 Mei 2024; simpan varian 14–16 Mei 2023 sebagai isu, jangan cipta acara kedua.

Sumber: L027, L028

**DQ07 — Kewangan**

Baki awal, penerimaan, baki akhir dan komitmen belum dibayar tidak boleh dipastikan daripada laporan program / permohonan.

Tindakan: Isi null; padankan resit, kelulusan, penyata dan pengesahan bendahari sebelum mengira baki.

Sumber: L003, L027, L043

**DQ08 — Hala Tuju**

Blueprint mengandungi ayat resolusi, yuran dan KPI sasaran yang boleh disalah baca sebagai keputusan telah diluluskan.

Tindakan: Semua kekal cadangan; jangan set status diluluskan, akaun aktif, dana diterima atau kemajuan 100% tanpa minit.

Sumber: L006, L009, L014

**DQ09 — Komuniti Alumni**

Senarai jawatankuasa mempunyai tempoh 2024–2026 dalam slaid dan 2024–2027 dalam dokumen.

Tindakan: Sahkan tempoh serta lantikan terkini; jangan gunakan senarai sejarah sebagai pentadbir semasa.

Sumber: L019, L025

**DQ10 — Aktiviti & Impak**

Permohonan pra-konvo bertarikh sebelum acara tetapi menyatakan wang telah digunakan.

Tindakan: Sahkan tarikh surat, program, kelulusan dan bayaran.

Sumber: L003

**DQ11 — Ringkasan**

Fail paparan dashboard dan format eksport/sandaran sebenar belum tersedia; hanya tujuh imej rujukan.

Tindakan: Bob perlu padankan skema aplikasi dahulu; jangan terus pulih atau tindih localStorage. Pakej ini bukan sandaran asli dashboard.

Sumber: UI-01, UI-02, UI-03, UI-04, UI-05, UI-06, UI-07

**DQ12 — Komuniti Alumni**

Data asas dan minat bertarikh lama; tahun tamat, negeri dan bidang pekerjaan tidak cukup untuk menghasilkan carta sebenar.

Tindakan: Padam carta demo dan paparkan Data belum tersedia; kemas kini profil sebelum analisis semasa.

Sumber: LROOT, L023

**DQ13 — Aktiviti & Impak**

Bengkel Pengurusan Alumni menyatakan 12 Mei 2026 (Rabu); tarikh itu jatuh pada Selasa.

Tindakan: Sahkan tarikh / hari program dan laporan pelaksanaan.

Sumber: L057, L058

**DQ14 — Sumber**

Sebahagian PDF berbentuk imbasan tanpa teks yang boleh diekstrak; dokumen dalam folder sudah sign tidak membuktikan tandatangan diperiksa.

Tindakan: Semak visual / OCR dokumen yang ditandakan dalam daftar sumber sebelum menaik taraf status kepada disahkan.

Sumber: L017, L048, L060, L063, L074, L075, L078
