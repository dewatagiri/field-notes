# LinkedIn post (BM first, EN second)

Article: https://dewatagiri.github.io/field-notes/job-linked-bridge-engine/
Code (MIT): https://github.com/dewatagiri/self_employed_bridge
Previous post: https://www.linkedin.com/feed/update/urn:li:activity:7529550240052523008/

---

## BM

Dalam artikel sebelum ini, saya tulis peraturan pinjaman jambatan untuk tukang: bayar kedai bahan terus, bukan tukang. Siaran itu di sini: https://www.linkedin.com/feed/update/urn:li:activity:7529550240052523008/

Kali ini saya jadikan semua peraturan itu sebuah enjin yang berjalan. Kalau peraturan dah ditulis, kenapa kita masih kira dengan tangan? Ini cara enjin itu berfikir, daripada satu kerja tukang cat sehingga keputusan simulasi:

1. Empat soalan: ada kerja sah? bahan jadi kos utama? pembayar layak? deposit kurang daripada kos bahan?
2. Semakan: identiti, saringan jenayah kewangan, rekod kredit, kedai dalam senarai.
3. Berapa: kos bahan RM5,000 tolak deposit RM2,000 = RM3,000, tertakluk pada had.
4. Bayar terus kepada kedai. Kerja besar atau tak sepadan pergi kepada pegawai.
5. Apa jadi kemudian: bayar tepat masa, lewat, bayar tunai kepada tukang, pertikaian, atau tinggal kerja. Setiap satu ada kebarangkalian dan kadar kutipan balik.
6. Kerugian = pinjaman × (1 tolak kadar kutipan balik). Ia ditanggung ikut giliran: rizab penaja, penjamin, pembiaya.
7. Ulang satu kumpulan pinjaman 1,000 kali. Itulah simulasi.

Hasilnya (angka rekaan):
* Rizab habis dalam 36% kumpulan.
* Kalau kadar kutipan balik jatuh suku (25% daripada kadar asal), untung RM25 bagi setiap pinjaman jadi rugi RM22.
* Yuran yang betul-betul cukup tampung kos dan jangkaan kerugian ialah kira-kira RM35, bukan RM60 yang saya reka.

Tentang enjin ini: 15 bahagian kod Python, 141 ujian automatik, 12 keputusan yang saya buat dan direkodkan. Saya tetapkan peraturan dan buat keputusan, AI tulis kod dan ujian, dan ujian itu yang buktikan. Bukan "minta AI buat aplikasi".

Kod terbuka (MIT): https://github.com/dewatagiri/self_employed_bridge

PERHATIAN: semua angka RM di atas ialah angka rekaan untuk ujian, bukan anggaran daripada data sebenar. Data kerugian sebenar di Malaysia belum ada.

Penjelasan penuh langkah demi langkah (BM dan EN): https://dewatagiri.github.io/field-notes/job-linked-bridge-engine/

Kalau anda ada proses kerja yang peraturannya dah ditulis tapi masih dikira dengan tangan, yang mana satu patut jadi enjin dahulu?

(Penafian: Ini adalah pandangan peribadi saya dan tidak mewakili mana-mana organisasi yang pernah atau sedang saya sertai.)

#AutomasiAI #Fintech #PMKS #PembiayaanMikro #Python #EkonomiMalaysia

---

## EN

In my last post I set out the rules of a bridge loan for tradespeople: pay the materials shop directly, not the painter. That post: https://www.linkedin.com/feed/update/urn:li:activity:7529550240052523008/

This time I turned all those rules into a working engine. If the rules are already written down, why are we still working them out by hand? Here is how the engine thinks, from one painter's job to the simulation result:

1. Four questions: a real job? is the main cost materials? is the payer eligible? is the deposit below the materials cost?
2. Checks: identity, financial-crime screening, credit record, shop on the list.
3. How much: materials RM5,000 minus deposit RM2,000 = RM3,000, within limits.
4. Pay the shop directly. A large or unusual job goes to an officer.
5. What happens next: pays on time, pays late, pays the painter in cash, a dispute, or the painter walks away. Each has a chance and a recovery rate.
6. Loss = loan x (1 minus recovery rate). It is taken in order: sponsor's reserve, guarantor, lender.
7. Repeat one group of loans 1,000 times. That is the simulation.

The result (made-up numbers):
* The reserve ran out in 36% of groups.
* If the recovery rate falls by a quarter of its starting value, a RM25 profit per loan becomes a RM22 loss.
* A fee that just covers costs and expected loss is about RM35, not the RM60 I made up.

About the engine: 15 parts in Python, 141 automatic tests, 12 decisions I made and recorded. I set the rules and made the decisions, AI wrote the code and the tests, and the tests proved it. I did not just ask AI to build an app.

Open code (MIT): https://github.com/dewatagiri/self_employed_bridge

WARNING: every RM figure above is made up for testing, not estimated from real data. No real Malaysian loss data exists yet.

The full step-by-step walkthrough (BM and EN): https://dewatagiri.github.io/field-notes/job-linked-bridge-engine/

If you have a work process whose rules are already written but still worked out by hand, which one should become an engine first?

Views are my own and do not represent any organisation I am or have been associated with.

#AIAutomation #Fintech #MSME #Microfinance #Python #Malaysia
