# 🚗 <span style="color:#ff5733;">Engelden Kaçan Robot</span>

## 🎯 <span style="color:#33ff57;">Proje Amacı</span>
Bu proje, **otonom hareket eden**, **engelleri algılayarak yön değiştiren** bir robotun tasarlanmasını ve geliştirilmesini amaçlamaktadır. 

Robot, **ultrasonik sensörler** kullanarak çevresini algılar ve uygun manevraları gerçekleştirerek yoluna devam eder.

---

## ⚙️ <span style="color:#3399ff;">Projenin Çalışma Prensibi</span>
💡 **HC-SR04 ultrasonik sensör** ile çevresini tarayan robot, belirlenen mesafe eşiğinin altına düşüldüğünde **Arduino** tarafından yönlendirilerek **motor sürücü** ile hareket ettirilir.

🛠 **Çalışma Adımları:**
1. Sensörden gelen mesafe verisi okunur.
2. Engel algılandığında yön değiştirme kararı alınır.
3. Motor sürücüye komut gönderilir.
4. Robot yeni rotasında hareketine devam eder.

---

## 🔧 <span style="color:#ffcc00;">Kullanılacak Malzemeler</span>

✔️ <span style="color:#ff5733;">Arduino Uno</span> *(Beyin)*  
✔️ <span style="color:#33ff57;">L298N Motor Sürücü Kartı</span> *(Motor kontrolü için)*  
✔️ <span style="color:#3399ff;">HC-SR04 Ultrasonik Mesafe Sensörü</span> *(Engel algılama için)*  
✔️ **6'lı AA Pil Yuvası & Li-Po Pil** *(Güç kaynağı)*  
✔️ **DC Motorlar & Tekerlekler** *(Hareket sistemi)*  
✔️ **LED ve Buzzer (Opsiyonel)** *(Geri bildirim için)*  

---

## 🚨 <span style="color:#ff3333;">Karşılaşılabilecek Problemler ve Çözümleri</span>

### ⚠️ Sensör Hassasiyeti
❌ **Yanlış ölçüm hataları olabilir.**  
✅ **Sensör konumu iyi ayarlanmalı, gerekirse birden fazla sensör kullanılmalıdır.**

### ⚠️ Motor Kontrol Problemleri
❌ **Düzensiz hareket olabilir.**  
✅ **Bağlantılar kontrol edilmeli ve uygun güç kaynağı kullanılmalıdır.**

### ⚠️ Güç Tüketimi
❌ **Bataryalar hızlı tükenebilir.**  
✅ **Enerji tasarrufu için bekleme modu kullanılabilir.**

---

📌 <span style="color:#ff9900;">Bu proje, robotik ve programlama alanında pratik yapmak için harika bir fırsattır!</span> 🚀
