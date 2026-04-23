plugin ini dirancang untuk meningkatkan aksesibilitas website melalui vitur visual,navigasi,audio.
Plugin ini bersifat:

🔌 Plug & Play
🌐 CDN-ready
⚙️ Modular (bundle terpisah)
🧩 Framework-agnostic (bisa dipakai di HTML, Laravel, dll)
instalation:
1.menggunakan cdn production:
<script src= "https://cdn.jsdelivr.net/gh/VCTryo0304/pluginaksesibilitas@1.0.1/accesibility.js" defer></script>
2. Menggunakan Local File (Development):
<script src="accesibility.js" defer></script>
semua file berada dalam satu folder:
pluginaksesibilitas/
  accesibility.js
  tampilan.bundle.js
  teks.bundle.js
  aksesibilitas.css
  
  Plugin bekerja dengan alur:

Load accesibility.js
Auto-detect BASE path
Load CSS (aksesibilitas.css)
Load bundle:
tampilan.bundle.js
teks.bundle.js
Jalankan init()
Inject panel aksesibilitas ke DOM
Visual Accessibility
Fitur	Deskripsi
Hide Images	Menyembunyikan gambar
High Contrast	Mode kontras tinggi
Reduce Motion	Nonaktifkan animasi
Monochrome	Grayscale mode
Big Cursor	Cursor besar
🔊 Audio & Voice
Fitur	Deskripsi
Text-to-Speech	Membacakan isi halaman
Voice Command	Kontrol dengan suara

Contoh perintah:

“scroll bawah”
“scroll atas”
“baca”
“stop”
🔍 Zoom & Magnifier
Fitur	Deskripsi
Zoom In/Out	Perbesar tampilan
Magnifier	Kaca pembesar cursor
Plugin expose fungsi ke global scope:

window.APR_IMAGES
window.APR_CONTRAST
window.APR_ANIMATION
window.APR_MONO
window.APR_CURSOR
window.APR_TTS
window.APR_VOICE
window.APR_ZOOM
window.APR_MAGNIFIER
Contoh penggunaan:
APR_CONTRAST.toggle();
APR_TTS.start();
APR_ZOOM.in();
APR_MAGNIFIER.toggle();
