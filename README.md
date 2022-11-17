Nama    : Alya Sefhia Eka Putri

NIM     : 312210108

Kelas   : TI.22.B1

              Repository ini dibuat untuk memenuhi tugas Pertemuan ke 9 Praktikun 4 Module Bahasa Pemograman

Pada halaman ini Tugas Pertemuan ke 9 Module Praktikum 4,Dosen memberi tugas dua bahan praktik seperti berikut:

1.  Soal Latihan yang ada pada module praktikum 4

    ![Soal Latihan](https://user-images.githubusercontent.com/115520278/202364645-e28a4e2d-7127-45c4-beb4-fe249bbef760.png)
    
 - Berikut ini saya menulis syntax sekaligus menuliskan langkah-langkahnya 
 
          print("===================================================================")
          print("Nama         :   Alya Sefhia Eka Putri")
          print("NIM          :   312210108")
          print("Kelas        :   TI.22.B1")
          print("Mata Kuliah  :   Bahasa Pemrograman")
          print("===================================================================")

          # membuat list
          print("Buat sebuah list sebanyak 5 elemen dengan nilai bebas")
          list = [1, 2, 3, 4, 5]
          print(list)

          # mengakses list
          print("Menampilkan elemen 3")
          print(list[2])

          print("ambil nilai elemen 2 sampai ke 4")
          print(list[1:4])

          print("ambil elemen terakhir")
          print(list[-1])

          # mengubah elemen list
          print("ubah elemen 4 dengan nilai lainnya")
          list[4]=10
          print(list[3])

          print("ubah elemen 4 sampai dengan elemen terakhir")
          list[4:5]=[20,11]
          print(list)

          # Tambah elemen list
          print("Ambil 2 bagian dari list pertama(A) dan jadikan list ke 2(B)")
          list_pertama=list[3:5]
          print(list_pertama)

          print("tambah list B dengan nilai string")
          list_pertama.append("guest")
          print(list_pertama)

          print("Tambah list B dengan 3 nilai")
          list_pertama.append(["guest",7,8])
          print(list_pertama)

          print("Menggabungkan list B dengan list A")
          gabung=list_pertama+list
          print(gabung)

- Berikut hasil run syntax untuk memenuhi latihan module 4 diatas 

  ![Latihan_4_Module](https://user-images.githubusercontent.com/115520278/202365573-a99ad186-089f-4b37-bf87-75be71e3066f.PNG)
  
2.  Soal Tugas Praktikum 4 Module 

    ![Tugas Pratikum](https://user-images.githubusercontent.com/115520278/202365940-26bfdf4b-58c2-4e92-b7c2-4d60e6ca5965.png)
    
- Pada soal tugas ini saya akan menulis dan menjelaskan syntax yang saya buat sebagai berikut

          print("===================================================================")
          print("Nama         :   Alya Sefhia Eka Putri")
          print("NIM          :   312210108")
          print("Kelas        :   TI.22.B1")
          print("Mata Kuliah  :   Bahasa Pemrograman")
          print("===================================================================")
          print("Tugas Praktikum module 4")

          # Buat program sederhana untuk menambahkan data kedalam sebuah list dengan rincian sebagai berikut: • Progam meminta
          # memasukkan data sebanyak-banyaknya (gunakan perulangan) • Tampilkan pertanyaan untuk menambah data (y/t?),
          # apabila jawaban t (Tidak), maka program akan menampilkan daftar datanya. • Nilai Akhir diambil dari perhitungan 3
          # komponen nilai (tugas: 30%, uts: 35%, uas: 35%) • Buat flowchart dan penjelasan programnya pada README.md. • Commit
          # dan push repository ke github.

          from prettytable import PrettyTable 

          baris = []
          stop = False

          # masukan nilai
          while (not stop):
              nama = input("Masukan Nama : ")
              nim = input("Masukan NIM : ")
              tugas = input("Masukan Nilai Tugas : ")
              uts = input("Masukan Nilai UTS : ")
              uas = input("Masukan Nilai UAS : ")
              nilai_akhir = 0.3 * float(tugas) + 0.35 * float(uts) + 0.35 * float(uas)
              baris.append([nama, nim, tugas, uts, uas, nilai_akhir])

              tanya = input("Tambah data? (y/n) : ")
              if (tanya == "n"):
                  stop = True

          # cetak nilai
          print("===================================================================")

          x = PrettyTable()
          no = 0

          for isi in baris:
              no += 1
              x.field_names = ["No", "Nama", "Nim", "Tugas", "UTS", "UAS", "Nilai Akhir"]
              x.add_row([no, isi[0], isi[1], isi[2], isi[3], isi[4], isi[5]])
          print(x)
          
- Berikut hasil run syntax yang saya buat untuk memenuhi praktikum 4 module  

  ![2022-11-17](https://user-images.githubusercontent.com/115520278/202366520-014b7683-871d-43a7-b8de-f4675871d79c.png)
  
- Berikut adala program Flowchart di atas

  ![Flowchart Module 4](https://user-images.githubusercontent.com/115520278/202366810-4f487501-1501-465e-b9b4-d49600f16959.png)
  
      Penjelasan singkat tentang fungsi While untuk mengatur kondisi seperti while not stop dan jika tidak
      berhenti maka system akan terus menampilkan perintah user untuk meninputkan data . Untuk perhitungan nilai
      akhir sesuai ketentuan yang dosen inginkan. Sedangkan untuk menampilkan hasil dari inputan user tersebut menggunakan fungsi/module yang ada pada PrettyTable bisa mengakses link berikut ini untuk panduan installation :

      *[How to install PIP](https://phoenixnap.com/kb/install-pip-windows)
      *[How to install PrettyTable](https://pypi.org/project/prettytable/)
      *[How to install Numpy](https://stackoverflow.com/questions/60496280/python-error-modulenotfounderror-no-module-named-modulename/60496306#60496306?newreg=38536a77f74f40a691560e099363f4c3)
      
Berikut adalah langkah - langkah tugas pertemuan ke 9 Praktikum 4 Module yang bisa saya jabarkan

Terimakasih....
