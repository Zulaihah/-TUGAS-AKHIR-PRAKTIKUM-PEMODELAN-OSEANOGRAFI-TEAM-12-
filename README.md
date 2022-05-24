# TUGAS AKHIR PRAKTIKUM PEMODELAN OSEANOGRAFI TEAM 12 
Repositori ini dibuat untuk memenuhi tugas akhir kelompok praktikum pemodelan oseanografi tahun 2022. Harapan kami semoga repositori ini dapat bermanfaat bagi kita semua.
# NAMA ANGGOTA TEAM 12
1. Afiq Mahasin 26050120130084 A
2. Galung Dhiva Maharani 26050120120010 A
3. Moses Wicaksono Kurniawan 26050120120005 A
4. Maldiva Hafiza Anjarika Suhendar
5. Siti Zulaihah 26050120130061 A
6. Vany Siregar 26050120120013 A
# PENDAHULUAN
Fenomena aliran dan transportasi adalah fenomena alam yang penting untuk dipelajari, karena mempengaruhi beberapa studi teknik. Fenomena ini terjadi dalam berbagai  situasi fisik, termasuk: perpindahan panas, proses pemisahan  kimia, aliran fluida dalam media berpori, dispersi pengotor dalam cairan, dan pengangkutan partikel kecil tersebut, dispersi polutan, garam, sedimen, dan lain- lain di  perairan dangkal. Beberapa pendekatan  skema beda hingga yang umum digunakan untuk menyelesaikan transportasi aliran fluida adalah skema beda hingga eksplisit (FTCS, Dufort Frankel, Leapfrog, dll) dan skema-skema beda hingga implisit yang dapat dibagi menjadi dua bagian (BTCS, Richardson, CrankNicolson , ADI). Persamaan adveksi difusi adalah persamaan diferensial parsial yang menggambarkan suatu masalah dengan fenomena transportasi kontaminan aliran air tanah,  sering disebut sebagai transportasi massal atau transportasi zat terlarut. Ada dua proses dasar yang bermasalah ketika mengangkut polutan di aliran air: difusi dan adveksi.

Matematika merupakan alat yang menarik untuk memodelkan fenomena  alam, karena matematika merancang fenomena alam dalam bentuk struktur matematika. Persamaan  lain yang memodelkan fenomena  alam adalah persamaan  yang sering disebut persamaan konveksi-difusi atau persamaan transpor. Persamaan konveksi-difusi adalah rumus yang digunakan untuk mempelajari fenomena transportasi polutan. Persamaan transpor merupakan salah satu persamaan diferensial yang menggambarkan sirkulasi aliran air di suatu muara dengan besaran C (konsentrasi garam) sebagai fungsi ruang dan waktu. Pemodelan matematika sering menemukan persamaan diferensial kompleks yang perlu diselesaikan secara analitik. Namun, solusi dari persamaan diferensial ini tidak hanya analitik, tetapi juga  numerik. Solusi numerik adalah metode untuk merumuskan masalah matematika  sehingga mereka dapat diselesaikan dengan operasi aritmatika dan operasi logika. Dengan perkembangan komputer dengan waktu komputasi yang  cepat,  pemodelan matematika menjadi lebih umum dengan penerapan metode numerik yang memfasilitasi penyelesaian persamaan matematika dalam  model matematika yang  dibuat. Teknik numerik kadang-kadang disebut sebagai matematika komputasi karena komputer digital pandai melakukan operasi tersebut.

ADVEKSI-DIFUSI 1D
Persamaan adveksi 1 dimensi yang digunakan :
df/dt= -U df/dx
Persamaan difusi 1 dimensi yang digunakan :
df/dt = Ad d**2f/dx
Persamaan adveksi - difusi 1 dimensi yang digunakan :
df/dt = -U df/dx + Ad d**2f/dx
Dimana f menggambarkan konsentrasi suatu zat terlarut, U adalah koefisien adveksi, dan Ad adalah koefisien difusi, dan x adalah arah sumbu horisontal.

# Modul 1 : Persamaan Adveksi - Difusi 1D
Penerapan Adveksi-Difusi 1D di dalam bidang Oseaografi :
- Mengetahui konsentrasi dan penyebaran polutan di sungai, parit, dan cabang sungai
- Pemodelan polutan
- Konservasi lingkungan
# Modul 2 : Persamaan Adveksi - Difusi 2D
Adveksi - Difusi 2D merupakan metode eksplisit dimana persamaan beda hingga dengan metode ini menggunakan pendekatan beda maju untuk turunan waktu, sedangkan untuk turunan terhadap ruang dilakukan dengan melihat arah kecepatan u. Jika u > 0 maka turunan terhadap ruang menggunakanpendekatan beda mundur, sebaliknya jika u < 0 digunakan pendekatan beda maju. Persamaan adveksi difusi-2D digunakan untuk memodelkan pergerakan polutan di laut.Persamaan pembangun yang berhubungan dengan transportasi konsentrasi polutan berupa persamaan Difusi 2D yakni 
![image](https://user-images.githubusercontent.com/78490254/169945155-12fcf280-d912-42c3-82e3-6df12c6b44da.png)
dimana 𝐶 menyatakan konsentrasi polutan yang terangkut dalam arah sumbu 𝑥 dan 𝑦. Konstanta 𝑉𝑥 dan 𝑉𝑦 disini menyatakan kecepatan aliran yang searah sumbu 𝑥 dan 𝑦 berturut turut. Juga 𝐷𝑥 dan 𝐷𝑦 juga merupakan konstanta yang menyatakan koefisien difusi yang searah sumbu 𝑥 dan sumbu 𝑦 berturut turut. Adapun syarat awal dan syarat batas yang menyertai persamaan pembangun akan dimulai dari domain yang teratur sebagai verifikasi solusi numerik, hingga ke domain yang tidak teratur,dan persamaan diskritisasi untuk model adveksi difusi 2D adalah sebagai berikut:
![image](https://user-images.githubusercontent.com/78490254/169945433-59a4eae5-71df-4a11-b1e8-fc93e0b8c75e.png)

Salah satu script pada Adveksi-Difusi 2D sebagai berikut : 
Untitled3.ipynb

Penerapan Persamaan Persamaan Adveksi - Difusi 2D di dalam bidang oseanografi :
- Menghitung dan memodelkan persebaran nutrien di laut atau sungai 
- Menghitung dan memodelkan penyebaran polutan dari proses industri
- Mengetahui persebaran polutan dari laguna dengan menghitung input dan outputnya
- Mengetahui sebaran kebocoran minyak di laut
# Modul 3 : Persamaan Hidrodinamika 1D
Penerapan Persamaan Hidrodinamika 1D di dalam bidang Oseaografi :
- Mengetahui sebaran tumpahan minyak mentah yang ada di perairan menggunakan data arah pergerakan arus pasang surut
- Untuk mengkaji fenomena suhu dingin di perairan 
- Mengetahui sebaran limbah air panas yang masuk ke perairan
# Modul 4 : Persamaan Hidrodinamika 2D
Penerapan Persamaan Hidrodinamika 2D di dalam bidang Oseaografi :
- Pemodelan gelombang karena angin
- Pemodelan sampah plastik di laut
- Pemodelan coastal dynamics dan sedimentasi pantai
