# 🎮 Arduino #18: LCD Ekran ile Engel Atlama Oyunu

Bu projede, **Arduino** ve **16x2 karakter LCD ekran** kullanarak basit bir **engel atlama oyunu** geliştirildi.  
Karakter, engellerden zıplayarak kaçınmalı ve puan toplamalıdır. Oyun butonla kontrol edilir.

🔗 [Web Siteme Bakmak İçin Tıkla](https://www.hakkiharmankaya.com/)  
🔗 [Tinkercad Tasarımına Göz At](https://www.tinkercad.com/things/cQbTRXnn0sB?sharecode=BsTOxH4q_9zp4RaQgbngYIdJX9BsrBeD3bvVL_sY7Uw)

---

## 🧰 Gerekli Malzemeler

- 1 adet **Arduino**
- 1 adet **potansiyometre**
- 1 adet **10kΩ direnç**
- 1 adet **16x2 LCD ekran**
- 1 adet **buton**
- 1 adet **330Ω direnç**
- **Jumper kabloları**
- **Breadboard**

---

## 🔧 Devre Kurulumu

### 📺 LCD Ekran Bağlantıları

| LCD Pin | Arduino Pin     |
|---------|-----------------|
| 1 (GND) | GND             |
| 2 (VCC) | 5V              |
| 3 (VO)  | Potansiyometre orta bacak |
| 4 (RS)  | D8              |
| 5 (RW)  | GND             |
| 6 (EN)  | D9              |
| 11 (D4) | D10             |
| 12 (D5) | D11             |
| 13 (D6) | D12             |
| 14 (D7) | D13             |
| 15 (LED+) | 5V           |
| 16 (LED-) | GND           |

### 🔘 Buton Bağlantısı

- Buton → 330Ω direnç → **D7 pinine**
- Diğer bacak → **GND**

---

## 🕹️ Oyun Özeti

- **Butona basıldığında** karakter zıplar.
- Engeller karaktere çarparsa oyun biter.
- Sürekli koşu animasyonu vardır.
- Üst satır ve alt satır engellerle dolabilir.
- Sağ üst köşede **puan** gösterilir.

---

## 💻 Arduino Kodları

Kod oldukça detaylı olduğu için bu dosyaya eklendi:  


Kod içeriğinde;

- Özel karakter tanımları
- Oyun başlatma/yeniden başlatma sistemi
- Terrain kaydırma sistemi
- Zıplama animasyonu
- Çarpışma kontrolü
- Skor hesaplama

... gibi tüm mekanikler yer almaktadır.

---

## 🧪 Tinkercad Simülasyonu

Devreyi Tinkercad üzerinde de test edebilirsiniz:  
🔗 [Tinkercad Tasarımına Göz At](https://www.tinkercad.com/things/cQbTRXnn0sB?sharecode=BsTOxH4q_9zp4RaQgbngYIdJX9BsrBeD3bvVL_sY7Uw)

---

## 📌 Notlar

- Oyun mantığı sprite tabanlıdır.
- Karakterin hareketi LCD’nin özel karakter kapasitesi ile sağlanır.
- Skor 99999'a kadar artar.
- Kod oldukça kapsamlıdır ve oyun mantığı örnekleri için idealdir.

---

## 📄 Lisans

Bu proje, eğitim ve eğlence amaçlı serbestçe kullanılabilir.

---
