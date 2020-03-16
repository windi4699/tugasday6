Soal 7.1 Implementasikan kode berikut yang merupakan contoh dan cara mengakses data dari array dua dimensi:
In [3]:
//program 7.1

 String[][] Siswa = {
    {"Lili","08111"},
    {"Lala","08122"},
    {"Maya","08133"}
};

for(int x=0; x < Siswa.length; x++){
    System.out.println("Nama "+Siswa[x][0]);
    System.out.println("NIM "+Siswa[x][1]);
}
Nama Lili
NIM 08111
Nama Lala
NIM 08122
Nama Maya
NIM 08133
Out[3]:
null
Soal 7.2 Terdapat sebuah data tabular Mahasiswa dengan dengan tabel sebagai berikut :
| NIM | Nama |IPK|
|"08111"|"Dono "|3.0| |"08113"|"Kasino"|2.7| |"08115"|"Indro "|3.1|
Implementasikan data tabular Mahasiswa diatas dalam sebuah array multi dimensi kedalam program 7.2
In [40]:
String[][] mahasiswa = {
     {"08111","Dono","3.0"},
     {"08113","Kasino","2.7"},
     {"08115","Indro","3.1"}
};

for(int m =0; m < mahasiswa.length; m++){
    System.out.println("Nama "+mahasiswa[m][0]);
    System.out.println("NIM "+mahasiswa[m][1]);
    System.out.println("IPK "+mahasiswa[m][2]);
}
Nama 08111
NIM Dono
IPK 3.0
Nama 08113
NIM Kasino
IPK 2.7
Nama 08115
NIM Indro
IPK 3.1
Out[40]:
null
+){
    System.out.println("Nama "+mahasiswa[m][0]);
    System.out.println("NIM "+mahasiswa[m][1]);
    System.out.println("IPK "+mahasiswa[m][2]);
}
Nama 08111
NIM Dono
IPK 3.0
Nama 08113
NIM Kasino
IPK 2.7
Nama 08115
NIM Indro
IPK 3.1
Out[40]:
null
Soal 7.4 Implementasikan kode Program 7.4 dibawah ini, lakukan juga inisisiali untuk element element dari array yang dibutuhkan
In [23]:
//Program 7.3
class PersegiPanjang{
    int panjang;
    int lebar;
    int luas;

    void setPanjang(int panjang) { 
        this.panjang = panjang;
    } 

    void setLebar(int lebar) { 
        this.lebar = lebar; 
    } 
    int getLuas(){
      luas = panjang * lebar;
      return luas;  
    }
}
Out[23]:
com.twosigma.beaker.javash.bkr903bf611.PersegiPanjang
In [27]:
PersegiPanjang [] myArray = new PersegiPanjang [3];

        myArray[0] = new PersegiPanjang();
        myArray[0].setPanjang(10); 
        myArray[0].setLebar(5);

        System.out.println("Luas Element ke 0 "+ myArray[0].getLuas());

   
        for (int i = 0; i < myArray.length; i++) {
            System.out.println("Luas Element ke "+i+ " "+myArray[i].getLuas());
            
        }
Luas Element ke 0 50
Luas Element ke 0 50
ERROR: java.lang.NullPointerException
In [ ]:
import java.util.ArrayList;

        ArrayList kantongAjaib = new ArrayList();

        // Mengisi kantong ajaib dengan 5 benda
        kantongAjaib.add("Senter Pembesar");
        kantongAjaib.add(532);
        kantongAjaib.add("tikus");
        kantongAjaib.add(1231234.132);
        kantongAjaib.add(true);

        // menghapus tikus dari kantong ajaib
        kantongAjaib.remove("tikus");

        // Menampilkan isi kantong ajaib
        System.out.println(kantongAjaib);

        // menampilkan banyak isi kantong ajaib
        System.out.println("Kantong ajaib berisi "+ kantongAjaib.size() +" item");
Soal 7.6 Lakukan eksekusi dari kode diatas dan amati hasilnya
In [28]:
import java.util.ArrayList;

        ArrayList kantongAjaib = new ArrayList();

        // Mengisi kantong ajaib dengan 5 benda
        kantongAjaib.add("Senter Pembesar");
        kantongAjaib.add(532);
        kantongAjaib.add("tikus");
        kantongAjaib.add(1231234.132);
        kantongAjaib.add(true);

        // menghapus tikus dari kantong ajaib
        kantongAjaib.remove("tikus");

        // Menampilkan isi kantong ajaib
        System.out.println(kantongAjaib);

        // menampilkan banyak isi kantong ajaib
        System.out.println("Kantong ajaib berisi "+ kantongAjaib.size() +" item");
[Senter Pembesar, 532, 1231234.132, true]
Kantong ajaib berisi 4 item
Out[28]:
null
In [ ]:
import java.util.HashMap;

        //Program 7.7

        // membuat objek hashmap
        HashMap<Integer, String> hari = new HashMap<Integer,String>();

        // mengisi nilai ke objek days
        hari.put(1, "Minggu");
        hari.put(2, "Senin");
        hari.put(3, "Selasa");
        hari.put(4, "Rabu");
        hari.put(5, "Kamis");
        hari.put(6, "Jum'at");
        hari.put(7, "Sabtu");

        // mencetak semua isi dari objek days
        System.out.println("Isi objek days: " + hari);
Soal 7.7 Lakukan eksekusi dari kode diatas dan amati hasilnya
In [29]:
import java.util.HashMap;

        //Program 7.7

        // membuat objek hashmap
        HashMap<Integer, String> hari = new HashMap<Integer,String>();

        // mengisi nilai ke objek days
        hari.put(1, "Minggu");
        hari.put(2, "Senin");
        hari.put(3, "Selasa");
        hari.put(4, "Rabu");
        hari.put(5, "Kamis");
        hari.put(6, "Jum'at");
        hari.put(7, "Sabtu");

        // mencetak semua isi dari objek days
        System.out.println("Isi objek days: " + hari);
Isi objek days: {1=Minggu, 2=Senin, 3=Selasa, 4=Rabu, 5=Kamis, 6=Jum'at, 7=Sabtu}
Out[29]:
null
In [ ]:
//program 7.8 
        import java.util.HashMap;

        // membuat objek hashmap
        HashMap<Integer, String> harihari = new HashMap<Integer,String>();

        // mengisi nilai ke objek hari
        harihari.put(1, "Minggu");
        harihari.put(2, "Senin");
        harihari.put(3, "Selasa");
        harihari.put(4, "Rabu");
        harihari.put(5, "Kamis");
        harihari.put(6, "Jum'at");
        harihari.put(7, "Sabtu");

        // mencetak semua isi dari objek hari
        System.out.println("Isi objek days: " + harihari);
        // mengambil hari senin
        System.out.println("Hari kedua: " + harihari.get(2));
Soal 7.8 Lakukan eksekusi dari kode diatas dan amati hasilnya
In [30]:
//program 7.8 
        import java.util.HashMap;

        // membuat objek hashmap
        HashMap<Integer, String> harihari = new HashMap<Integer,String>();

        // mengisi nilai ke objek hari
        harihari.put(1, "Minggu");
        harihari.put(2, "Senin");
        harihari.put(3, "Selasa");
        harihari.put(4, "Rabu");
        harihari.put(5, "Kamis");
        harihari.put(6, "Jum'at");
        harihari.put(7, "Sabtu");

        // mencetak semua isi dari objek hari
        System.out.println("Isi objek days: " + harihari);
        // mengambil hari senin
        System.out.println("Hari kedua: " + harihari.get(2));
Isi objek days: {1=Minggu, 2=Senin, 3=Selasa, 4=Rabu, 5=Kamis, 6=Jum'at, 7=Sabtu}
Hari kedua: Senin
Out[30]:
null
In [ ]:
import java.util.HashMap;

        //Program 7.9

        // membuat objek hashmap
        HashMap<Integer, String> days = new HashMap<Integer,String>();

        // mengisi nilai ke objek days
        days.put(1, "Minggu");
        days.put(2, "Senin");
        days.put(3, "Selasa");
        days.put(4, "Rabu");
        days.put(5, "Kamis");
        days.put(6, "Jum'at");
        days.put(7, "Sabtu");

        // mencetak semua isi dari objek days
        System.out.println("Isi objek days: " + days);
        System.out.println("Hari kedua: " + days.get(2));

        // menghapus malam minggu <-- jomblo detected :D
        days.remove(1);
        System.out.println("Isi objek days: " + days);

        // menghapus semua hari <-- oh tidak kiamat donk!
        days.clear();
        System.out.println("Isi objek days: " + days);
Soal 7.9 Lakukan eksekusi dari kode diatas dan amati hasilnya
In [31]:
import java.util.HashMap;

        //Program 7.9

        // membuat objek hashmap
        HashMap<Integer, String> days = new HashMap<Integer,String>();

        // mengisi nilai ke objek days
        days.put(1, "Minggu");
        days.put(2, "Senin");
        days.put(3, "Selasa");
        days.put(4, "Rabu");
        days.put(5, "Kamis");
        days.put(6, "Jum'at");
        days.put(7, "Sabtu");

        // mencetak semua isi dari objek days
        System.out.println("Isi objek days: " + days);
        System.out.println("Hari kedua: " + days.get(2));

        // menghapus malam minggu <-- jomblo detected :D
        days.remove(1);
        System.out.println("Isi objek days: " + days);

        // menghapus semua hari <-- oh tidak kiamat donk!
        days.clear();
        System.out.println("Isi objek days: " + days);
Isi objek days: {1=Minggu, 2=Senin, 3=Selasa, 4=Rabu, 5=Kamis, 6=Jum'at, 7=Sabtu}
Hari kedua: Senin
Isi objek days: {2=Senin, 3=Selasa, 4=Rabu, 5=Kamis, 6=Jum'at, 7=Sabtu}
Isi objek days: {}
Out[31]:
null
In [ ]:
import java.util.HashMap;

        //program 7.10

        // membuat objek hashmap
        HashMap<Integer, String> days = new HashMap<Integer,String>();

        // mengisi nilai ke objek days
        days.put(1, "Minggu");
        days.put(2, "Senin");
        days.put(3, "Selasa");
        days.put(4, "Rabu");
        days.put(5, "Kamis");
        days.put(6, "Jum'at");
        days.put(7, "Sabtu");

        // mengubah hari menggu menjadi hari ahad
        days.put(1, "Ahad");

        // mengubah hari rabu menjadi rabo
        days.replace(4, "Rabo");

        // mencetak semua isi dari objek days
        System.out.println("Isi objek days: " + days);
Soal 7.10 Lakukan eksekusi dari kode diatas dan amati hasilnya
In [32]:
import java.util.HashMap;

        //program 7.10

        // membuat objek hashmap
        HashMap<Integer, String> days = new HashMap<Integer,String>();

        // mengisi nilai ke objek days
        days.put(1, "Minggu");
        days.put(2, "Senin");
        days.put(3, "Selasa");
        days.put(4, "Rabu");
        days.put(5, "Kamis");
        days.put(6, "Jum'at");
        days.put(7, "Sabtu");

        // mengubah hari menggu menjadi hari ahad
        days.put(1, "Ahad");

        // mengubah hari rabu menjadi rabo
        days.replace(4, "Rabo");

        // mencetak semua isi dari objek days
        System.out.println("Isi objek days: " + days);
Isi objek days: {1=Ahad, 2=Senin, 3=Selasa, 4=Rabo, 5=Kamis, 6=Jum'at, 7=Sabtu}
Out[32]:
null
In [33]:
//program 7.11
public class Buku {

    private String title;
    private String author;

    public Buku(String title, String author) {
        this.title = title;
        this.author = author;
    }

    public String getTitle() {
        return title;
    }

    public void setTitle(String title) {
        this.title = title;
    }

    public String getAuthor() {
        return author;
    }

    public void setAuthor(String author) {
        this.author = author;
    }

}
Out[33]:
com.twosigma.beaker.javash.bkr903bf611.Buku
In [34]:
// program 7.12

import java.util.HashMap;
import java.util.Map;

        // membuat objek hashmap
        HashMap<String, Buku> books = new HashMap<String, Buku>();

        // membuat objek buku
        Buku bukuJava = new Buku("Tutorial Java", "Petani Kode");
        Buku bukuKotlin = new Buku("Pemrograman Kotlin", "Petani Kode");
        Buku bukuAndroid = new Buku("Pemrograman Android", "Petani Kode");

        // mengisi objek hashmap dengan objek buku
        books.put("java", bukuJava);
        books.put("kotlin", bukuKotlin);
        books.put("android", bukuAndroid);

        // cetak semua buku
        for(Map.Entry b: books.entrySet()){
            Buku buku = (Buku) b.getValue();
            System.out.println(b.getKey() + ": "+ buku.getTitle());
        }
java: Tutorial Java
android: Pemrograman Android
kotlin: Pemrograman Kotlin
Out[34]:
null
In [ ]:
