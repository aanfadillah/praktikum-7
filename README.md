## NAMA : AAN FADILLAH PUTRA
## NIM : 312210327
## KELAS : TI.22.A.3

# Soal

![aan 2](https://user-images.githubusercontent.com/115763475/205222864-07b39d65-96b3-40e9-8908-8eaa0df8081b.jpg)

```python
x = {}

def tambah():
    print("Tambah Data")
    nama = input("Masukkan Nama Mahasiswa   : ")
    nim = input("Masukkan NIM              : ")
    tugas = int(input("Masukkan Nilai Tugas      : "))
    uts = int(input("Masukkan Nilai UTS        : "))
    uas = int(input("Masukkan Nilai UAS        : "))
    akhir = tugas * 30/100 + uts * 35/100 + uas * 35/100
    x[nama] = nim , tugas, uts , uas , akhir
def tampilkan():
    if x.items():
        print("---------------------------------------------------------------------------------")
        print("\n                               DAFTAR NILAI MAHASISWA                    ")
        print("---------------------------------------------------------------------------------")
        print("| No |      Nama      |     NIM     |  Tugas  |   UTS   |   UAS   |    Akhir    |")
        print("---------------------------------------------------------------------------------")
        i = 0
        for b in x.items():
             i += 1
             print("| {no:2d} | {0:14s} | {1:11s} | {2:7d} | {3:7d} | {4:7d} | {5:7f}   |"
                . format ( b [ 0 ][: 14 ], b [ 1 ][ 0 ], b [ 1 ][ 1 ], b [ 1 ][ 2 ], b [ 1 ][ 3 ], b [ 1 ][ 4 ] , no = i ))
        print("---------------------------------------------------------------------------------")
    else :
        print("---------------------------------------------------------------------------------")
        print("\n                               DAFTAR NILAI MAHASISWA                    ")
        print("---------------------------------------------------------------------------------")
        print("| No |      Nama      |     NIM     |  Tugas  |   UTS   |   UAS   |    Akhir    |")
        print("---------------------------------------------------------------------------------")
        print("|                                TIDAK ADA DATA                                 |")
        print("---------------------------------------------------------------------------------")
def hapus():
    print ( "Hapus Data" )
    nama = input("Masukkan Nama Mahasiswa   : ")
    if  nama in  x . keys ():
        del  x [ nama ]
    else :
        print ( "Nama {0} Tidak Ditemukan" . format ( nama ))
def ubah():
    print ( "Ubah Data" )
    nama = input("Masukkan Nama Mahasiswa   : ")
    if nama in  x . keys ():
        nim = input("Masukkan NIM              : ")
        tugas = int(input("Masukkan Nilai Tugas      : "))
        uts = int(input("Masukkan Nilai UTS        : "))
        uas = int(input("Masukkan Nilai UAS        : "))
        akhir = tugas * 30/100 + uts * 35/100 + uas * 35/100
        x[nama] = nim , tugas, uts , uas , akhir
    else :
        print ( "Nama{0} Tidak Ditemukan" . format(nama ))

while True:
    print("")
    print("===========================")
    print("|   Program Input Nilai   |")
    print("===========================")
    c = input("L)ihat, T)ambah, U)bah, H)apus, K)eluar: ")
    if c.lower() == "l":
        tampilkan()
    elif c.lower() == "t":
        tambah()
    elif c.lower() == "u":
        ubah()
    elif c.lower() == "h":
        hapus()
    elif c.lower() == "k":
        print()
        print("---------------------------------------------------------------------------------")
        print("                                 PROGRAM TELAH SELESAI                    ")
        print("---------------------------------------------------------------------------------")
        break

    else:
        print()
        print("Kode yang anda masukkan salah!")
 ```   
 
 # Outputnya
 
### Tambah(t)

![t 1 aan](https://user-images.githubusercontent.com/115763475/205223837-bb4cf931-db88-4be3-b95f-d5fa6397f3e3.png)

### Lihat(l)

![l 1 aan](https://user-images.githubusercontent.com/115763475/205224000-0159f79e-2289-49da-909a-640557975c5b.png)

### Ubah(u)

![u 1 aan](https://user-images.githubusercontent.com/115763475/205224577-e9c07279-5aa7-463b-88c4-ce8ebf4675f2.png)

### Hapus(h)

![h 1 aan](https://user-images.githubusercontent.com/115763475/205224787-c8701061-ccd6-440c-87c3-cd9e6f7cdbad.png)

### Keluar(k)

![k1 aan](https://user-images.githubusercontent.com/115763475/205225150-fdda2d8b-4ccb-45f8-ab89-81c4f8129d0f.png)

# Latihan
## Soal

![aan](https://user-images.githubusercontent.com/115763475/205227851-c2731a3d-23d5-45b5-bc26-e9acf57e0733.jpg)

```python

import math
def a(x):
  return x**2
a = lambda x : x**2
print(a(2))
def b(x, y):
  return math.sqrt(x**2 + y**2)
b = lambda x, y : x ** 2 + y ** 2
print(b(2, 2))
def c(*args):
  return sum(args)/len(args)
c = lambda *args : sum(args)/len(args)
print(c(1,2,3,4,5))
def d(s):
  return "".join(set(s))
d = lambda s: "".join(set(s))
print(d("buku"))

 ```
 
 # Ouput
 
 ![aan123](https://user-images.githubusercontent.com/115763475/205227852-9cc6bad1-66c8-423a-ba39-9ce6dcee4235.png)

# Flowchart

![Flowchart aan](https://user-images.githubusercontent.com/115763475/205229022-6e37a55e-b81f-4165-990c-f4b64b4118ea.png)

## =======================SELESAI=========================
