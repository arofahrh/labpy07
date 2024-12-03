# praktikum 7
    Buat program sederhana dengan mengaplikasikan penggunaan class. Buatlah
    class untuk menampilkan daftar nilai mahasiswa, dengan ketentuan:
    • Method tambah() untuk menambah data
    • Method tampilkan() untuk menampilkan data
    • Method hapus(nama) untuk menghapus data berdasarkan nama
    • Method ubah(nama) untuk mengubah data berdasarkan nama
    • Buat diagram class, flowchart dan penjelasan programnya pada README.md.
    • Commit dan push repository ke github.

# flowchart 

![Screenshot 2024-12-03 192124](https://github.com/user-attachments/assets/ec68f3f9-219e-4c84-b17b-e846ee23a3c7)

# diagram class
![Screenshot 2024-12-02 130300](https://github.com/user-attachments/assets/60084022-6da1-447f-9109-de3b8015e249)

# kode python
    
    class DaftarNilaiMahasiswa:
        def __init__(self):  
            self.mahasiswa = {}

    def tambah(self, nama, nilai):
        """Menambah data mahasiswa."""
        self.mahasiswa[nama] = nilai
        print(f"Data {nama} dengan nilai {nilai} berhasil ditambahkan.")

    def tampilkan(self):
        """Menampilkan semua data mahasiswa."""
        if not self.mahasiswa: 
            print("Tidak ada data mahasiswa.")
        else:
            print("Daftar Nilai Mahasiswa:")
            for nama, nilai in self.mahasiswa.items():
                print(f"Nama: {nama}, Nilai: {nilai}")

    def hapus(self, nama):
        """Menghapus data mahasiswa berdasarkan nama."""
        if nama in self.mahasiswa:
            del self.mahasiswa[nama]
            print(f"Data {nama} berhasil dihapus.")
        else:
            print(f"Data {nama} tidak ditemukan.")

    def ubah(self, nama, nilai_baru): 
        """Mengubah data mahasiswa berdasarkan nama."""
        if nama in self.mahasiswa:
            self.mahasiswa[nama] = nilai_baru
            print(f"Data {nama} berhasil diubah menjadi nilai {nilai_baru}.")
        else:
            print(f"Data {nama} tidak ditemukan.")
    if __name__ == "__main__":
        daftar_nilai = DaftarNilaiMahasiswa()

    # Menambahkan data
    daftar_nilai.tambah("travis", 90)
    daftar_nilai.tambah("scott", 85)

    # Menampilkan data
    daftar_nilai.tampilkan()

    # Mengubah data
    daftar_nilai.ubah("travis", 95)

    # Menampilkan data setelah diubah
    daftar_nilai.tampilkan()

    # Menghapus data
    daftar_nilai.hapus("scott")

    # Menampilkan data setelah dihapus 
    daftar_nilai.tampilkan()  

 # penjelasan kode :
 1. Definisi Kelas DaftarNilaiMahasiswa:
    - Kelas ini digunakan untuk menyimpan dan mengelola data mahasiswa beserta nilai-nilai mereka.
    - Di dalam kelas ini, kita memiliki metode (fungsi) yang berbeda untuk menambah, menampilkan, menghapus, dan mengubah data mahasiswa.
 2. Metode __init__:
    - Ini adalah metode yang dipanggil saat kita membuat objek baru dari kelas DaftarNilaiMahasiswa.
    - Di sini, kita membuat sebuah dictionary kosong bernama mahasiswa untuk menyimpan data mahasiswa.
 3. Metode tambah:
    - Metode ini digunakan untuk menambahkan data mahasiswa baru.
    - Kita memberikan nama dan nilai mahasiswa, dan data tersebut disimpan dalam dictionary mahasiswa.
    - Setelah data ditambahkan, kita mencetak pesan bahwa data berhasil ditambahkan.
 4. Metode tampilkan:
    - Metode ini digunakan untuk menampilkan semua data mahasiswa yang telah ditambahkan.
    - Jika tidak ada data, maka akan muncul pesan "Tidak ada data mahasiswa."
    - Jika ada data, kita akan mencetak daftar nama dan nilai mahasiswa.
 5. Metode hapus:
    - Metode ini digunakan untuk menghapus data mahasiswa berdasarkan nama.
    - Jika nama mahasiswa ada dalam dictionary, maka data tersebut akan dihapus dan kita akan mencetak pesan bahwa data berhasil dihapus.
    - Jika nama tidak ditemukan, kita akan mencetak pesan bahwa data tidak ditemukan.
 6. Metode ubah:
    - Metode ini digunakan untuk mengubah nilai mahasiswa yang sudah ada.
    - Jika nama mahasiswa ditemukan, kita akan mengubah nilainya dan mencetak pesan bahwa data berhasil diubah.
    - Jika nama tidak ditemukan, kita akan mencetak pesan bahwa data tidak ditemukan.
  - Contoh Penggunaan Kode
    Di bagian bawah kode, kita memiliki contoh penggunaan kelas DaftarNilaiMahasiswa:
1. Membuat Objek:
   Kita membuat objek baru dari kelas DaftarNilaiMahasiswa dengan nama daftar_nilai.
2. Menambahkan Data:
   Kita menambahkan dua mahasiswa: "travis" dengan nilai 90 dan "scott" dengan nilai 85.
3. Menampilkan Data:
   Setelah menambahkan data, kita menampilkan semua data mahasiswa yang ada.
4. Mengubah Data:
   Kita mengubah nilai mahasiswa "travis" dari 90 menjadi 95.
5. Menampilkan Data Setelah Diubah:
   Kita menampilkan data lagi untuk melihat perubahan yang telah dilakukan.
6. Menghapus Data:
   Kita menghapus data mahasiswa "scott".
7. Menampilkan Data Setelah Dihapus:
   Kita menampilkan data lagi untuk memastikan bahwa "scott" sudah dihapus.

# input dan output :
![Screenshot 2024-12-03 194742](https://github.com/user-attachments/assets/e4f1fe93-a54e-4a6d-a8f8-dfcc08f0b458)
