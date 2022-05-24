# TUGAS AKHIR PRAKTIKUM PEMODELAN OSEANOGRAFI TEAM 12 ☘
Repositori ini dibuat untuk memenuhi tugas akhir kelompok praktikum pemodelan oseanografi tahun 2022. Harapan kami semoga repositori ini dapat bermanfaat bagi kita semua.
# NAMA ANGGOTA TEAM 12
1. Afiq Mahasin 26050120130084 A
2. Galung Dhiva Maharani 26050120120010 A
3. Moses Wicaksono Kurniawan 26050120120005 A
4. Maldiva Hafiza Anjarika Suhendar
5. Siti Zulaihah 26050120130061 A
6. Vany Siregar 26050120120013 A
# 1. PENDAHULUAN
Fenomena aliran dan transportasi adalah fenomena alam yang penting untuk dipelajari, karena mempengaruhi beberapa studi teknik. Fenomena ini terjadi dalam berbagai  situasi fisik, termasuk: perpindahan panas, proses pemisahan  kimia, aliran fluida dalam media berpori, dispersi pengotor dalam cairan, dan pengangkutan partikel kecil tersebut, dispersi polutan, garam, sedimen, dan lain- lain di  perairan dangkal. Beberapa pendekatan  skema beda hingga yang umum digunakan untuk menyelesaikan transportasi aliran fluida adalah skema beda hingga eksplisit (FTCS, Dufort Frankel, Leapfrog, dll) dan skema-skema beda hingga implisit yang dapat dibagi menjadi dua bagian (BTCS, Richardson, CrankNicolson , ADI). Persamaan adveksi difusi adalah persamaan diferensial parsial yang menggambarkan suatu masalah dengan fenomena transportasi kontaminan aliran air tanah,  sering disebut sebagai transportasi massal atau transportasi zat terlarut. Ada dua proses dasar yang bermasalah ketika mengangkut polutan di aliran air: difusi dan adveksi.

Matematika merupakan alat yang menarik untuk memodelkan fenomena  alam, karena matematika merancang fenomena alam dalam bentuk struktur matematika. Persamaan  lain yang memodelkan fenomena  alam adalah persamaan  yang sering disebut persamaan konveksi-difusi atau persamaan transpor. Persamaan konveksi-difusi adalah rumus yang digunakan untuk mempelajari fenomena transportasi polutan. Persamaan transpor merupakan salah satu persamaan diferensial yang menggambarkan sirkulasi aliran air di suatu muara dengan besaran C (konsentrasi garam) sebagai fungsi ruang dan waktu. Pemodelan matematika sering menemukan persamaan diferensial kompleks yang perlu diselesaikan secara analitik. Namun, solusi dari persamaan diferensial ini tidak hanya analitik, tetapi juga  numerik. Solusi numerik adalah metode untuk merumuskan masalah matematika  sehingga mereka dapat diselesaikan dengan operasi aritmatika dan operasi logika. Dengan perkembangan komputer dengan waktu komputasi yang  cepat,  pemodelan matematika menjadi lebih umum dengan penerapan metode numerik yang memfasilitasi penyelesaian persamaan matematika dalam  model matematika yang  dibuat. Teknik numerik kadang-kadang disebut sebagai matematika komputasi karena komputer digital pandai melakukan operasi tersebut.

- **ADVEKSI-DIFUSI 1D**

Persamaan adveksi 1 dimensi yang digunakan : 

df/dt= -U df/dx                     (1)

Persamaan difusi 1 dimensi yang digunakan : 

df/dt = Ad d**2f/dx                 (2)

Persamaan adveksi - difusi 1 dimensi yang digunakan : 

df/dt = -U df/dx + Ad d**2f/dx      (3)

Dimana f menggambarkan konsentrasi suatu zat terlarut, U adalah koefisien adveksi, dan Ad adalah koefisien difusi, dan x adalah arah sumbu horisontal.

   - Diskritisasi Model Persamaan Adveksi 1 Dimensi

  Persamaan beda hingga dengan metode ini adalah pendekatan beda maju untukturunan waktu, sedangkan untuk turunan terhadap ruang dilakukan dengan melihat arahkecepatan u. Jika u>0 maka turunan terhadap ruang menggunakan pendekatan bedamundur, sebaliknya jika u<0 digunakan pendekatan beda maju. Persamaan (1)didiskritisasi menjadi:
![Screenshot (327)](https://user-images.githubusercontent.com/92524237/170057822-b53af133-22b1-4131-a6ff-464eb60268b2.png)
Untuk mengurangi keruwetan pemrograman, maka persamaan (1.1) dan (1.2)digabungkan sehingga diskritisasi persamaan adveksi dengan metode upstream adalah:
![Screenshot (329)](https://user-images.githubusercontent.com/92524237/170058870-f28a42f8-6edb-4efb-8405-4081cc83da38.png)

   - Diskritisasi Model Persamaan Difusi 1 Dimensi

  Persamaan beda hingga mentode ini adalah pendekatan beda maju untuk turunanwaktu dan beda pusat untuk turunan ruang. Bila indeks n untuk waktu, indeks i untukruang, dan AD dianggap konstan terhadap ruang dan waktu, maka persamaan (3.1) dapatdideskritisasi menjadi :
![Screenshot (331)](https://user-images.githubusercontent.com/92524237/170059773-47f8a34f-6a94-4b95-a9d1-3641ed229661.png)

   - Diskritisasi Model Persamaan Adveksi-Difusi1 Dimensi
 
  Penyelesaian persamaan (4.1) dilakukan dengan beda hingga dimana sukuAdveksi menggunakan Metode Eksplisit Upstream, sedangkan suku difusimenggunakan pendekatan beda maju untuk turunan waktu dan beda pusat untuk turunan ruang.
![Screenshot (333)](https://user-images.githubusercontent.com/92524237/170060292-6b0c9f94-57d0-4669-a031-1880b8db3a83.png)
![Screenshot (335)](https://user-images.githubusercontent.com/92524237/170060499-34c19b79-54a3-4e80-92a9-07a03b87dfb4.png)


HIDRODINAMIKA
Hidrodinamika adalah cabang dari mekanika fluida, khususnya zat cair incompressible yang dipengaruhi oleh gaya internal dan eksternal. Dalam hidrodinamika laut gaya-gaya yang terpenting adalah gaya gravitasi, gaya gesekan, dan gaya coriolis. Dalam oseanografi, mekanika fluida digunakan berdasarkan mekanika Newton yang dimodifikasi dengen memperhitungkan turbulensi.
# 2. METODE DAN HASIL
1. Modul 2 : Persamaan Adveksi - Difusi 2D
2. Modul 3 : Persamaan Hidrodinamika 1D Sederhana
3. Modul 4 : Persamaan Hidrodinamika 2D Sederhana
# 2.1 Modul 2 : Persamaan Adveksi - Difusi 2D
Adveksi - Difusi 2D merupakan metode eksplisit dimana persamaan beda hingga dengan metode ini menggunakan pendekatan beda maju untuk turunan waktu, sedangkan untuk turunan terhadap ruang dilakukan dengan melihat arah kecepatan u. Jika u > 0 maka turunan terhadap ruang menggunakanpendekatan beda mundur, sebaliknya jika u < 0 digunakan pendekatan beda maju. Persamaan adveksi difusi-2D digunakan untuk memodelkan pergerakan polutan di laut.Persamaan pembangun yang berhubungan dengan transportasi konsentrasi polutan berupa persamaan Difusi 2D yakni 
![image](https://user-images.githubusercontent.com/78490254/169945155-12fcf280-d912-42c3-82e3-6df12c6b44da.png)
dimana 𝐶 menyatakan konsentrasi polutan yang terangkut dalam arah sumbu 𝑥 dan 𝑦. Konstanta 𝑉𝑥 dan 𝑉𝑦 disini menyatakan kecepatan aliran yang searah sumbu 𝑥 dan 𝑦 berturut turut. Juga 𝐷𝑥 dan 𝐷𝑦 juga merupakan konstanta yang menyatakan koefisien difusi yang searah sumbu 𝑥 dan sumbu 𝑦 berturut turut. Adapun syarat awal dan syarat batas yang menyertai persamaan pembangun akan dimulai dari domain yang teratur sebagai verifikasi solusi numerik, hingga ke domain yang tidak teratur,dan persamaan diskritisasi untuk model adveksi difusi 2D adalah sebagai berikut:
![image](https://user-images.githubusercontent.com/78490254/169945433-59a4eae5-71df-4a11-b1e8-fc93e0b8c75e.png)

Contoh Script :

#parameter awal

C = 0.84  #nilai kecepatan aliran

ad = 1.84  #koefisiendifusi

#skenario 1

#theta = 84 #CFL:0.569473691923612

#skenario 2

#theta = 60 + 84 #CFL:0.6198796573015902

#skenario 3

#theta = 135 + 84 #CFL:0.6250694134910891

#skenario 4

theta = 315 + 84 #CFL:0.6250694134910892

#paramter lanjutan

q = 0.95

x = 300

y = 300

dx = 3

dy = 3
# 2.2 Modul 3 : Persamaan Hidrodinamika 1D Sederhana
Pada modul 3 dibahas mengenai model hidrodinamika 1D sederhana dengan menggunakan 2 persamaan yaitu persamaan kontinuitas dan persamaan momentum. Dalam pemodelan yang dilakukan, terdapat dua parameter yang terdapat di dalam pembuatan model yaitu kecepatan arus dan perubahan elevasi muka air dengan masing – masing parameter ini memiliki 2 hasil yaitu di dalam grid tertentu dan dalam waktu tertentu. Sehingga akan menghasilkan 4 grafik yang mewakili kondisi masing-masing parameter.

Berikut ini merupakan Script dari pengerjaan modul 3 ini :
Masukkan library yang diperlukan yakni *Matplotlib* dan *Numpy*
```
import matplotlib.pyplot as plt
import numpy as np
```
Kemudian masukkan parameter awal 
```
p = 5000		#Panjang Grid
T = 1200		#Waktu Simulasi
A = 0.5		  #Amplitudo
D = 15		  #Depth/Kedalaman
dt = 2
dx = 100
To = 300		#Periode
```
Masukkan pula parameter lanjutannya
```
g = 9.8		#Koefisien Gravitasi
pi = np.pi 
C = np.sqrt(g*D)	#Kecepatan Arus
s = 2*pi/To		#Kecepatan Sudut Gelombang
L = C*To		#Panjang Gelombang
k = 2*pi/L		#Koefisien Panjang Gelombang
Mmax = int(p//dx)
Nmax = int(T//dt)
```
Selanjutnya, dilakukan penyelesaian persamaan hidrodinamika 1D
```
zo = [None for _ in range(Mmax)]
uo = [None for _ in range(Mmax)]

hasilu = [None for _ in range(Nmax)]
hasilz = [None for _ in range(Nmax)]

for i in range(1, Mmax+1):
  zo[i-1] = A*np.cos(k*(i)*dx)
  uo[i-1] = A*C*np.cos(k*((i)*dx+(0.5)*dx))/(D+zo[i-1])
for i in range(1, Nmax+1):
  zb = [None for _ in range(Mmax)]
  ub = [None for _ in range(Mmax)]
  zb[0] = A*np.cos(s*(i)*dt)
  ub[-1] = A*C*np.cos(k*L-s*(i)*dt)/(D+zo[-1])
  for j in range (1, Mmax):
    ub[j-1] = uo[j-1]-g*(dt/dx)*(zo[j]-zo[j-1])
  for k in range(2, Mmax+1):
    zb[k-1] = zo[k-1]-(D+zo[k-1])*(dt/dx)*(ub[k-1]-ub[k-2])
    hasilu[i-1] = ub
    hasilz[i-1] = zb
  for p in range(0, Mmax):
    uo[p] = ub[p]
    zo[p] = zb[p]
```
Lalu, dibuat grafik dengan menambahkan identitas diri
```
def rand_col_hex_string():
  return f'#{format(np.random.randint(0,16777215), "#08x")[2:]}'

hasilu_np = np.array(hasilu)
hasilz_np = np.array(hasilz)

fig0, ax0 = plt.subplots(figsize=(12,8))
for i in range (1, 16):
  col0 = rand_col_hex_string()
  line, = ax0.plot(hasilu_np[:,i-1], c=col0, label=f'n={i}')
  ax0.legend()

  ax0.set(xlabel='Waktu', ylabel='Kecepatan Arus', title='''Team 12 Praktikum Pemodelan Oseanografi
  Perubahan Kecepatan Arus Dalam Grid Tertentu di sepanjang Waktu''')
  ax0.grid()

fig1, ax1 = plt.subplots(figsize=(12,8))
for i in range(1, 16):
  col1= rand_col_hex_string()
  line, = ax1.plot(hasilz_np[:,i-1], c=col1, label=f'n={i}')
  ax1.legend()

  ax1.set(xlabel='Waktu', ylabel='Elevasi Muka Air', 
          title='''Team 12 Praktikum Pemodelan Oseanografi
          Perubahan Elevasi Permukaan Air Dalam Grid Tertentu di sepanjang Waktu''')
  ax1.grid()

fig2, ax2 = plt.subplots(figsize=(12,8))
for i in range(1, 16):
  col2= rand_col_hex_string()
  line, = ax2.plot(hasilu_np[i-1], c=col2, label=f't={i}')
  ax2.legend()

  ax2.set(xlabel='Grid', ylabel='Kecepatan Arus', 
          title='''Team 12 Praktikum Pemodelan Oseanografi
          Perubahan Kecepatan Arus Dalam Waktu Tertentu di Sepanjang Grid''')
  ax2.grid()

fig3, ax3 = plt.subplots(figsize=(12,8))
for i in range(1, 16):
  col3= rand_col_hex_string()
  line, = ax3.plot(hasilz_np[i-1], c=col3, label=f't={i}')
  ax3.legend()

  ax3.set(xlabel='Grid', ylabel='Elevasi Muka Air', 
          title='''Team 12 Praktikum Pemodelan Oseanografi
          Perubahan Elevasi Muka Air Dalam Waktu Tertentu di Sepanjang Grid''')
  ax3.grid()

plt.show()
```
# 2.3 Modul 4 : Persamaan Hidrodinamika 2D Sederhana

# 3. PENERAPAN DALAM BIDANG OSEANOGRAFI
# Modul 1 : Persamaan Adveksi - Difusi 1D
Penerapan Adveksi-Difusi 1D di dalam bidang Oseaografi :
- Mengetahui konsentrasi dan penyebaran polutan di sungai, parit, dan cabang sungai
- Pemodelan polutan
- Konservasi lingkungan
# Modul 2 : Persamaan Adveksi - Difusi 2D
Penerapan Persamaan Persamaan Adveksi - Difusi 2D di dalam bidang oseanografi :
- Menghitung dan memodelkan persebaran nutrien di laut atau sungai 
- Menghitung dan memodelkan penyebaran polutan dari proses industri
- Mengetahui persebaran polutan dari laguna dengan menghitung input dan outputnya
- Mengetahui sebaran kebocoran minyak di laut
# Modul 3 : Persamaan Hidrodinamika 1D Sederhana
Penerapan Persamaan Hidrodinamika 1D di dalam bidang Oseaografi :
- Mengetahui sebaran tumpahan minyak mentah yang ada di perairan menggunakan data arah pergerakan arus pasang surut
- Untuk mengkaji fenomena suhu dingin di perairan 
- Mengetahui sebaran limbah air panas yang masuk ke perairan
# Modul 4 : Persamaan Hidrodinamika 2D Sederhana
Penerapan Persamaan Hidrodinamika 2D di dalam bidang Oseaografi :
- Pemodelan gelombang karena angin
- Pemodelan sampah plastik di laut
- Pemodelan coastal dynamics dan sedimentasi pantai
