# Dotnet Store - E-Ticaret Uygulaması

Bu proje, ASP.NET Core MVC mimarisi kullanılarak geliştirilmiş, modern ve kapsamlı bir e-ticaret platformudur. Kullanıcı yönetimi, ürün kataloglama, sepet yönetimi ve ödeme entegrasyonu gibi temel e-ticaret özelliklerini barındırır.

## 🚀 Özellikler

- **Kullanıcı Yönetimi:** ASP.NET Core Identity ile kayıt, giriş, rol yönetimi (Admin/User) ve yetkilendirme.
- **Ürün ve Kategori Yönetimi:** Ürünlerin kategorilere göre listelenmesi ve detaylı ürün görünümü.
- **Sepet Sistemi:** Dinamik sepet yönetimi ve ürün ekleme/çıkarma işlemleri.
- **E-posta Servisi:** Smtp tabanlı e-posta gönderim desteği.
- **Güvenlik:** Şifre politikaları, hesap kilitleme ve güvenli çerez (cookie) yönetimi.
- **Veri Seeding:** Uygulama ilk çalıştığında otomatik olarak örnek verilerin (ürünler, kategoriler) yüklenmesi.

## 🛠️ Teknolojiler

- **Backend:** ASP.NET Core MVC (.NET 8+)
- **ORM:** Entity Framework Core
- **Database:** MS SQL Server
- **Authentication:** ASP.NET Core Identity
- **Frontend:** Bootstrap, Razor Pages, View Components
- **Tools:** Dependency Injection, Repository Pattern

## 📦 Kurulum

### 1. Veritabanı Yapılandırması
`appsettings.json` dosyasındaki `ConnectionStrings` bölümüne kendi SQL Server bağlantı dizinizi ekleyin:

```json
"ConnectionStrings": {
  "DefaultConnection": "Server=YOUR_SERVER;Database=DotnetStoreDb;Trusted_Connection=True;TrustServerCertificate=True;"
}
```

### 2. Migration Uygulama
Veritabanı tablolarını oluşturmak için Package Manager Console üzerinden şu komutu çalıştırın:

```bash
Update-Database
```

### 3. Çalıştırma
Projeyi Visual Studio veya CLI üzerinden başlatın:

```bash
dotnet run
```

## 📂 Proje Yapısı

- `Controllers/`: Uygulama mantığı ve yönlendirmeler.
- `Models/`: Veri modelleri ve DataContext.
- `Views/`: Kullanıcı arayüzü (Razor).
- `Services/`: Sepet ve E-posta gibi yardımcı servisler.
- `ViewComponents/`: Tekrar kullanılabilir arayüz bileşenleri.
- `wwwroot/`: CSS, JS ve resim dosyaları.

## 📝 Lisans
Bu proje eğitim amaçlı geliştirilmiştir.
