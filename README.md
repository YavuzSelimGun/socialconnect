# SocialConnect – Konum Tabanlı Sosyal Etkinlik API

SocialConnect, kullanıcıların konum bazlı sosyal etkinlikler oluşturabildiği ve
etkinliklere katılabildiği bir backend API projesidir. Proje, konum verileriyle
çalışan RESTful servislerin tasarlanması ve modüler backend mimarisi üzerine
odaklanmaktadır.

Bu repository, projenin mimarisini, dosya yapısını ve kullanılan teknolojileri
göstermek amacıyla hazırlanmış bir **demo / skeleton** versiyondur.

---

## Kullanılan Teknolojiler
- Python, Django, Django REST Framework
- PostgreSQL, PostGIS
- JWT tabanlı kimlik doğrulama
- Docker & Docker Compose

---

## Mimari Yaklaşım
- Modüler Django app yapısı (`users`, `activity`, `location`)
- RESTful API mimarisi
- JWT ile stateless authentication
- PostGIS kullanılarak konum bazlı sorgular
- Docker ile izole geliştirme ortamı

---

## Uygulama Bileşenleri

### Users
- Kullanıcı kayıt ve giriş işlemleri
- JWT tabanlı kimlik doğrulama
- Kullanıcıya ait temel profil işlemleri

### Activity
- Etkinlik oluşturma ve listeleme
- Etkinlik kapasitesi ve katılım mantığı
- Kullanıcı–etkinlik ilişkileri

### Location
- Konum bazlı veri modeli
- PostGIS ile mesafe ve alan sorguları
- Etkinliklerin konuma göre filtrelenmesi

---

## Servisler
- Django backend servisi
- PostgreSQL + PostGIS veritabanı
- Docker Compose ile çoklu servis yönetimi

---

## Güvenlik ve Yapılandırma
- Ortam değişkenleri `.env` dosyası üzerinden yönetilmektedir
- Hassas bilgiler ve üretim kodları bu repository’de paylaşılmamaktadır

---

## Not
Bu repository, akademik ve kişisel projelerde geliştirilen kodların tamamını
içermemektedir. Kodlar private olarak saklanmakta olup, görüşme sürecinde
talep edilmesi halinde paylaşılabilir.
