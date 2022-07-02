
# SORU 1 : Symfony kullanmanın avantajları nedir? Kendi cümlelerinizle açıklayınız.

 - Düz PHP ile yazdığınız kodu yaklaşık 1/5 kadar kısa bir zamanda yazabilirsiniz. 
 - Hazır kütüphaneler oluşturarak hazırladığınız modülleri tek satır kod ile projenize çağırabilir ve çalıştırabilirsiniz. 
 - Güvenlik açısından baktığımızda geniş bir geliştirici kitlesinin olması sebebiyle sürekli güncellenir ve güvenlik ve stabilize konusunda tüm işlemleri otomatik sağlar. CSRF, XSS, SQL Injection vs. gibi birçok saldırıya karşı koruma sağlar.
 - Bir proje içerisinde birden fazla yazılımcının entegre şekilde tek bir kurguda kod yazmasını sağlar.
 - Console komutlarını tek bir kodda otomatikleştirebilirsiniz.

# SORU 2 : Symfony ile environment (ortam) ayarlaması nasıl yapılır?
 
 Symfony ile environment oluşturmak için öncelikle composer'ı kurmamız gerekiyor. Composer kurulduktan sonra
 altaki komut satırını konsola girerek çalışma ortamı oluşturumaya başlıyoruz.
 
    //geleneksel bir web uygulaması oluşturuyorsanız bunu çalıştırın
    symfony new my_project_directory --version=5.4 --webapp

    //bir mikro hizmet, konsol uygulaması veya API oluşturuyorsanız bunu çalıştırın
    symfony new my_project_directory --version=5.4   
    
 Eğer gelenekssel bir web uygulaması ortamı oluşturmak istiyorsanız devam den bir kaç işlem daha 
 mevcut. Bu işlemler composer'dan web uygulaması için gerekli dosyaları ortamınıza yukleme işlemleridir.
 Bunun içinde  oluşturduğunuz ortam dosyanızın içine konsolda girerek altaki komutu yazmanız yeterlidir.
 gerekli dosyalar bu komut sayesınde ortam dosyanıza kurulacaktır.

    composer require webapp

# SORU 3 : Yeni bir Symfony projesi oluşturmak için kullanılan composer komutu nedir? Alternatif bir komutla Symfony projesi oluşturabilir miyiz?

    composer create-project symfony/skeleton symproject

 Üstteki komut ile composer üzerinden symfony projesi oluşturabiliriz. Diğer bir secenek'de 2.soruda 
 anlattığım şekilde symfony cll'ni kullanarak çalışma ortamı oluşturabiliriz.

# SORU 4 : Laravel framework ve Symfony framework arasındaki temel farklardan iki tanesini yazınız.

  - Symfony veritabanı erişimi için Doktrini kullanıyorken, Laravel veritabanı erişimi için Eloquent kullanıyor.
  - Symfony ara katman yazılımını desteklemek için gözlemci kalıbı kullanırken ,Laravel ara katman yazılımını desteklemek için dekoratör desenini kullanıyor.
  

