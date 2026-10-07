# Riset konsep — situs ulang tahun Liya

Tanggal riset: 8 Oktober 2026

## Arah pengalaman

Saya membandingkan bentuk kartu ucapan statis, halaman cerita panjang, dan scrapbook digital personal. Untuk hadiah yang akan dibuka lewat tautan—kemungkinan besar di ponsel—scrapbook satu halaman memberi rasa seperti membuka kartu fisik, sambil tetap membuat ucapan mudah dibaca dan dibagikan. Contoh situs ulang tahun yang diceritakan Nabiu Studio juga memakai pendekatan scrapbook/kolase digital untuk membuat situs terasa seperti hadiah personal: https://nabiu.studio/garden/websites-for-you-and-your-loved-ones

## Keputusan desain

- Cerita dalam urutan sederhana: kartu pembuka → empat harapan → surat dalam amplop → lilin → salam penutup. Pengunjung bisa mengikuti alur dengan scroll biasa dan berhenti kapan saja.
- Rasa scrapbook tanpa foto palsu: tekstur kertas, label tanggal, warna pastel, kartu miring, amplop, dan ilustrasi kue CSS memberi kesan buatan tangan. Tidak memasukkan foto atau kenangan spesifik yang belum diberikan.
- Interaksi kecil dan punya tujuan: surat dibuka dengan tombol, lilin bisa ditiup, lalu konfeti merayakan tindakan. Tidak ada musik autoplay agar kartu tetap sopan ketika dibuka di tempat umum.
- Tetap nyaman di ponsel: satu halaman statis tanpa paket besar; grid berubah menjadi kolom di layar sempit. Panduan responsive web.dev menyarankan layout fleksibel, zoom tetap diizinkan, dan target sentuh cukup besar: https://web.dev/articles/accessible-responsive-design?hl=en
- Gerakan dapat dikurangi: animasi kue dan konfeti menghormati pengaturan sistem prefers-reduced-motion, mengikuti teknik yang didokumentasikan W3C: https://www.w3.org/WAI/WCAG22/Understanding/animation-from-interactions/
- Ringan dan cepat dibuka: ilustrasi dibuat dengan CSS, tanpa pustaka animasi dan tanpa foto berat. Jika foto ditambahkan kelak, web.dev menyarankan ukuran gambar responsif dan optimasi byte: https://web.dev/articles/responsive-images

## Hosting

Situs HTML/CSS/JS statis sesuai GitHub Pages. GitHub mendukung publikasi dari workflow Actions dan merekomendasikan workflow kustom bila perlu kendali alur publikasi: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

## Batas personalisasi

Nama dan tanggal sudah dipasang. Teks surat sengaja berisi doa universal, bukan klaim hubungan atau memori tertentu, karena konteks personal tambahan belum diberikan. Semua teks dapat diedit langsung di index.html.
