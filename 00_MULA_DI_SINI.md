# Pakej data Dashboard Alumni PSS untuk Bob

Disediakan pada **4 November 2026**, untuk Akmal Hazreen Fizree bin Jamaludin, Pegawai Alumni Politeknik Sandakan Sabah.

**Berikan keseluruhan ZIP kepada Bob.** Fail utama ialah `DATA_UTAMA_BOB.json`. Data disusun mengikut tujuh tab dashboard dalam gambar yang dibekalkan. `PEMETAAN_7_TAB.json` menerangkan cara memadankan setiap tab.

## Apa yang ada

| Kandungan | Bilangan / keterangan |
|---|---|
| Data utama alumni | 547 baris asal; 476 kumpulan identiti calon selepas padanan sementara |
| Borang keahlian 2023 | 314 respons; 278 kumpulan identiti calon, bertindih dengan data utama |
| Minat aktif | 171 respons YA; 152 calon unik berdasarkan respons terakhir |
| Minat talk/seminar | 134 respons YA; 118 calon unik berdasarkan respons terakhir |
| Program / aktiviti | 18 rekod, merangkumi 2022–2026; pelaksanaan tidak semuanya disahkan |
| Kewangan | 17 butiran; laporan, permohonan dan anggaran dipisahkan |
| Blueprint | 16 cadangan / fasa; tiada kelulusan diandaikan |
| Sumber | 122 entri: fail komputer, Google Drive dan 7 imej dashboard |
| Isu pengesahan | 14 isu bersama tindakan susulan |

547, 314, 476 dan 278 mempunyai maksud berlainan. **Jangan jumlahkan data utama dengan respons borang. Jangan labelkan mana-mana angka itu sebagai ahli berdaftar rasmi sebelum semakan.**

## Penemuan penting untuk Tab KPI

Pelan Tindakan PSS **2026** menyatakan sasaran **5 program/aktiviti melibatkan alumni PSS**, dengan PIC **Pegawai Alumni**. Fail pemantauan versi diubah 5 Ogos 2026 merekodkan **2 / 5 = 40%**.

Ini rujukan sasaran institusi 2026, bukan bukti sasaran SKT/SKU individu telah diluluskan. Angka 40% ialah snapshot dalam sumber, bukan pengesahan pencapaian terkini hingga November. Bukti dan senarai program perlu dipadankan sebelum kemajuan dikemas kini. Nota dashboard lama yang hanya menyebut sasaran sejarah 2025 perlu disemak berdasarkan penemuan ini.

## Arahan penyerahan kepada Bob

1. Baca fail utama, pemetaan dan kamus data sebelum mengubah dashboard.
2. Simpan sandaran data sedia ada. Periksa kod atau contoh eksport CSV/sandaran asli untuk mengetahui nama medan sebenar.
3. Padankan tujuh bahagian JSON ke tujuh tab. Gunakan ID yang disediakan untuk mengelakkan acara atau transaksi berulang.
4. Kekalkan nilai tidak diketahui sebagai `null` dan paparkan **Belum disahkan**. Jangan tukar nilai kosong kepada sifar.
5. Kekalkan sasaran institusi, sasaran individu, snapshot kemajuan dan pencapaian terkini sebagai medan berasingan.
6. Rekod jemputan, tentatif, anggaran dan cadangan tidak boleh automatik dianggap pelaksanaan, bayaran atau kelulusan.
7. Untuk kewangan, `amaun_dilapor_rm` bukan `amaun_dibayar_disahkan_rm`. Baki dana belum dapat ditentukan. Butiran anggaran pra-konvo RM8,160 bukan pembayaran sebenar.
8. Untuk komuniti, paparan Ahli hanya menerima agregat. Profil bernama dan respons minat sejarah untuk pegawai/pentadbir sahaja.
9. Untuk Tab Penglibatan, `penghantaran_baharu` memang kosong. Respons borang 2023 ialah senarai susulan sejarah, bukan penghantaran baharu, permohonan AJK atau pelantikan.
10. Semak `ISU_DAN_PENGESAHAN.json` dan dapatkan pengesahan pegawai bagi nilai bercanggah sebelum menandakan rekod disahkan.

## Keserasian import

Pakej ini **bukan fail Sandaran/Pulih asli dashboard**. Hanya gambar dashboard tersedia; kod, nama medan CSV dan struktur localStorage belum diketahui. Bob perlu memetakan data atau membina penukar import dahulu. Jangan terus menggunakan butang Pulih untuk fail ini.

Untuk paparan pegawai, data bernama perlu kawalan akses sebenar. Menukar dropdown peranan dalam pelayar sahaja tidak melindungi fail yang sudah dihantar kepada pengguna Ahli. Jika dashboard dikongsi sebagai fail statik, gunakan agregat sahaja dalam muatan Ahli.

## Ketepatan dan liputan

Sumber diperiksa dalam folder kerja Pegawai Alumni CISEC, data utama di akar OneDrive dan carian/folder Google Drive berkaitan alumni serta Pelan Tindakan PSS 2026. Ini bukan audit keseluruhan komputer atau keseluruhan Google Drive. Fail institusi lain tidak dimasukkan sebagai pencapaian PSS. Salinan dengan hash sama dikenal pasti; fail acara yang berlainan format digabungkan secara manual mengikut acara, bukan dijumlahkan sebagai program tambahan.

106 fail tempatan melalui proses bacaan teks/sel; tidak semua kandungan telah disahkan secara visual atau ditranskripsikan menjadi data berstruktur. Fail yang berupa imbasan / teks sangat terhad ditandakan dalam daftar sumber. Resit, tandatangan dan penyata bank belum direkonsiliasi. Daftar sumber ialah jejak rujukan, bukannya bukti semua 122 entri telah diaudit atau diluluskan.

Maklumat IC, telefon, e-mel peribadi, alamat penuh, akaun bank, gaji, tandatangan dan pautan gambar pasport tidak disertakan. Nama, program pengajian dan maklumat kerjaya terhad disertakan untuk kegunaan dalaman. ID pakej ialah ID baharu; bukan nombor IC atau nombor pelajar.

Tarikh penyediaan fail tidak bermaksud data alumni, jawatankuasa, kewangan atau pencapaian semuanya terkini pada tarikh itu. Semua sumber asal dikekalkan tanpa perubahan.
