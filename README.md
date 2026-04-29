# Kawien AI: Intelligent Note Pro
### *Ultra Cognitive Dashboard & Microservice Ecosystem*

**Kawien AI: Intelligent Note Pro**, geleneksel not alma sürecini bir bilişsel davranış analiz aracına dönüştürmek için tasarlanmış, mikroservis tabanlı son teknoloji bir ekosistemdir. Platform, kullanıcı düşünce kalıplarını değerlendirmek ve gerçek zamanlı bilişsel içgörüler sağlamak için deterministik bir yapay zeka motoru kullanır.

<img width="1911" height="915" alt="image" src="https://github.com/user-attachments/assets/aea5529c-118a-43f2-9dc4-f537013cb394" />


---

##  Projeye Genel Bakış (Project Overview)
Bu proje; **Docker** ile orkestra edilen, **JWT** ile güvenliği sağlanan ve **GitHub Actions** üzerinden sağlam bir **CI/CD** hattı ile otomatikleştirilen yüksek performanslı bir mikroservis yığınını (stack) uygular. 

Öne çıkan özelliği, kullanıcı verilerini analiz ederek beyin baskınlığını ve hafıza metriklerini belirleyen **"Bilişsel Zeka Paneli" (Cognitive Intelligence Dashboard)**'dir.

---

##  Temel Özellikler (Key Features)

*   **Bilişsel Yapay Zeka Motoru:** Tutma (Retention), Detay (Detail) ve Hız (Speed) puanlarını hesaplamak için kullanıcı girdilerini analiz eder.
*   **Beyin Baskınlık Analizi:** Dinamik SVG filtreleri kullanarak "Sol Beyin" ve "Sağ Beyin" eğilimlerini görselleştirir.
*   **Mikroservis Mimarisi:** Kimlik Doğrulama (Auth), Not Yönetimi (Note Management) ve Bildirimler (Notifications) için birbirinden bağımsız servisler.
*   **Asenkron İletişim:** Yüksek verimli e-posta teslimatı ve servisler arası iletişim için **HTTPX** kullanımı.
*   **Modern Arayüz:** Chart.js ve Plus Jakarta Sans fontu ile oluşturulmuş, modern ve "glassmorphic" Dashboard tasarımı.

---

##  Teknik Mimari ve Altyapı
Sistem, katmanlar arasında sorumlulukların net ayrılmasını sağlayan **Clean Architecture** modelini takip eder:

![Technical Architecture](https://github.com/user-attachments/assets/50e5b269-cfe9-4016-a608-cdd8bdbea458)

1.  **API Katmanı (FastAPI):** İstek yönlendirme, Pydantic doğrulama ve kimlik doğrulama işlemlerini yönetir.
2.  **Çekirdek Mantık (Service Layer):** İş kurallarını ve AI bilişsel puanlama algoritmasını yürütür.
3.  **Veritabanı Katmanı (SQLAlchemy):** PostgreSQL/SQLite ile verilerin kalıcı olarak depolanmasını sağlar.
4.  **Gateway (Nginx):** Ters ana sunucu (reverse proxy) görevi görerek servisler arasındaki trafiği yönetir.

![System Flow](https://github.com/user-attachments/assets/e9126675-78fa-429d-94fa-6d0d27f05c80)
![DB Schema](https://github.com/user-attachments/assets/f9e17e9e-c0be-4492-a810-22c4bb7ce70d)

---

## Yapay Zeka Sistemi (AI System Definition)
<img width="1642" height="906" alt="image" src="https://github.com/user-attachments/assets/05d8859b-5489-42a8-ab5b-63e7aedfc01d" />


Sistemimizdeki bilişsel analizler şu akademik temellere dayanmaktadır:
*   **Mueller, P. A., & Oppenheimer, D. M. (2014):** Not alma biçimlerinin bilişsel etkisi.
*   **Tulving, E., et al. (1994):** Epizodik bellekte hemisferik kodlama/geri çağırma asimetrisi.
*   **Rathod et al. (2016):** Beyin fonksiyonları üzerindeki nörolojik içgörüler.

---

## 🛠️ Gelişmiş Özellikler

### 1. Tam CI/CD Hattı
GitHub Actions kullanılarak profesyonel bir boru hattı kurulmuştur. Her "push" işlemi şunları tetikler:
*   **Ortam Kurulumu:** Sanal ortam ve bağımlılıkların yüklenmesi.
*   **Linting & Formatting:** Kod kalitesi kontrolleri.
*   **Otomatik Testler:** Test paketinin yürütülmesi.
*   **Konteyner Derleme:** Docker imajlarının doğrulanması.

### 2. Otomatik Testler
Sistem, AI Mantık Motorunu ve API uç noktalarını (endpoints) doğrulayan birim testleri içerir. Bu, puanlama algoritmasının her güncellemede doğru kalmasını sağlar.

### 3. Konteyner Orkestrasyonu
Tüm yapı Docker ile konteynerize edilmiştir. **Docker Compose** ile yönetilen bu yapı, servislerin izole edildiği ve birbirine güvenli ağlarla bağlandığı "bulut benzeri" bir ortam sağlar.

---

## 🏁 Başlarken (Getting Started)

### Ön Koşullar
*   Docker & Docker Compose yüklü olmalıdır.

### Kurulum
Terminalinizi açın ve proje klasöründe şu komutu çalıştırın:
```bash
docker-compose up --build
