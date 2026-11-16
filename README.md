# flixora_films
Streaming platform
# Flixora

Netflix benzeri bir film ve dizi izleme deneyimi sunan, kendi içerik kütüphanenizi yönetebileceğiniz web tabanlı bir uygulama.

## 🎯 Ne Yapıyor?

- Film ve dizileri kategorilere göre listeleme (tür, yıl, popülerlik)
- Kapak görseli, özet, oyuncu kadrosu ve fragman bilgisi gösterimi
- Arama ve filtreleme (tür, yıl, puan)
- "İzleme Listem" özelliği (favorilere ekleme)
- Basit yönetim paneli ile içerik ekleme, düzenleme ve silme
- Kullanıcı girişi (e-posta + şifre)
- Duyarlı (responsive) tasarım — mobil ve masaüstünde çalışır

## 🛠️ Kullanılan Teknolojiler

- **Ön yüz:** React (Vite ile)
- **Arka yüz:** Node.js + Express
- **Veritabanı:** SQLite (geliştirme), PostgreSQL (üretim)
- **Kimlik doğrulama:** JWT (JSON Web Token)
- **Stil:** Tailwind CSS
- **API:** RESTful

## 🚀 Nasıl Çalıştırılır?

### Gereksinimler
- Node.js 18 veya üzeri
- npm veya yarn
- Git

### Kurulum
```bash
# Depoyu klonlayın
git clone https://github.com/kullaniciadi/flixora.git
cd flixora

# Bağımlılıkları yükleyin
npm install

# Ortam değişkenlerini ayarlayın
cp .env.example .env
# .env dosyasını açıp aşağıdaki değerleri doldurun:
# DATABASE_URL=...
# JWT_SECRET=...
# PORT=3000

# Veritabanını oluşturun ve başlangıç verilerini yükleyin
npm run migrate
npm run seed

# Geliştirme sunucusunu başlatın
npm run dev
