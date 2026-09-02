<div align="center">

# ⚡ Menu-Matik // NEXT-GEN QR ECOSYSTEM

### *Sıfır Sunucu. Sıfır Veritabanı. Sıfır Aylık Maliyet. Sonsuz Hız.*

<br/>

[![Live Deployment](https://img.shields.io/badge/PRODUCTION-menu--matik.vercel.app-e11d48?style=for-the-badge&logo=vercel&logoColor=white)](https://menu-matik.vercel.app/)
[![Architecture](https://img.shields.io/badge/ARCHITECTURE-100%25%20CLIENT--SIDE-0284c7?style=for-the-badge&logo=codewars&logoColor=white)](#-mimari-manifesto)
[![Payload Compression](https://img.shields.io/badge/DATA_ENGINE-MICRO--PAYLOAD%20v2-10b981?style=for-the-badge&logo=speedtest&logoColor=white)](#-mühendislik-detayları)
[![License](https://img.shields.io/badge/LICENSE-MIT%20ENTERPRISE-8b5cf6?style=for-the-badge)](LICENSE)

<br/>

```
      __  __ _____ _   _ _   _      __  __    _  _____ ___ _  __
     |  \/  | ____| \ | | | | |    |  \/  |  / \|_   _|_ _| |/ /
     | |\/| |  _| |  \| | | | |____| |\/| | / _ \ | |  | || ' / 
     | |  | | |___| |\  | |_| |____| |  | |/ ___ \| |  | || . \ 
     |_|  |_|_____|_| \_|\___/     |_|  |_/_/   \_|_| |___|_|\_\
                                                            
               -- ZERO-INFRASTRUCTURE DIGITAL MENU ENGINE --
```

<p align="center">
  <b>Geleneksel, hantal ve fahiş SaaS aboneliklerini unutun.</b><br/>
  menu-matik; modern web teknolojilerini kullanarak kafe ve restoranların tüm menü altyapısını doğrudan URL hash katmanına sıkıştıran, yüksek performanslı bir dijital vitrin mimarisidir.
</p>

[🌐 Canlı Deneyimle](https://menu-matik.vercel.app/) • [🚀 Özellikler](#-temel-yetenekler) • [🧠 Mimari](#-mimari-manifesto) • [👨‍💻 İletişim](#-mimar--sistem-tasarımı)

---

</div>

<br/>

## 💎 Neden Farklı? (Problem / Çözüm Paradigması)

| Geleneksel QR Menü Sistemleri | ⚡ menu-matik Mimarisi |
| :--- | :--- |
| **Aylık 500-1500 TL SaaS Aidatı** | **%100 Ömür Boyu Ücretsiz & Sunucusuz (Zero Infra)** |
| **40 MB Ağır ve Açılmayan PDF Dosyaları** | **< 15 KB Ultra Hafif, App-Like Native Arayüz** |
| **Veritabanı Çökmesi = Masada Menüsüzlük** | **Merkeziyetsiz; Veri Doğrudan URL İçinde Yaşar** |
| **Abonelik Bittiğinde Kilitlenen QR Kodlar** | **Kalıcı; Masaya Basılan QR Kod Asla Ölmez** |

---

## 🚀 Temel Yetenekler

* 📦 **Micro-Payload Veri Sıkıştırma Motoru:** 30 farklı ürün, kategori ve fiyat verisi; özel sözdizimi algoritması ile **< 400 baytlık** mikroskobik bir parametreye dönüştürülür.
* ✏️ **Gerçek Zamanlı Yerinde (Inline) Editör:** Menü ürünlerini silip baştan yazmaya gerek kalmadan, tablo üzerinde milisaniyeler içinde isim ve fiyat revizyonu.
* 🖨️ **Baskıya Hazır Ultra-HD PNG Dışa Aktarımı:** Matbaa standartlarında ($600 \times 700$ Canvas render), kurumsal çerçeveli, logo ve masa yönlendirmeli vektörel QR çıktısı.
* 📱 **Tam Reaktif & Cihaz Bağımsız:** iOS Safari, Android Chrome ve masaüstü tarayıcılarda piksel şaşması yaşatmayan CSS Grid / Flexbox iskeleti.
* 🎯 **Entegre Lead-Generation Modülü:** Hem yönetici hem son kullanıcı ekranında yüksek dönüşümlü danışmanlık ve portföy temas noktaları.

---

## 🧠 Mimari Yapı: Veri Nasıl Havada Taşınır?

Sistem, geleneksel bir REST API veya SQL/NoSQL veritabanı yerine **tarayıcı belleği ve URL fragment identifier (`#`)** mekanizmasını bir veri depolama birimi gibi kullanır:

```text
┌─────────────────────────────────────────────────────────────┐
│                   YÖNETİCİ ARAYÜZÜ (STATE)                  │
│       [Kaşarlı Tost: 120]  [Flat White: 115]  ...           │
└──────────────────────────────┬──────────────────────────────┘
                               │
                               ▼
        ┌──────────────────────────────────────────────┐
        │        MICRO-PAYLOAD PARSER ENGINE           │
        │  t=Kadıköy;y=Tost:120,Kruvasan:165;i=...     │
        └──────────────────────┬───────────────────────┘
                               │
            ┌──────────────────┴──────────────────┐
            ▼                                     ▼
┌───────────────────────┐             ┌───────────────────────┐
│ REED-SOLOMON QR MATRIX│             │   VERCEL HASH ROUTER  │
│  (Pure JS Canvas)     │             │ https://.../#m=[DATA] │
└───────────┬───────────┘             └───────────┬───────────┘
            │                                     │
            ▼                                     ▼
┌───────────────────────┐             ┌───────────────────────┐
│ 600x700 PNG MATBAA    │             │ MÜŞTERİ MOBİL EKRANI  │
│   BASKI ŞABLONU       │             │   (Zero-Lag Render)   │
└───────────────────────┘             └───────────────────────┘
```

---

## ⚡ Hızlı Başlangıç

Projeyi yerel ortamınızda çalıştırmak için derleme aracına (Node, npm, Webpack) ihtiyaç yoktur. Saf web teknolojileri ile inşa edilmiştir.

```bash
# 1. Repoyu klonlayın
git clone [https://github.com/batuhanbayatli/menu-matik.git](https://github.com/batuhanbayatli/menu-matik.git)

# 2. Proje dizinine gidin
cd menu-matik

# 3. index.html dosyasını herhangi bir modern tarayıcıda açın
open index.html # macOS
start index.html # Windows
```

---

## 🛠️ Teknoloji Yığını

* **Core:** HTML5 Semantic Engine, CSS3 Modern Flex/Grid Layout
* **Typography:** Plus Jakarta Sans & JetBrains Mono
* **Icons:** FontAwesome v6.4 Enterprise Icons
* **QR Compiler:** QRious Low-Footprint Reed-Solomon Generator
* **Deployment:** Vercel Edge Network

---

## 👨‍💻 Mimar & Sistem Tasarımı

<div align="center">

### **Batuhan Bayatlı**
*FinTech, InsurTech & Enterprise Web Systems Architect*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect%20Professionally-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/batuhanbayatlı)
[![Portfolio](https://img.shields.io/badge/bGroup-Venture%20Ecosystem-e11d48?style=for-the-badge&logo=safari&logoColor=white)](https://www.linkedin.com/in/batuhanbayatlı)

<br/>

> *"En karmaşık kurumsal problemleri, sıfır maliyetli ve ölçeklenebilir saf mühendislik modelleriyle çözüyoruz."*

</div>

---

## 📜 Lisans

Bu proje [MIT Lisansı](LICENSE) kapsamında korunmaktadır. Ticari ve bireysel kullanıma tamamen açıktır.
