# Oneri Raporu

## 1. Proje Konusu
Arduino Smart Car, **otonom hareket edebilen** ve **karşısına çıkan engelleri algılayarak yön değiştiren** bir robot projesidir. Bu proje, **temel robotik, elektronik ve programlama becerileri** kazandırmayı hedefler ve IoT (Nesnelerin İnterneti) uygulamalarına giriş yapmak için iyi bir fırsattır. Proje, Arduino Uno kartı ile entegre edilen sensörler ve motor sürücüler kullanarak otonom hareket etmesini sağlar.

---

## 2. Proje Hedefleri
- **Otonom hareket eden bir robot geliştirmek:** Robot, çevresindeki engelleri algılayarak yön değiştirebilecek.
- **Engel algılama ve yönlendirme algoritmalarını uygulamak:** Robot, HC-SR04 ultrasonik sensörleri ile çevresini sürekli tarar ve mesafeye göre yön değiştirir.
- **Sensörler ve motor sürücüler ile çalışmayı öğrenmek:** Proje, robotik sistemlerde kullanılan temel sensörler ve motor sürücülerle çalışma pratiği kazandırır.
- **Arduino ve C++ ile programlama pratiği yapmak:** Proje, Arduino IDE kullanarak programlama becerilerini geliştirmeye yönelik bir fırsat sunar.

---

## 3. Tahmini Zaman Çizelgesi
| **Görev**                                        | **Tahmini Süre**  |
|--------------------------------------------------|-------------------|
| **Proje Planlaması ve Araştırma**                | 1 hafta           |
| **Arduino ve Sensörlerin Kurulumu**              | 1 hafta           |
| **Yazılım Geliştirme ve Engel Algılama Algoritması** | 2 hafta           |
| **Donanım Montajı ve Testler**                   | 2 hafta           |
| **Yazılım ve Donanım Entegrasyonu**              | 2 hafta           |
| **Test ve Hata Ayıklama**                        | 1 hafta           |
| **Son Testler ve Optimizasyon**                  | 1 hafta           |
| **Proje Sonuçları ve Rapor Hazırlama**           | 1 hafta           |
| **Toplam Süre**                                  | 9 hafta           |

---

## 4. Kaynak Planlaması

### **Proje Ekibi:**
- **Sevgi Nur Öksüz (Proje Yöneticisi):** Proje takibini yapacak, genel yönlendirme ve raporlama.
- **Buse Yıldız (Teknik Sorumlu):** Arduino ve sensörlerin kurulumu, yazılım geliştirme ve algoritmaların oluşturulmasından sorumlu kişi.
- **Aybüke Erarslan (Donanım Uzmanı):** Elektronik bileşenlerin montajı ve test edilmesinden sorumlu kişi.
- **Onur Kerem (Yazılım Geliştirici):** C++ ile programlama, algoritmaların yazılması ve sensör/motor kontrol yazılımlarının geliştirilmesinden sorumlu kişi.

---

### **Kullanılacak Ekipmanlar:**

| **Parça**                          | **Açıklama**                                |
|------------------------------------|--------------------------------------------|
| 🟢 **Arduino Uno**                  | Robotun beyni, program çalıştırma ve sensör motor kontrolü |
| 🟡 **L298N Motor Sürücü Kartı**     | Motorların hız ve yön kontrolü            |
| 🔵 **HC-SR04 Ultrasonik Sensör**    | Engel algılama ve mesafe ölçümü           |
| 🔴 **DC Motorlar & Tekerlekler**    | Robotun hareket etmesini sağlar           |
| ⚫ **6'lı AA Pil Yuvası & Li-Po Pil**| Robotun güç kaynağı                       |
| 🟣 **Jumper Kablolar**              | Bağlantılar için                          |
| 🟠 **LED ve Buzzer (Opsiyonel)**    | Geri bildirim sistemleri                  |

---

### **Kullanılacak Yazılımlar:**

- **Arduino IDE:** Arduino kartının programlanması için kullanılan yazılım.
- **C++:** Proje kodlaması için kullanılan programlama dili.

---

### **Proje Maliyeti:**

| **Ekipman**                        | **Yaklaşık Maliyet (USD)**                 |
|------------------------------------|--------------------------------------------|
| 🟢 **Arduino Uno**                  | 10 USD                                     |
| 🟡 **L298N Motor Sürücü Kartı**     | 5 USD                                      |
| 🔵 **HC-SR04 Ultrasonik Sensör**    | 3 USD                                      |
| 🔴 **DC Motorlar & Tekerlekler**    | 10 USD                                     |
| ⚫ **6'lı AA Pil Yuvası & Li-Po Pil**| 8 USD                                      |
| 🟣 **Jumper Kablolar (set)**       | 2 USD                                      |
| 🟠 **LED ve Buzzer (Opsiyonel)**    | 2 USD                                      |
| **Toplam**                         | **40 USD**                                 |

**Not:** Maliyetler yaklaşık değerlerdir ve kullanılan tedarikçilere göre değişebilir. Ayrıca, bazı ekipmanlar (örneğin, Arduino Uno) birden fazla projede kullanılabilir, bu nedenle toplam maliyet birden fazla proje için paylaşılabilir.

---

## 5. Risk Analizi

| **Problem**                             | **Çözüm**                                      |
|-----------------------------------------|----------------------------------------------|
| **❌ Sensör Hassasiyeti**               | Sensör konumu iyi ayarlanmalı, gerekirse birden fazla sensör kullanılmalı. |
| **❌ Motor Kontrol Sorunları**          | Bağlantılar doğru yapılmalı, motor sürücü kartı düzgün beslenmeli. |
| **❌ Pil Tükenme Problemi**             | Li-Po batarya veya şarj edilebilir pil kullanılmalı. |
| **❌ Engel Algılama Yanılgısı**         | Robotun sağa ve sola bakarak en uygun yolu seçmesi için kod optimize edilmeli. |

---

## 6. Ticari Potansiyel
Bu proje, özellikle **eğitim** ve **robotik uygulamalar** alanlarında ticari potansiyele sahip olabilir. Ayrıca, **IoT uygulamaları** için uygun bir temel oluşturur. Otonom robotlar, özellikle eğitim sektöründe, robotik kurslar ve workshop'lar için kullanılabilir. Ayrıca, lojistik ve depo otomasyonu gibi alanlarda daha gelişmiş versiyonlarıyla ticari kullanım potansiyeli bulunabilir.

---

