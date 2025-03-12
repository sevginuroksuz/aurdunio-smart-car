# 🚗 Arduino Smart Car

<p align="center">
  <img src="https://www.arduino.cc/en/uploads/Main/ArduinoUno_R3_Front_450px.jpg" width="300">
</p>

## 📌 Proje Hakkında  
Arduino Smart Car, **otonom hareket edebilen** ve **karşısına çıkan engelleri algılayarak yön değiştiren** bir robot projesidir.  
Bu proje sayesinde **temel robotik, elektronik ve programlama becerileri** geliştirilecek ve IoT uygulamalarına giriş yapılacaktır.

---

## 🎯 Proje Amacı  
✔️ Otonom hareket eden bir robot geliştirmek  
✔️ Engel algılama ve yönlendirme algoritmalarını uygulamak  
✔️ Sensörler ve motor sürücüler ile çalışmayı öğrenmek  
✔️ Arduino ve C++ ile programlama pratiği yapmak  

---

## ⚙️ Çalışma Prensibi  

### 📡 **1. Engel Algılama:**  
- **HC-SR04 Ultrasonik Sensör**, robotun önündeki mesafeyi ölçer.  
- Eğer mesafe **belirlenen eşik değerin altına düşerse**, robot yön değiştirir.  

### 🔄 **2. Karar Verme:**  
- **Mesafe uygunsa:** Robot düz ilerler.  
- **Engel varsa:** Robot sağa veya sola dönerek yoluna devam eder.  

### 🚗 **3. Hareket Kontrolü:**  
- **L298N Motor Sürücü Kartı**, motorlara gerekli komutları iletir.  
- **DC motorlar**, verilen komutlara göre robotun yönlendirilmesini sağlar.  

### 🔁 **4. Döngüsel Çalışma:**  
- Robot **çevresini sürekli tarar** ve engelleri algıladıkça yön değiştirir.  

---

## 🛠 Kullanılacak Malzemeler  

| **Parça**                             | **Açıklama**                              |
|---------------------------------------|------------------------------------------|
| 🟢 **Arduino Uno**                     | Robotun beyni, program çalıştırma       |
| 🟡 **L298N Motor Sürücü Kartı**         | Motorların hız ve yön kontrolü          |
| 🔵 **HC-SR04 Ultrasonik Sensör**       | Engel algılama ve mesafe ölçümü         |
| 🔴 **DC Motorlar & Tekerlekler**       | Robotun hareket etmesini sağlar        |
| ⚫ **6'lı AA Pil Yuvası & Li-Po Pil**   | Robotun güç kaynağı                     |
| 🟣 **Jumper Kablolar**                 | Bağlantılar için                        |
| 🟠 **LED ve Buzzer (Opsiyonel)**       | Geri bildirim sistemleri                |

---

## 📝 Yazılım ve Algoritma  

```cpp
#define trigPin 9
#define echoPin 10
#define motorA1 3
#define motorA2 5
#define motorB1 6
#define motorB2 11

void setup() {
  pinMode(trigPin, OUTPUT);
  pinMode(echoPin, INPUT);
  pinMode(motorA1, OUTPUT);
  pinMode(motorA2, OUTPUT);
  pinMode(motorB1, OUTPUT);
  pinMode(motorB2, OUTPUT);
  Serial.begin(9600);
}

void loop() {
  long duration;
  int distance;

  digitalWrite(trigPin, LOW);
  delayMicroseconds(2);
  digitalWrite(trigPin, HIGH);
  delayMicroseconds(10);
  digitalWrite(trigPin, LOW);

  duration = pulseIn(echoPin, HIGH);
  distance = duration * 0.034 / 2;

  Serial.println(distance);

  if (distance < 20) { 
    digitalWrite(motorA1, LOW);
    digitalWrite(motorA2, HIGH);
    digitalWrite(motorB1, HIGH);
    digitalWrite(motorB2, LOW);
    delay(500);
  } else {  
    digitalWrite(motorA1, HIGH);
    digitalWrite(motorA2, LOW);
    digitalWrite(motorB1, HIGH);
    digitalWrite(motorB2, LOW);
  }
}
```

---

## 🚨 Karşılaşılabilecek Problemler ve Çözümleri  

| **Problem**                             | **Çözüm**                                      |
|-----------------------------------------|----------------------------------------------|
| **❌ Sensör Hassasiyeti**               | Sensör konumu iyi ayarlanmalı, gerekirse birden fazla sensör kullanılmalı. |
| **❌ Motor Kontrol Sorunları**          | Bağlantılar doğru yapılmalı, motor sürücü kartı düzgün beslenmeli. |
| **❌ Pil Tükenme Problemi**             | Li-Po batarya veya şarj edilebilir pil kullanılmalı. |
| **❌ Engel Algılama Yanılgısı**         | Robotun sağa ve sola bakarak en uygun yolu seçmesi için kod optimize edilmeli. |

---

## 🎬 Video ve Görseller  

📸 **Robotun çalışmasını gösteren bir demo videosu eklenecek**  
🎥 **Prototip görüntüleri paylaşılacak**  

---

## 📌 Katkıda Bulunmak İster misin?  
Projeye katkıda bulunmak için:  
1. **Fork yap** 🍴  
2. **Yeni bir dal (branch) oluştur** 🌿  
3. **Geliştirmeleri yap ve commit at** 💻  
4. **Pull request gönder** 🚀  

Her türlü öneriye açığım!  

📧 **İletişim:** [sevginuroksuz@gmail.com]  

---

## 🏆 Lisans  
🔗 **Bu proje MIT Lisansı ile sunulmaktadır.**  
