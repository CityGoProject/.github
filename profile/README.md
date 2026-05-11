<div align="center">

# CityGo

### Akıllı Ulaşım ve Rezervasyon Sistemi

[![Java](https://img.shields.io/badge/Java-17-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)](https://openjdk.org/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.2.5-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)](https://spring.io/projects/spring-boot)
[![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![H2 Database](https://img.shields.io/badge/H2-Database-0000BB?style=for-the-badge)](https://www.h2database.com/)

Farklı ulaşım türlerini tek bir platformda birleştiren, Java ve React tabanlı full-stack bilet rezervasyon uygulaması.

[Proje Reposu](https://github.com/CityGoProject/CityGo) · [README](https://github.com/CityGoProject/CityGo#readme) · [Kurulum](https://github.com/CityGoProject/CityGo#-başlarken)

</div>

---

## Proje Hakkında

**CityGo**, CENG106 Nesne Yönelimli Programlama dersi kapsamında geliştirilen bir akıllı ulaşım ve rezervasyon sistemidir. Kullanıcılar uçak, tren ve otobüs seferlerini arayabilir, görsel koltuk haritası üzerinden koltuk seçebilir, bilet satın alabilir ve biletlerini yönetebilir.

Yönetici kullanıcılar ise admin paneli üzerinden seferleri, ulaşım araçlarını, kullanıcıları, biletleri ve dışa aktarma işlemlerini yönetebilir.

---

## Öne Çıkan Özellikler

| Alan | Özellikler |
|------|------------|
| Kullanıcı Yönetimi | Kayıt, giriş, rol bazlı kullanıcı ayrımı, güvenli şifre saklama |
| Sefer Arama | Kalkış, varış, tarih ve araç tipine göre filtreleme |
| Rezervasyon | Görsel koltuk seçimi, bilet alma, bilet iptali |
| Admin Paneli | Sefer CRUD, kullanıcı/bilet listesi, istatistikler |
| Veri Dışa Aktarma | Bilet verilerini JSON ve CSV formatında indirme |
| OOP Tasarımı | Kalıtım, kapsülleme, soyutlama, polymorphism ve exception handling |

---

## Teknoloji Yığını

| Katman | Teknolojiler |
|--------|--------------|
| Backend | Java 17, Spring Boot, Spring Data JPA, Maven |
| Frontend | React, Vite, Material UI, React Router, Axios |
| Veritabanı | H2 Database, dosya tabanlı kalıcı geliştirme verisi |
| Mimari | REST API, katmanlı mimari, DTO tabanlı istek/cevap yapısı |
| Kalite | Merkezi hata yönetimi, validasyon, unit testler |

---

## OOP Odaklı Tasarım

CityGo yalnızca çalışan bir web uygulaması değil, aynı zamanda OOP prensiplerini gerçek bir senaryoda uygulayan bir ders projesidir.

- **Kalıtım:** `Kullanici -> Yolcu/Admin`, `UlasimAraci -> Ucak/Tren/Otobus`
- **Soyutlama:** Abstract sınıflar ve `IRezervasyon`, `IAranabilir`, `IExportable` interface'leri
- **Çok Biçimlilik:** Araç türlerine göre farklı fiyat hesaplama ve overloaded arama metotları
- **Kapsülleme:** Entity alanlarının private tutulması, kontrollü getter/setter erişimi
- **Exception Handling:** Özel exception sınıfları ve merkezi `GlobalExceptionHandler`

---

## Ekip

| İsim | Sorumluluk Alanı |
|------|------------------|
| Mustafa Mert Çevik | Ulaşım araçları, sefer modeli, arama API'si |
| Muhammed Köseoğlu | Proje altyapısı, kullanıcı sistemi, auth API, admin panel altyapısı |
| Ömer Faruk Kara | Frontend geliştirme, kullanıcı akışı, dışa aktarma modülü |
| Elif Feyza Şengül | Rezervasyon sistemi, bilet yönetimi, hata yönetimi |

---

## Hızlı Başlangıç

```bash
# Backend
cd backend
mvn clean install
mvn spring-boot:run

# Frontend
cd frontend
npm install
npm run dev
```

Varsayılan adresler:

- Backend: `http://localhost:8080`
- Frontend: `http://localhost:5173`
- H2 Console: `http://localhost:8080/h2-console`

Ayrıntılı kurulum ve kullanım için ana proje README dosyasını inceleyin:

**https://github.com/CityGoProject/CityGo#readme**
