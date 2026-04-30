#  Intelligent Note Pro
### *Ultra Cognitive Dashboard & Microservice Ecosystem*

## Executive Summary

Bu projeye başlamadan önce, ders gereksinimlerini (Clean Architecture, Containerization, CI/CD vb.) en iyi karşılayacak senaryoyu belirlemek için kısa bir araştırma yaptık. Araştırmamız sonucunda, bir Not Yönetim Sistemi ilk bakışta basit görünse de, arka planda karmaşık bir mikroservis mimarisi kurmak, veritabanı ilişkilerini yönetmek ve üzerine “Akıllı Analiz” katmanları eklemek için oldukça uygun olduğunu fark ettik. Tasarım fikrimiz araştırma projemizden esinlenmiştir, ancak tüm kod ve tasarım bize aittir. Tasarım kısmı için HTML kullandık. Container yapısı için Docker kullandık. Backend tarafında Python ile Visual Studio Code kullanarak temiz bir mimari oluşturduk. Veritabanı tarafında ise proje kapsamında belirlenen tabloları oluşturmak için SQLite kullandık. Sistemimiz ayrıca kullanıcıların not oluşturmasına ve notlara aciliyet seviyesi atamasına olanak tanır. Bunun yanında, önemli notları öne çıkaran yapay zekâ destekli akıllı sıralama sistemi tasarladık.



## Product Description and Vision
PROBLEM
Günlük akademik ve profesyonel yaşamda, görevleri ve notları düzenleme ve yönetme konusunda sıkça problemler yaşanmaktadır. Çoğu zaman kritik bilgiler, kağıt notlar, düz metin dosyaları veya önceliklendirme özelliği olmayan basit uygulamalarda dağınık şekilde tutulur. Bu durum, son teslim tarihlerini ve acil görevleri kaçırmaya neden olabilir ve zaman yönetimini olumsuz etkiler.

Geleneksel not alma yöntemlerinde, kullanıcılar yapılandırılmış bilgi saklama, aciliyet seviyeleri ve akıllı önceliklendirme gibi imkanlara sahip değildir. Bilgi miktarı arttıkça, kullanıcılar neyin kritik olup olmadığını ayırt etmekte zorlanabilir.

Bununla birlikte, bazı modern sistemler sağlık veya verimlilik önerileri sunmaya çalışsa da, bu tür önerilerin her kullanıcı için %100 doğru ve geçerli olamayacağı unutulmamalıdır. Her bireyin fiziksel ve psikolojik durumu farklı olduğu için, bu öneriler kesin doğrular olarak değil, destekleyici nitelikte değerlendirilmelidir. Bu nedenle, akademik ve bilimsel çalışmalar esas alınmalı ve bu tür özellikler %100 onaylanmış çözümler olarak kabul edilmemelidir.

## Solution: Smart Notes Application
Projemiz, bu önemli probleme akıllı bir not uygulaması geliştirerek basit ve etkili bir çözüm sunmaktadır. Bu uygulama, kullanıcıların notlarını yapılandırılmış bir şekilde saklaması ve yönetmesi için merkezi bir platform sağlar.

Uygulama, kullanıcılara her nota bir aciliyet seviyesi atama imkanı sunarak önceliklerini net bir şekilde belirlemelerine yardımcı olur. Ayrıca, yapay zekâ tabanlı akıllı sıralama özelliği sayesinde en kritik notlar listenin en üstünde gösterilir.

Bunun yanı sıra, sistem yapay zekâ tabanlı önerilerin (verimlilik veya sağlık gibi) kesin kararlar olmadığının bilinciyle tasarlanmıştır. Sistem %100 doğruluk iddiasında bulunmaz, aksine kullanıcıların daha bilinçli kararlar almasına yardımcı olmayı hedefler.

Uygulama, backend geliştirme için Python, veri depolama için SQLite kullanmaktadır. Docker ise containerization için kullanılarak uygulamanın farklı ortamlarda tutarlı bir şekilde çalışmasını sağlar. Genel olarak sistem, Clean Architecture ve REST API prensiplerine uygun, hafif, ölçeklenebilir ve mikroservis tabanlı bir çözüm sunmayı amaçlamaktadır.

## Target Audience
Üniversite öğrencileri ve ödevleri ile son teslim tarihleri
Profesyoneller ve günlük görevleri ile sorumlulukları
Küçük ekipler ve görev takip ihtiyaçları
Yapılandırılmış ve akıllı not alma ihtiyacı olan kullanıcılar





 
 
## Core Features and Capabilities 
**Authentication Structure** 
Şu anda sistem, tüm işlemleri yürütmek ve erişimi sağlamak için tek bir Admin hesabına sahiptir. Notlarla ilgili tüm işlemler bu doğrulanmış hesap üzerinden gerçekleştirilir. Sistem şu an yalnızca tek bir yetkilendirme yapısıyla çalışmaktadır, ancak ölçeklenebilir şekilde tasarlanmıştır. Bu nedenle proje genişletildiğinde, sıfırdan başlamak gerekmeden ek erişim kontrol mekanizmaları sisteme dahil edilebilir.

**Urgency Level Classification** 
Her notun bir aciliyet seviyesi bulunmaktadır. Bu sayede kullanıcılar hangi işlerin hemen yapılması gerektiğini ve hangilerinin bekleyebileceğini anında görebilir. Bu durum görevlerin daha iyi organize edilmesini sağlar ve günlük akışı daha düzenli hale getirir.

  **AI-Driven Smart Sorting**
Akıllı sıralama, sistemin öne çıkan özelliklerinden biridir. Notları sıralamak için yapay zekâ kullanır. Her not, aciliyet ve önem derecesine göre değerlendirilir. Bu sayede en kritik not en üstte yer alır. Bu özellik, önemli görevlerin gözden kaçırılmasını önler.Ayrıca alınan notlar ve verilen veriler sayesinde beyninin hangi yönü unutmaya yatkın nasıl geliştirirsin .

 **CRUD Operations**
Sistem; oluşturma (create), okuma (read), güncelleme (update) ve silme (delete) işlemlerini destekler. Kullanıcılar yeni not ekleyebilir, mevcut notları görüntüleyebilir, güncelleyebilir ve silebilir.

 **RESTful API Architecture**
Sistem, tüm işlevlerine REST API üzerinden erişim sağlar. Bu sayede farklı istemci uygulamalarla kolayca entegre edilebilir. Bu özellik, sistemi modüler ve esnek hale getirir. 
 
 **Database Management**
Sistem, notları saklamak için bir veritabanına sahiptir. SQLite & PGADMIN veritabanı yönetim sistemi olarak kullanılmaktadır. Bu sayede veriler düzenli ve organize bir şekilde tutulur. 

**Containerization Support**
Sistem container yapısına sahiptir. Bu sayede farklı ortamlarda tutarlı bir şekilde çalışabilir. Containerization aracı olarak Docker kullanılmaktadır.

<img width="1886" height="872" alt="image" src="https://github.com/user-attachments/assets/5c0581d5-50d8-431a-aae4-5168d5dd2346" />


<img width="1911" height="915" alt="image" src="https://github.com/user-attachments/assets/aea5529c-118a-43f2-9dc4-f537013cb394" />

<img width="1916" height="948" alt="image" src="https://github.com/user-attachments/assets/82079a07-a9a9-4158-b2b8-461ce7159982" />

---

##  Projeye Genel Bakış (Project Overview)
Bu proje; **Docker** ile orkestra edilen, **JWT** ile güvenliği sağlanan ve **GitHub Actions** üzerinden sağlam bir **CI/CD** hattı ile otomatikleştirilen yüksek performanslı bir mikroservis yığınını (stack) uygular. 

Öne çıkan özelliği, kullanıcı verilerini analiz ederek beyin baskınlığını ve hafıza metriklerini belirleyen **"Bilişsel Zeka Paneli" (Cognitive Intelligence Dashboard)**'dir.
<img width="1642" height="906" alt="image" src="https://github.com/user-attachments/assets/05d8859b-5489-42a8-ab5b-63e7aedfc01d" />
<img width="1720" height="912" alt="image" src="https://github.com/user-attachments/assets/612bcf43-ed0b-4a59-a97e-448b2e11aeaa" />

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
