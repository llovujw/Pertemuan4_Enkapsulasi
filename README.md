# Pertemuan4_Enkapsulasi

## Profil
| Variable | Isi |
| -------- | --- |
| **Nama** | Intan Virginia Aulia Putri |
| **NIM** | 312310657 |
| **Kelas** | TI.23.A.6 |
| **Mata Kuliah** | Pemrograman Orientasi Objek |

### Latihan
Buatlah kode program java untuk:
- Mendeklarasikan class **Person**, dengan atribut `Nama`, `JenisKelamin`, `Umur` dan lengkapi dengan `access modifier`.
- Buatlah dua buah objek dari class **Person** bernama Anton dan Riko dan panggil method `setter` dan `getter`.

``` javascript
// Deklarasi class Person
public class Person {
    private String Nama;
    private String JenisKelamin;
    private int Umur;

    // Setter untuk atribut Nama, JenisKelamin, dan Umur
    public void setNama(String Nama) {
        this.Nama = Nama;
    }

    public void setJenisKelamin(String JenisKelamin) {
        this.JenisKelamin = JenisKelamin;
    }

    public void setUmur(int Umur) {
        this.Umur = Umur;
    }

    // Getter untuk atribut Nama, JenisKelamin, dan Umur
    public String getNama() {
        return this.Nama;
    }

    public String getJenisKelamin() {
        return this.JenisKelamin;
    }

    public int getUmur() {
        return this.Umur;
    }

    // Main method
    public static void main(String[] args) {
        // Membuat objek Anton dari class Person
        Person Anton = new Person();

        // Memanggil setter untuk mengisi nilai atribut Anton
        Anton.setNama("Anton");
        Anton.setJenisKelamin("Laki-laki");
        Anton.setUmur(25);

        // Menampilkan informasi Anton menggunakan getter
        System.out.println("Informasi Anton:");
        System.out.println("Nama: " + Anton.getNama());
        System.out.println("Jenis Kelamin: " + Anton.getJenisKelamin());
        System.out.println("Umur: " + Anton.getUmur());

        // Membuat objek Riko dari class Person
        Person Riko = new Person();

        // Memanggil setter untuk mengisi nilai atribut Riko
        Riko.setNama("Riko");
        Riko.setJenisKelamin("Perempuan");
        Riko.setUmur(30);

        // Menampilkan informasi Riko menggunakan getter
        System.out.println("\nInformasi Riko:");
        System.out.println("Nama: " + Riko.getNama());
        System.out.println("Jenis Kelamin: " + Riko.getJenisKelamin());
        System.out.println("Umur: " + Riko.getUmur());
    }
}
```
### Penjelasan
1. Class:
Sebuah `class` adalah template atau blueprint untuk membuat objek. Class mendefinisikan atribut (variabel) dan metode (fungsi) yang akan dimiliki oleh objek.
2. Atribut (Attributes):
Atribut adalah variabel yang disimpan di dalam class, yang mendeskripsikan properti dari class tersebut. Dalam contoh ini, atribut `Nama`, `JenisKelamin`, dan `Umur` adalah properti dari **Person**.
3. Access Modifier:
Access modifier digunakan untuk menentukan visibilitas atribut dan metode di dalam class. Dalam Java, ada beberapa access modifier:
    - `private`: Atribut/metode hanya bisa diakses di dalam class.
    - `public`: Atribut/metode bisa diakses dari luar class.
    - `protected` dan `default`: Digunakan untuk kontrol akses lebih lanjut, misalnya di dalam package atau subclass.
Dalam contoh ini, atribut seperti `Nama`, `JenisKelamin`, dan `Umur` bisa dibuat private untuk membatasi akses langsung dan kemudian menyediakan `setter` dan `getter` untuk mengaksesnya.
4. Setter dan Getter:
    - Setter adalah metode yang digunakan untuk mengubah nilai dari suatu atribut.
    - Getter adalah metode yang digunakan untuk mendapatkan nilai dari atribut tersebut.

#### Tampilan Output
![1](ss/1.png)
