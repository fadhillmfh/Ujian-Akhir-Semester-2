# Ujian-Akhir-Semester-2
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Muhammad Fadhiil Hidayatullah
<br>NIM		:	1227050087
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
matriks adalah susunan bilangan, simbol, atau ekspresi yang disusun dalam baris dan kolom sehingga membentuk suatu bangun persegi. Program ini dibuat untuk mensortir bilangan yang ada pada matriks yang bisa habis dibagi dengan 3,5,7 atau bisa disebut dengan modulus 3,5,dan 7.

## Source Code
#include <iostream>
#include <iomanip>
using namespace std;
int main(){
    
	int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

    cout<<" Input jumlah baris: "; 
	cin>>jumlahBaris;
    cout<<" Input jumlah kolom: "; 
	cin>>jumlahKolom;
    cout << endl;

    for(i = 0; i < jumlahBaris; i++){
        for(j = 0; j < jumlahKolom; j++){
            cout << " Baris " <<i+1<<", Kolom "<<j+1<< " = ";
            cin >> arr[i][j];
        }
        cout << endl;
    }

    cout << " Hasil input nilai : " << endl;

    for(i = 0; i < jumlahBaris ; i++){
    for(j = 0; j < jumlahKolom; j++){
        cout << setw(3) << arr[i][j] << " ";
    }
    cout << endl;
    }

    cout << " Hasil bilangan yang habis dibagi 3,5,7 : " << endl;

    for(i = 0; i < jumlahBaris ; i++){
    for(j = 0; j < jumlahKolom; j++){
        if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
        cout << setw(3) << arr[i][j] << " ";
        }
    }
    cout << endl;
    }
	cout<<endl;
}
## Output
<img width="960" alt="image" src="https://user-images.githubusercontent.com/121006802/209503342-c091661c-8cb9-4af9-a6dc-7110ad89ec41.png">
