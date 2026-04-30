#  Intelligent Note Pro
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
<img width="817" height="350" alt="image" src="https://github.com/user-attachments/assets/2019561c-0115-434f-81be-39ca6546d84b" />

<img width="407" height="562" alt="image" src="https://github.com/user-attachments/assets/475c6eac-5a3d-456b-b329-5362d6f84873" />


---

##  Teknik Mimari ve Altyapı
Sistem, katmanlar arasında sorumlulukların net ayrılmasını sağlayan **Clean Architecture** modelini takip eder:

![Technical Architecture](https://github.com/user-attachments/assets/50e5b269-cfe9-4016-a608-cdd8bdbea458)

1.  **API Katmanı (FastAPI):** İstek yönlendirme, Pydantic doğrulama ve kimlik doğrulama işlemlerini yönetir.
2.  **Çekirdek Mantık (Service Layer):** İş kurallarını ve AI bilişsel puanlama algoritmasını yürütür.
3.  **Veritabanı Katmanı (SQLAlchemy):** PostgreSQL/SQLite ile verilerin kalıcı olarak depolanmasını sağlar.
4.  **Gateway (Nginx):** Ters ana sunucu (reverse proxy) görevi görerek servisler arasındaki trafiği yönetir.

![System Flow](https://github.com/user-attachments/assets/e9126675-78fa-429d-94fa-6d0d27f05c80)


---

## Yapay Zeka Sistemi (AI System Definition)
<img width="1642" height="906" alt="image" src="https://github.com/user-attachments/assets/05d8859b-5489-42a8-ab5b-63e7aedfc01d" />


Sistemimizdeki bilişsel analizler şu akademik temellere dayanmaktadır:
*   **Mueller, P. A., & Oppenheimer, D. M. (2014):** Not alma biçimlerinin bilişsel etkisi.
*   **Tulving, E., et al. (1994):** Epizodik bellekte hemisferik kodlama/geri çağırma asimetrisi.
*   **Rathod et al. (2016):** Beyin fonksiyonları üzerindeki nörolojik içgörüler.
<img width="811" height="346" alt="image" src="https://github.com/user-attachments/assets/6316a2fb-f527-44ba-9344-8a5c423cf325" />

---

## 🛠️ Gelişmiş Özellikler

### 1. Tam CI/CD Hattı
GitHub Actions kullanılarak profesyonel bir boru hattı kurulmuştur. Her "push" işlemi şunları tetikler:
*   **Ortam Kurulumu:** Sanal ortam ve bağımlılıkların yüklenmesi.
*   **Linting & Formatting:** Kod kalitesi kontrolleri.
*   **Otomatik Testler:** Test paketinin yürütülmesi.
*   **Konteyner Derleme:** Docker imajlarının doğrulanması.
    <img width="1882" height="773" alt="image" src="https://github.com/user-attachments/assets/38349cee-7a0b-4456-9fc6-27b3836b919e" />


<img width="797" height="428" alt="image" src="https://github.com/user-attachments/assets/2c429e9a-3d60-4a6c-838a-e750cf5478e9" />


### 2. Otomatik Testler
Sistem, AI Mantık Motorunu ve API uç noktalarını (endpoints) doğrulayan birim testleri içerir. Bu, puanlama algoritmasının her güncellemede doğru kalmasını sağlar.
<img width="765" height="316" alt="image" src="https://github.com/user-attachments/assets/08ef17a1-4257-4056-869c-4fc2166b4483" />

### 3. Konteyner Orkestrasyonu
Tüm yapı Docker ile konteynerize edilmiştir. **Docker Compose** ile yönetilen bu yapı, servislerin izole edildiği ve birbirine güvenli ağlarla bağlandığı "bulut benzeri" bir ortam sağlar.

<img width="1168" height="655" alt="image" src="https://github.com/user-attachments/assets/7087249d-9f9f-478f-aca8-5eede166c6f4" />




<img width="1918" height="770" alt="image" src="https://github.com/user-attachments/assets/9137e41b-cacb-4c46-b7db-3c5de374d4ad" />

---
##  Kullanılan Programlar & Diller
DOCKER
PGADMIN
PYTHON
HTML 
SQL 

##  Başlarken (Getting Started)

### Ön Koşullar
*   Docker & Docker Compose yüklü olmalıdır.

### Kurulum
Terminalinizi açın ve proje klasöründe şu komutu çalıştırın:
```bash
docker-compose up --build
