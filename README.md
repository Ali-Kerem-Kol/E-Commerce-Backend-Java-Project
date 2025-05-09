# E-Ticaret Backend Java Projesi

## Proje Açıklaması

Bu proje, Spring Boot kullanılarak geliştirilen bir e-ticaret platformunun arka ucunu (backend) uygular. Kullanıcıların ürünleri alışveriş sepetine eklemeleri, sepetlerini yönetmeleri ve sipariş vermeleri için bir API sağlar. Güvenlik, JWT (JSON Web Token) kullanılarak sağlanır ve kullanıcı kimlik doğrulaması garanti altına alınır. Ayrıca, kullanıcı hesapları, alışveriş sepetleri ve siparişleri yönetmek için gerekli servisleri ve veritabanı yapısını da içerir.

---

## Kullanılan Teknolojiler

- **Java 17** (veya daha yeni sürümler)
- **Spring Boot** (Web, Data, Security, JPA)
- **JWT** (Kimlik doğrulama için JSON Web Token)
- **Spring Security** (API uç noktalarını güvenli hale getirmek için)
- **PostgreSQL** (veya tercihinize bağlı başka bir veritabanı)
- **Lombok** (Boilerplate kodları azaltmak için)
- **Maven** (Bağımlılık yönetimi için)
- **JPA / Hibernate** (Veritabanı etkileşimleri için)
- **Postman** (API testleri için)

---

## Özellikler

- Kullanıcı kaydı ve giriş
- JWT tabanlı güvenlik ve kimlik doğrulama
- Alışveriş sepeti yönetimi
  - Sepete ürün ekleme, çıkarma ve miktar güncelleme
  - Sepetteki ürünleri görüntüleme
  - Sepeti temizleme
- Sipariş oluşturma
- Kullanıcıları ve ürünleri yönetmek için admin yetkisi
- Kullanıcı dostu hata mesajları ile hata yönetimi
- Spring Security ile güvenli API uç noktaları

---

## Kurulum

1. Depoyu bilgisayarınıza klonlayın:

    ```bash
    git clone https://github.com/your-username/E-Commerce-Backend-Java-Project.git
    ```

2. Projeyi IDE’nizde açın (örneğin IntelliJ IDEA veya Eclipse).

3. `application.properties` dosyasına gerekli bilgileri ekleyin. Özellikle aşağıdaki alanları kendi bilgilerinizle doldurduğunuzdan emin olun:

    - **Veritabanı**:
      - `spring.datasource.url`: Veritabanınızın bağlantı URL’si.
      - `spring.datasource.username`: Veritabanı kullanıcı adınız.
      - `spring.datasource.password`: Veritabanı şifreniz.
      
    - **E-posta**:
      - `spring.mail.username`: E-posta adresiniz (onay e-postaları göndermek için).
      - `spring.mail.password`: E-posta hesabınıza özel uygulama şifresi.

    **Uyarı:** `application.properties` dosyasındaki örnek değerleri kendi gerçek bilgilerinizle değiştirmeyi unutmayın:

    ```properties
    spring.datasource.url=[Veritabanı URL’iniz]
    spring.datasource.username=[Kullanıcı adınız]
    spring.datasource.password=[Şifreniz]
    
    spring.mail.username=[E-posta adresiniz (onay e-postaları için)]
    spring.mail.password=[Uygulamaya özel şifreniz]
    ```

4. Projeyi çalıştırın:

    ```bash
    ./mvnw spring-boot:run
    ```

5. Tarayıcınızdan `http://localhost:8080` adresine giderek API'ye erişebilirsiniz.

---

## Postman Alanı

API'yi aşağıdaki bağlantı üzerinden paylaşılan Postman çalışma alanında da test edebilirsiniz:  
[<img src="https://run.pstmn.io/button.svg" alt="Postman'da Çalıştır" style="width: 128px; height: 32px;">](https://god.gw.postman.com/run-collection/37739159-d3965a51-94ac-419c-8068-b965338288db?action=collection%2Ffork&source=rip_markdown&collection-url=entityId%3D37739159-d3965a51-94ac-419c-8068-b965338288db%26entityType%3Dcollection%26workspaceId%3Ddbeb00ea-a61f-4017-acac-c435de319aa6)

---

## Katkıda Bulunma

Bu repoyu forklayabilir, geliştirmeler yapabilir ve pull request gönderebilirsiniz. Katkılarınız her zaman memnuniyetle karşılanır!

---

## Lisans

Bu proje [MIT Lisansı](LICENSE) ile lisanslanmıştır. Detaylar için LICENSE dosyasına göz atabilirsiniz.
