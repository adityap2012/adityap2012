#include <iostream>

using namespace std;

int main() {
    string nama;
    int golongan, jamKerja;
    int upah, lembur, totalGaji;

    cout << "Masukkan nama karyawan : ";
    cin >> nama;

    cout << "Masukkan golongan kerja (2 atau 3) : ";
    cin >> golongan;

    cout << "Masukkan jam kerja (lebih dari 48 jam) : ";
    cin >> jamKerja;

    if (golongan == 2) {
        upah = 35000;
    }
    else if (golongan == 3) {
        upah = 50000;
    }

    if (jamKerja > 48) {
        lembur = (jamKerja - 48) * 10000;
    }
    else {
        lembur = 0;
    }

    totalGaji = upah + lembur;

    cout << "Nama Karyawan : " << nama << "\n";
    cout << "Golongan Kerja : " << golongan << "\n";
    cout << "Jam Kerja : " << jamKerja << " jam" << "\n";
    cout << "Gaji Bersih : Rp " << totalGaji << ",-" << "\n";


}
