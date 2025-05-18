# 🧾 T.C. Kimlik Doğrulama Servisi (SOAP - Node.js)

Bu proje, Türkiye Cumhuriyeti vatandaşlarına ait kimlik bilgilerini doğrulamak için **Node.js** kullanılarak geliştirilmiş bir SOA (Service-Oriented Architecture) servisidir.

Servis, [T.C. Kimlik Doğrulama Web Servisi](https://tckimlik.nvi.gov.tr/service/kpspublic.asmx) (SOAP) üzerinden veri alarak, girilen bilgilerin doğruluğunu kontrol eder.

---

## 🚀 Uygulamayı Çalıştırma

### Gereksinimler
- Node.js (v18 veya üzeri önerilir)
- VSCode
- Terminal / Komut satırı

### Başlatma Adımları

1. 📁 Proje klasörüne geçin:

   ```bash
   cd SOA_PROJE
   
2. Gerekli bağımlılıkları yükleyin:
   ```bash
   npm install

3. Servisi başlatın:
   ```bash
   npm start

## 📡 API Kullanımı

1. Endpoint:
   ```bash
   POST http://localhost:3000/validate

2. Gönderilecek JSON Body:
   ```bash
   {
    "tcNo": "XXXXXXXXXXX",
    "firstName": "Name",
    "lastName": "Surname",
    "birthYear": 0000
   }

## 📌 Notlar

- Bu servis, **Nüfus ve Vatandaşlık İşleri Genel Müdürlüğü (NVİ)**’nin resmi SOAP servisine bağlanarak kimlik doğrulama işlemi yapar.
- Doğrulama işlemi için **gerçek T.C. kimlik bilgileri** kullanılmalıdır.
- Servis, yalnızca **eğitim**, **demo** ve **entegrasyon testleri** amacıyla geliştirilmiştir.
- Uygulama **yalnızca localhost üzerinde çalışır**, dış ağlara açık değildir.
