# Praktikum04



## soal1.cpp 

**Alur Argoritma**
1. Mendeklarasikan Variable int a,max, sebagai varible input
2. memberikan perintah awal bahwa **max=0** .
3. masukan syntax do .
4. inputkan nilai yang ingin di masukan dengan cin>> **a**
5. membandikan nilain variable **A** dengan Variable **max** jika **a>max** 
6. masukan syntax while unntuk mengulang variabel.
7. inputkan/ intruksikan variabe ***a!=0** untuk menghentikan program dengan mengakhiri dengan variable ***0***
8. cetak nilai terbesar dari bilangafn acak yang di inputkan .
**flowchrt Program**
![fl1](https://github.com/ilhamhernanda01/Praktikum04/blob/master/Flowchart1.jpg)

**CODE PROGRAM**
```c++
#include<iostream>
using namespace std;
int main ()
{   cout<< "Algoritma Mencari Nilai Terbesar Dari Bilangan Yang Diinputkan"<<endl;
    cout<< "=============================================================="<<endl;
    int max,A;
    max=0;

    do{
        cout<< "masukin nilai yang ingin di masukan :"; cin >> A;
        if (max<A)
            max=A;
    }
    while (A!=0);
    cout<< "hasilnya = " <<max<< endl;
    return 0;
}
```
**HASIL**
![hasil1](https://github.com/ilhamhernanda01/Praktikum04/blob/master/hasill%20coding1.png)

## Latihan2.cpp 

**Alur Argoritma**
1. Mendeklarasikan Variable penjelas (x,y,barang,harga,jumlah barang,diskon,banyak barang,total,nilai N dan total belanjaan).
2. membaca nilai **N** untuk menginput banyaknya barang dan di deskripsikan lagi dengan (x,y) untuk varaibel pembanding
3. membandikan nilai variable **x**dan **y** dengan hasil x lebih kecil atrau sama dengan y (x<=y) mengunakan while untuk mengulang hasil semua intruksi yang di inputkan.
4. membaca atrau cetak variabel **a** untuk barang ke-
5. membaca atau cetak variable **jumlah beli** dan **harga** utuk mengisntruksikan input harga dan barang.
6. input program sesuai perintah 
        ```harga_barang = harga*jumlah_beli;
           total=total + harga_barang;
           total_beli += jumlah_beli;``` 

untuk bisa menjumlahkan hasil.
7. kemudian deskripsikan variabel diskon yang mau kita taruh di program ini dengan intruksi (if-than-else)
8. jika selesai intruksikan kembali (bayar=total-diskon).
9.cetak semua hasil perintah di atas (jumlah baraeng, total harga belanja, diskon yang di bertikan,harga yang harus di bayar 

** Flowchart Program**
![fl2](https://github.com/ilhamhernanda01/Praktikum04/blob/master/Flowchart2.jpeg)


**CODE PROGRAM**
```c++
#include<iostream>
using namespace std;
int main ()
{
    cout<< "Tugas Praktikum4"<< "Program Menghitung Total Belanja"<< endl;
    cout<< "=====================================================" <<endl;
    int jumlah_beli=0,total_beli=0,x,y,a;
    long int
    harga=0,harga_barang=0,total=0,bayar=0,diskon;
    cout<< "Masukan Jumlah Barang (N):"; cin>>y;
    x=1;

    while(x<=y)
    {
        cout<< "Barang Ke-"; cin>>a;
        cout<< "Masukan Banyaknya barang: "; cin>>jumlah_beli;
        cout<< "Masukan Harga Barang:Rp"; cin>>harga;
        harga_barang = harga*jumlah_beli;
        total=total + harga_barang;
        total_beli += jumlah_beli;
        x++;
    }
    if(total>=1000000)
    {
        diskon=total*10/100;
    }
    else if (total>500000&&total<1000000)
    {
        diskon=total*5/100;
    }else{
    diskon=0;
    }
    cout<< "=====================================================" <<endl;
    bayar=total-diskon;
    cout<< "Total Barang Yang Di Beli : "<<total_beli<<endl;
    cout<< "Total Semua Pembelian :Rp"<<total<<endl;
    cout<< "Mendapatkan Diskon Sebesar :Rp"<<diskon<<endl;
    cout<< "Total Yang Harus Di Bayar =Rp"<<bayar<<endl;
}

```

**HASIL**
![hasil2](https://github.com/ilhamhernanda01/Praktikum04/blob/master/hasill%20coding2.png)

**Terima Kasih**
