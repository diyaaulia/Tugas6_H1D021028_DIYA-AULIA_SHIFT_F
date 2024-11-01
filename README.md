# Tugas6_H1D021028_DIYA-AULIA_SHIFT_F
# LINK/FOLDER PROJECT TERDAPAT PADA GDRIVE DIBAWAH INI
https://drive.google.com/file/d/1Q4xU6E47I1r590DNT634w4DEjEUhuU57/view?usp=drive_link
![WhatsApp Image 2024-10-31 at 22 18 01 (1)](https://github.com/user-attachments/assets/a5bedfc6-1a6d-4fdb-b20b-566c5d5fb12e)
Membuat Proyek Ionic
# 1. Jika Anda belum memiliki proyek Ionic, buatlah proyek baru dengan menjalankan perintah berikut di terminal:
ionic start nama-proyek blank
cd nama-proyek
# 2. Membuat Halaman Baru
Jika Anda ingin menambahkan komponen ke halaman baru, buatlah halaman dengan perintah:
ionic generate page NamaHalaman
Ini akan membuat folder baru di dalam direktori src/app yang berisi file-file yang diperlukan untuk halaman tersebut.
# 3. Menambahkan Komponen
Ionic memiliki banyak komponen UI yang siap digunakan. Untuk menambahkannya ke halaman Anda, ikuti langkah berikut:
Buka File HTML Halaman: Buka file HTML dari halaman yang ingin Anda tambahkan komponen, misalnya nama-halaman.page.html.
Tambahkan Komponen: Tambahkan tag komponen yang ingin Anda gunakan. Misalnya, jika Anda ingin menambahkan tombol dan kartu, Anda dapat menulis:
<ion-header>
  <ion-toolbar>
    <ion-title>Judul Halaman</ion-title>
  </ion-toolbar>
</ion-header>

<ion-content>
  <ion-card>
    <ion-card-header>
      <ion-card-title>Judul Kartu</ion-card-title>
    </ion-card-header>
    <ion-card-content>
      Ini adalah konten dari kartu.
      <ion-button expand="full">Klik Saya</ion-button>
    </ion-card-content>
  </ion-card>
</ion-content>

# 4. Menambahkan Logika (Opsional)
Jika komponen Anda memerlukan logika, buka file TypeScript terkait, misalnya nama-halaman.page.ts. Anda bisa menambahkan metode atau properti sesuai kebutuhan:
import { Component } from '@angular/core';
@Component({
  selector: 'app-nama-halaman',
  templateUrl: './nama-halaman.page.html',
  styleUrls: ['./nama-halaman.page.scss'],
})
export class NamaHalamanPage {

  constructor() { }

  onButtonClick() {
    console.log('Tombol diklik!');
  }
}
Kemudian, Anda bisa menghubungkan metode ini dengan tombol di HTML:
<ion-button expand="full" (click)="onButtonClick()">Klik Saya</ion-button>

# 5. Mengimpor Modul (Jika Diperlukan)
Jika Anda menggunakan komponen yang memerlukan modul tambahan (seperti IonicModule), pastikan untuk mengimpor modul tersebut di dalam app.module.ts atau modul yang sesuai.
# 6. Menjalankan Proyek
Setelah semua selesai, jalankan proyek Anda untuk melihat hasilnya:
ionic serve
Buka browser dan arahkan ke http://localhost:8100 untuk melihat halaman Anda.

