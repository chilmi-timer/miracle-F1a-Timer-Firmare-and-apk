Firmware (hex) ada 3 macam:
1. Untuk timer hijau 2 servo
2. Untuk timer hijau 4 servo
3. Untuk timer biru the simpel (arduino pro mini)


Note:
Timer anda mungkin memiliki pin mapping yang sedikit berbeda dengan fw terbaru sehingga perlu sedikit penyesuaian (soldering). Misalkan buzzer di timer lama ada di pin 10, dan di fw baru ada di pin 9. Maka buzzer tidak bunyi sampai pinnya di pindah.


Bagi pengguna timer 2 servo yang menginginkan servo wing dan hook, bisa solder sendiri di pin 5 (wing) dan 6(hook)


Berikut saya lampirkan pin mapping masing2:


// pin mapping untuk Hijau 4 servo lgtfx...............................................................................
  buzzer = 9;
  hook_sw = 8;
  bunt_sw = 7;
  DT_pin = 2;
  stab_pin =3;
  rud_pin = 4;
  wing_pin = 5;
  hook_pin = 6;
  led_pin =11;
  profile_pin = A4;
  batt_pin = A2;
  batt_pin2 = A3;
  


// pin mapping untuk  hijau 2 servo lgtfx minievb;........................................
  buzzer = A0;
  hook_sw = 10;
  bunt_sw = 11;
  DT_pin = 2;
  stab_pin =3;
  rud_pin = 4;
  wing_pin = 5;
  hook_pin = 8;
  led_pin =12;
  profile_pin = 9;
  batt_pin = A3;
  batt_pin2 = A2;


CHANGE LOG 
4.0 :
1. add live hook ( seting glide time menit dengan hook, satu beep = 1 menit, tahan hook kedepan lalu nyalakan timer, hitung beep lalu lepaskan hook)
2. apk: read menggunakan pembacaan kode spesifik mencegah data yang acak2an di tabel, bat voll untuk 2s, ACceleration timeout dan mode goto, servo mapping (user input to micros),
4.1:
   Fw: bug fix( posisi servo during bailout/ setelah acctimeout), suara buzzer during acc, 
