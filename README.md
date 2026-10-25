# Program-Arduino-Blink-3-LED-3-Methods
ini adalah program untuk menjalankan perintah blink 3 led dengan 3 metode

Cara pemakaian
1.salin kode yang berada di bawah
2.lalu tempel kode ke kolom arduino droid
dan kode sudah bisa di compile dan di gunakan.

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
}```