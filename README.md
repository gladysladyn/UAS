# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Gladys Lady Nathasha
<br>NIM		:	1227050052
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Matriks adalah susunan bilangan-bilangan berbentuk persegi panjang yang diatur dalam baris atau kolom dengan dibatasi kurung. Bilangan yang tersusun dalam matriks disebut elemen/unsur matriks. Baris adalah susunan bilangan-bilangan yang mendatar (horizontal), sedangkan kolom adalah susunan bilangan-bilangan yang tegak (vertikal). Ordo matriks adalah banyaknya elemen baris dan banyaknya elemen kolom dari suatu matriks. Jika sebuah matriks memiliki i baris dan j kolom, maka matriks tersebut berordo i x j, dapat dituliskan Ai.j.
Transpose suatu matriks, misal matriks A, yang dilambangkan dengan At adalah sebuah matriks yang disusun dengan cara menukarkan baris matriks A menjadi kolom matriks At dan kolom matriks A menjadi baris matriks At.
Operasi modulus adalah sebuah operasi yang menghasilkan sisa pembagian dari suatu bilangan terhadap bilangan lainnya. Dalam bahasa pemrograman operasi ini umumnya dilambangkan dengan simbol %, mod atau modulo, tergantung bahasa pemrograman yang digunakan.

## Source Code
#include <iostream>

using namespace std;

int main(){
	int i, j, a, b, matriks[10][10], transpose[10][10];

	cout << "Masukkan jumlah baris matriks: ";
	cin >> a;
	cout << "Masukkan jumlah kolom matriks: ";
	cin >> b;

	cout << "Masukkan nilai matriks\n";
	cout << "(tekan spasi untuk kolom selanjutnya dan tekan enter untuk baris selanjutnya)\n";
	for (i = 0; i < a; i++){
		for (j = 0; j < b; j++){
    		cin >> matriks[i][j];
    	}
	}

	for (i = 0; i < a; i++){
    	for (j = 0; j < b; j++){
    		transpose[j][i] = matriks[i][j];
    	}
	}

	cout << "Hasil Transpose Matriks: \n";
	for (i = 0; i < b; i++){
    	for (j = 0; j < a; j++){
    	cout << transpose[i][j] << "\t";
    	}
    cout << endl;
	}
}
  
  

#include <iostream>
#include <iomanip>

using namespace std;

int main(){
    int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

    cout<<"Input jumlah baris: "; cin>>jumlahBaris;
    cout<<"Input jumlah kolom: "; cin>>jumlahKolom;
    cout << endl;

    for(i = 0; i < jumlahBaris; i++){
        for(j = 0; j < jumlahKolom; j++){
            cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
            cin >> arr[i][j];
        }
        cout << endl;
    }

	cout << "Hasil: " << endl;

    for(i = 0; i < jumlahBaris ; i++){
        for(j = 0; j < jumlahKolom; j++){
            cout << setw(3) << arr[i][j] << " ";
        }
        cout << endl;
    }

    cout << "\nBilangan yang habis dibagi 3: " << endl;
    for(i = 0; i < jumlahBaris ; i++){
        for(j = 0; j < jumlahKolom; j++){
            if(arr[i][j] % 3 == 0){
                cout << arr[i][j] << " ";
            }
        }
        cout << endl;
    }

    cout << "\nBilangan yang habis dibagi 5: " << endl;
    for(i = 0; i < jumlahBaris ; i++){
        for(j = 0; j < jumlahKolom; j++){
            if(arr[i][j] % 5 == 0){
                cout << arr[i][j] << " ";
            }
        }
        cout << endl;
    }

    cout << "\nBilangan yang habis dibagi 7: " << endl;
    for(i = 0; i < jumlahBaris ; i++){
        for(j = 0; j < jumlahKolom; j++){
            if(arr[i][j] % 7 == 0){
                cout << arr[i][j] << " ";
            }
        }
        cout << endl;
    }
    
    cout << endl;
    return 0;
}

	
	
## Output
Masukkan jumlah baris matriks: 2
Masukkan jumlah kolom matriks: 2
Masukkan nilai matriks
(tekan spasi untuk kolom selanjutnya dan tekan enter untuk baris selanjutnya)
2  4

3  6
Hasil Transpose Matriks:
2       3
4       6

--------------------------------
Process exited after 10.15 seconds with return value 0
Press any key to continue . . .
  
  
Input jumlah baris: 3
Input jumlah kolom: 3

Baris 1, kolom 1 = 2
Baris 1, kolom 2 = 4
Baris 1, kolom 3 = 6

Baris 2, kolom 1 = 3
Baris 2, kolom 2 = 6
Baris 2, kolom 3 = 9

Baris 3, kolom 1 = 4
Baris 3, kolom 2 = 7
Baris 3, kolom 3 = 14

Hasil:
  2   4   6
  3   6   9
  4   7  14

Bilangan yang habis dibagi 3:
6
3 6 9


Bilangan yang habis dibagi 5:




Bilangan yang habis dibagi 7:


7 14
 

--------------------------------
Process exited after 13.48 seconds with return value 0
Press any key to continue . . .
