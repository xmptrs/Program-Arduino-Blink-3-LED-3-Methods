# Program-Arduino-Blink-3-LED-3-Methods
ini adalah program untuk menjalankan perintah blink 3 led dengan 3 metode

Cara pemakaian

1.salin kode yang berada di bawah

2.lalu tempel kode ke kolom arduino droid

dan kode sudah bisa di compile dan di gunakan.

Tanpa Fungsi

```
const int ledMerah = 2;
const int ledKuning = 3;
const int ledHijau = 4;

void setup() {
  pinMode(ledMerah, OUTPUT);
  pinMode(ledKuning, OUTPUT);
  pinMode(ledHijau, OUTPUT);
}

void loop() {
  // === LED MERAH BERKEDIP 5 KALI ===
  // Kedip 1
  digitalWrite(ledMerah, HIGH); delay(400);
  digitalWrite(ledMerah, LOW); delay(400);
  // Kedip 2
  digitalWrite(ledMerah, HIGH); delay(400);
  digitalWrite(ledMerah, LOW); delay(400);
  // Kedip 3
  digitalWrite(ledMerah, HIGH); delay(400);
  digitalWrite(ledMerah, LOW); delay(400);
  // Kedip 4
  digitalWrite(ledMerah, HIGH); delay(400);
  digitalWrite(ledMerah, LOW); delay(400);
  // Kedip 5
  digitalWrite(ledMerah, HIGH); delay(400);
  digitalWrite(ledMerah, LOW); delay(400);

  delay(500); // Jeda sebelum ganti warna

  // === LED HIJAU BERKEDIP 3 KALI ===
  // Kedip 1
  digitalWrite(ledHijau, HIGH); delay(400);
  digitalWrite(ledHijau, LOW); delay(400);
  // Kedip 2
  digitalWrite(ledHijau, HIGH); delay(400);
  digitalWrite(ledHijau, LOW); delay(400);
  // Kedip 3
  digitalWrite(ledHijau, HIGH); delay(400);
  digitalWrite(ledHijau, LOW); delay(400);

  delay(500); // Jeda sebelum ganti warna

  // === LED KUNING BERKEDIP 2 KALI ===
  // Kedip 1
  digitalWrite(ledKuning, HIGH); delay(400);
  digitalWrite(ledKuning, LOW); delay(400);
  // Kedip 2
  digitalWrite(ledKuning, HIGH); delay(400);
  digitalWrite(ledKuning, LOW); delay(400);

  delay(500); // Jeda sebelum ganti warna
}
```

Dengan Fungsi For

```
const int ledMerah = 2;
const int ledKuning = 3;
const int ledHijau = 4;

void setup() {
  pinMode(ledMerah, OUTPUT);
  pinMode(ledKuning, OUTPUT);
  pinMode(ledHijau, OUTPUT);
}

void loop() {
  // LED Merah berkedip 5 kali
  for (int i = 0; i < 5; i++) {
    digitalWrite(ledMerah, HIGH);
    delay(400);
    digitalWrite(ledMerah, LOW);
    delay(400);
  }
  delay(500);

  // LED Hijau berkedip 3 kali
  for (int i = 0; i < 3; i++) {
    digitalWrite(ledHijau, HIGH);
    delay(400);
    digitalWrite(ledHijau, LOW);
    delay(400);
  }
  delay(500);

  // LED Kuning berkedip 2 kali
  for (int i = 0; i < 2; i++) {
    digitalWrite(ledKuning, HIGH);
    delay(400);
    digitalWrite(ledKuning, LOW);
    delay(400);
  }
  delay(500);
}
```

Dengan Fungsi While
```
const int ledMerah = 2;
const int ledKuning = 3;
const int ledHijau = 4;

void setup() {
  pinMode(ledMerah, OUTPUT);
  pinMode(ledKuning, OUTPUT);
  pinMode(ledHijau, OUTPUT);
}

void loop() {
  // LED Merah berkedip 5 kali
  int i = 0;
  while (i < 5) {
    digitalWrite(ledMerah, HIGH);
    delay(400);
    digitalWrite(ledMerah, LOW);
    delay(400);
    i++;
  }
  delay(500); // Jeda sebelum ganti warna

  // LED Hijau berkedip 3 kali
  int j = 0;
  while (j < 3) {
    digitalWrite(ledHijau, HIGH);
    delay(400);
    digitalWrite(ledHijau, LOW);
    delay(400);
    j++;
  }
  delay(500); // Jeda sebelum ganti warna

  // LED Kuning berkedip 2 kali
  int k = 0;
  while (k < 2) {
    digitalWrite(ledKuning, HIGH);
    delay(400);
    digitalWrite(ledKuning, LOW);
    delay(400);
    k++;
  }
  delay(500); // Jeda sebelum ganti warna
}
```

Dengan Fungsi Parameter

```
//LOOPING DENGAN FUNGSI
int merah = 2;
int kuning = 3;
int hijau = 4; 

void setup ()
{
  pinMode(merah, OUTPUT);
  pinMode(kuning, OUTPUT);
  pinMode(hijau, OUTPUT);
} 

void loop ()
{
   blink(1, 5, merah, 2000) ; 
   blink(1, 3, kuning, 1000) ; 
   blink(1,2 , hijau, 500) ;   
} 

void blink (int nilaiawal, int nilaiakhir,int led, int lama)
{
  for (int  i =  nilaiawal; i <=nilaiakhir; i ++)
   {
     digitalWrite (led, HIGH) ;
    delay (lama);
    digitalWrite (led, LOW) ;
    delay (lama);
  }
 }
```

Silahkan Gunakan Variabel dan Pin yang sesuai dengan yang anda gunakan..
