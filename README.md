# 📱 Menu-Matik // Akıllı ve Sıfır Maliyetli QR Menü Motoru

> Kafe, restoran ve butik işletmeler için veritabanı, sunucu veya aylık abonelik maliyeti gerektirmeyen **%100 istemci taraflı (Client-Side)** dijital QR menü mimarisi.

[![Live Demo](https://img.shields.io/badge/Canlı%20Sürüm-menu--matik.vercel.app-e11d48?style=for-the-badge&logo=vercel)](https://menu-matik.vercel.app/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Pure Vanilla](https://img.shields.io/badge/Stack-HTML5%20%7C%20CSS3%20%7C%20Vanilla%20JS-f59e0b?style=for-the-badge)](https://developer.mozilla.org/)

---

## 🎯 Projenin Amacı ve Çözülen Problem

Geleneksel QR menü sistemleri işletmeleri **yüksek aylık SaaS aboneliklerine**, **hantal PDF dosyalarına** veya masadaki QR kodların bozulmasına yol açan dinamik yönlendirme tuzaklarına mahkum eder. 

**menu-matik**, bu darboğazı aşmak için geliştirilmiş akıllı bir mikro-mimari örneğidir:
1. **Sıfır Sunucu & Sıfır Veritabanı Maliyeti:** Tüm menü verisi istemci tarafında sıkıştırılarak URL hash (`#m=...`) bileşenine aktarılır.
2. **Kalıcı Masabaşı QR Kod:** Masalara basılan QR kodlar hiçbir zaman abonelik bitişi nedeniyle kapanmaz; link kendi içinde veriyi taşır.
3. **App-Like Pürüzsüz Mobil Deneyim:** Müşteri kamerayla okuttuğu anda milisaniyeler içinde reaktif, hafif ve temiz bir mobil menüyle karşılaşır.

---

## ✨ Öne Çıkan Özellikler

* ⚡ **Ultra Hafif Veri Sıkıştırma (Micro-Payload):** Ürün isim ve fiyatları URI bileşenlerine zarar vermeyen kompakt bir formatta paketlenir; QR kodun fiziksel veri yoğunluğu minimize edilerek her kameranın anında okuması sağlanır.
* ✏️ **Yerinde (Inline) Düzenleme:** Yönetici panelinde ürün adı veya fiyatı silmeye gerek kalmadan tek tıkla yerinde revize edilebilir.
* 🖨️ **Matbaaya Hazır PNG İndirici:** Üretilen QR kod; işletme adı, hizalama çerçevesi ve çağrı metniyle birlikte tek tıkla 600x700 yüksek çözünürlüklü baskı formatında indirilebilir.
* 📦 **Kategori Kotaları (Freemium Model):** Yiyecek, İçecek ve Tatlı kategorileri için 10'ar ürünlük kota kontrolü.
* 📢 **Entegre Müşteri Kazanım (Lead-Gen) Kuşağı:** Menülerin ve yönetim panelinin altına stratejik olarak entegre edilmiş kurumsal danışmanlık ve portföy kartları.

---

## 🛠️ Teknik Mimari & Çalışma Mantığı

```text
[İşletme / Admin Paneli] 
         │
         ├──> Form Verisi (İsim, Fiyat, Kategori)
         ├──> Kompakt Payload Üretimi (t=...;y=...;i=...;d=...)
         ├──> Canvas Üzerinde Reed-Solomon QR Çizimi (QRious)
         └──> Matbaaya Hazır Yüksek Çözünürlüklü PNG Dışa Aktarımı
         
[Masadaki Müşteri]
         │
         ├──> QR Kod Okutma (Kamera)
         ├──> [https://menu-matik.vercel.app/#m=](https://menu-matik.vercel.app/#m=)[PAYLOAD]
         ├──> Hash Çözücü (Client-Side Parser)
         └──> Minimalist & Reaktif Mobil Menü Görünümü
```

---

## 🚀 Canlı Önizleme & Kurulum

Sistem herhangi bir harici paket veya derleme adımı (npm, node, backend) gerektirmez.

1. Repoyu klonlayın:
```bash
git clone [https://github.com/batuhanbayatli/menu-matik.git](https://github.com/batuhanbayatli/menu-matik.git)
```
2. `index.html` dosyasını doğrudan tarayıcınızda açın veya Vercel / GitHub Pages üzerinde yayınlayın.

Canlı uygulamayı doğrudan deneyimlemek için:  
👉 **[menu-matik.vercel.app](https://menu-matik.vercel.app/)**

---

## 👨‍💻 Mimar & Geliştirici

**Batuhan Bayatlı**  
*FinTech, InsurTech ve Kurumsal Web Sistemleri Mimarı*

* 🌐 **LinkedIn:** [linkedin.com/in/batuhanbayatlı](https://www.linkedin.com/in/batuhanbayatlı)

---

## 📄 Lisans

Bu proje [MIT Lisansı](LICENSE) altında açık kaynak olarak sunulmaktadır.
