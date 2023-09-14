# kumpulan-code-algoritma-dan-pemrograman-2

izin menjawab bu

/******************************************************************************

                              Online C++ Compiler.
               Code, Compile, Run and Debug C++ program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

// Online C++ compiler to run C++ program online
#include <iostream>
using namespace std;

struct Mahasiswa {
    string Name;
    int NIM;
    int Nilai[3];
};

int main() {
    float angka, total = 0, rata;
    int jumlahNilai;
    string grade;
    Mahasiswa mahasiswa;
    
    cout<<"Masukan nama mahasiswa :";
    cin>>mahasiswa.Name;
    cout<<"Masukan NIM mahasiswa :";
    cin>>mahasiswa.NIM;
    cout<<"Masukan Nilai Algoritma :";
    cin>>mahasiswa.Nilai[0];
    cout<<"Masukan Nilai Kalkulus :";
    cin>>mahasiswa.Nilai[2];
    cout<<"Masukan Nilai Struktur Data :";
    cin>>mahasiswa.Nilai[1];
    
    jumlahNilai = end(mahasiswa.Nilai)-begin(mahasiswa.Nilai);
    
    for (int i = 0; i < jumlahNilai; i++){
        total += mahasiswa.Nilai[i];
    }
    
    rata = total / jumlahNilai;
    
    if (rata >= 80){
        grade = "A";
    } else if (rata >= 70 && rata < 79) {
        grade = "B"; 
    } else if (rata >= 60 && rata < 69){
        grade = "C";
    } else if (rata >= 50 && rata < 59) {
        grade = "D";
    } else {
        grade = "E";
    }
    
    cout<<"\n==================\n";
    cout<<"Nama :"<<mahasiswa.Name<<"\n";
    cout<<"NIM :"<<mahasiswa.NIM<<"\n";
    cout<<"Nilai Algoritma : "<<mahasiswa.Nilai[0]<<"\n";
    cout<<"Nilai Kalkulus : "<<mahasiswa.Nilai[1]<<"\n";
    cout<<"Nilai Struktur Data :"<<mahasiswa.Nilai[2]<<"\n";
    cout<<"Total Nilai : "<<total<<"\n";
    cout<<"Rata - Rata : "<<rata<<"\n";
    cout<<"Grade : "<<grade;
    
    
    return 0;
}
