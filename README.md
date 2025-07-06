## 👥 Takım Üyeleri

- **Şevval Nesibe Arslan**: Scrum Master
- **Melih Tuna İpek**: Developer  
- **Emirhan Arslan**: Product Owner

--- 

## 📌 ÜRÜN AÇIKLAMASI  
**Diyabet Dostu**, diyabet riski taşıyan veya diyabetle yaşayan bireylerin günlük yaşamlarında daha sağlıklı tercihler yapmalarına yardımcı olan, belirtilere dayalı kişisel öneriler sunan bir web platformudur.

Kullanıcılar, siteye giriş yaparak günlük ruh hali, yaşadığı belirtiler ve beslenme tercihleri gibi kısa bilgileri paylaşır. Diyabet Dostu bu verileri analiz ederek, kullanıcıya basit ama etkili yönlendirmeler sunar.  
Örneğin:  
- “Baş dönmesi yaşıyorsan su tüketimini artırmalısın.”  
- “Tatlı isteğin fazlaysa bu insülin dalgalanması olabilir.”  

**Diyabet Dostu**, tıbbi bir teşhis aracı değildir. Amaç; farkındalık kazandırmak, kullanıcıyı bilinçlendirmek ve gerektiğinde bir uzmana yönlendirmektir.  
Web üzerinden erişilebilmesi sayesinde hem mobil hem masaüstü cihazlarda kolaylıkla kullanılabilir. Basit ve sade arayüzü, özellikle yaşlı bireyler için erişilebilirlik sunar.

---

## ⚙ ÜRÜN ÖZELLİKLERİ

### 1. 🧭 Belirti Girişi ve Analiz
- Kullanıcılar, web sitesi üzerinden günlük belirtilerini (örneğin halsizlik, titreme, baş ağrısı) işaretler.
- Sistem, bu belirtilere göre olası riskleri analiz eder.
- Gerekli durumlarda kullanıcı, bir uzmana danışması yönünde uyarılır.

### 2. 🍞 Beslenme Öneri Modülü
- Kullanıcının verilerine göre hangi gıdalardan kaçınması gerektiği önerilir.
- Alternatif sağlıklı alışkanlıklar ve besin önerileri sunulur.
- Örnek: “Beyaz ekmeği azalt, tam tahıllı ürünleri tercih et.”

### 3. 📊 Kişisel Takip Paneli
- Kullanıcı geçmiş günlerdeki belirti girişlerini ve sistemin sunduğu önerileri görebilir.
- Basit grafiklerle zaman içindeki gelişim gözlemlenebilir.

### 4. 🔒 Gizlilik ve Kolay Erişim
- Kullanıcı girişi isteğe bağlıdır.
- Kişisel veriler saklanmaz, herhangi bir dış sunucuya gönderilmez.
- Tüm kullanım deneyimi sade, büyük fontlarla ve anlaşılır tasarımla sunulur.

### 5. 🧠 Hikâyeleştirme Modülü (Opsiyonel)
- Gelişmiş sürümde kullanıcı verilerine dayalı eğlenceli sağlık hikâyeleri sunulur.
- Amaç: Kullanıcıyı motive etmek ve sağlık davranışlarını eğlenceli bir şekilde pekiştirmek.

### 6. 🗓 Haftalık Sağlık Planlayıcı
- Kullanıcı kendi hedeflerini belirleyebilir (örneğin “günde 8 bardak su”, “haftada 3 yürüyüş”).
- Bu hedeflere ne kadar uyduğu basit görsellerle sunulur.

### 7. 💬 Bilgi Merkezi
- Diyabet hakkında temel bilgiler: Nedir, belirtileri nelerdir, ne zaman tehlikeye işaret eder?
- SSS (Sık Sorulan Sorular) bölümü.
- “Bugünkü bilgini test et” gibi mini etkileşimli testler.

### 8. 📣 Hatırlatmalar ve Geri Bildirimler
- Siteyi düzenli ziyaret eden kullanıcılar için küçük uyarılar:  
  - “Bugün kendini nasıl hissediyorsun?”  
  - “Üst üste 3 gündür halsizlik bildirildi. Bir sağlık uzmanına danışmayı düşün.”

---

## 🎯 **Hedef Kitle:**

- Tip 2 diyabet riski taşıyan bireyler  
- Diyabet geçmişi olan bireylerin aile üyeleri  
- Sağlık hizmetine erişimi sınırlı bölgelerde yaşayanlar  
- Yaşlı bireyler veya teknolojiyle arası iyi olmayan kullanıcılar  
- Sağlıklı yaşam alışkanlıkları edinmek isteyen bireyler  
- İlk kez diyabet tanısı almış ve rehberliğe ihtiyaç duyan kullanıcılar  

---

## 💡 **Gelecek Geliştirmeler:**

- Cihaz bağlantılı glikozmetre desteği (Bluetooth entegresiyle)  
- WhatsApp üzerinden günlük sağlık raporu gönderimi  
- Diyetisyen ve doktor destekli içerikler  
- Kullanıcılar arası destek topluluğu / sosyal forum  
- Sağlık kuruluşlarıyla iş birlikleri

---

## 🧩 Teknik Bileşenler
🖥 HTML & CSS
Basit ve koyu temalı bir kullanıcı arayüzü tasarlanmıştır.

Ana bileşenler:

Sohbet alanı (#chat)

Metin giriş kutusu ve “Gönder” butonu

Mesaj renkleri:

Kullanıcı mesajları → yeşil

Bot yanıtları → mavi

🧠 JavaScript
Kullanıcıdan gelen mesajı fetch() fonksiyonu ile http://localhost:8000/predict adresine JSON formatında gönderir.

API'den gelen bot cevabı sohbet alanına eklenir.

Enter tuşu ile mesaj gönderimi desteklenmektedir.

🔄 Çalışma Akışı
👤 Kullanıcı metin kutusuna bir mesaj yazar.

📤 Mesaj, JSON formatında sunucuya (backend) gönderilir.

🧠 Backend (yapay zekâ) bu mesaja yanıt üretir.

📥 Gelen yanıt, “Bot:” etiketiyle ekranda gösterilir.

---

## 🔄 Takım Backlog ve Süreç Yönetimi

📋 Miro üzerinden güncel proje backlog ve görev panomuza aşağıdan ulaşabilirsiniz:

➡️ [AI Team 123 Miro Backlog Board](https://miro.com/app/board/uXjVIhfZIGA=/?share_link_id=374145866072)  

---

## 🚀 Sprint 1
🎯 Sprint Hedefi
Sprint içinde tamamlanması tahmin edilen puan: 100 Puan

Toplam Backlog: 360 Puan
Proje sürecimiz 3 Sprint'e ayrılmıştır. Bu nedenle ilk Sprint'e en az 100 puan ile başlanması uygun görülmüştür.

## 🧩 Kod Örneği: JS ile API Entegrasyonu
Kullanıcının mesajını alıp Flask API’ye gönderen JavaScript kodunun terminal çıktısı veya editör görünümü.

![WhatsApp Görsel 2025-07-06 saat 13 53 10_14aedfa9](https://github.com/user-attachments/assets/6a705c21-cb73-4279-aa7a-297d04d675fc)

![WhatsApp Görsel 2025-07-06 saat 13 53 27_76827289](https://github.com/user-attachments/assets/e2e160ee-580c-4015-8853-50e178a2d5ba)

![WhatsApp Görsel 2025-07-06 saat 13 53 52_0781fe13](https://github.com/user-attachments/assets/7d3ffeb4-6792-4884-b2e4-b26b5563249c)

## 📋 Sprint Backlog (Miro)
Sprint 1 boyunca planlanan görevlerin yer aldığı backlog tablosunun ekran görüntüsü.

![Ekran görüntüsü 2025-07-06 192657](https://github.com/user-attachments/assets/0e8005d8-2f8a-4f88-bdba-32b60d213f3d)

## ✅ Daily Scrum Örneği
Sprint 1 süresince yapılan yazılı-sesli günlük takım değerlendirmesi örneği.

![WhatsApp Görsel 2025-07-06 saat 19 56 41_d8344b06](https://github.com/user-attachments/assets/fbff8c11-fea2-4743-b753-5d1725652056)


![WhatsApp Görsel 2025-07-06 saat 13 20 31_2f64832a](https://github.com/user-attachments/assets/ec681503-d6f0-4dfe-ad84-f08903d42dbb)

