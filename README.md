Berkay CILIZ 130202013 

Başlatmak için

"npm install -g @ionic/cli"
"git clone https://github.com/BerkayCiliz/130202013.git"
"cd ionifits"
"npm install firebase"
"ionic serve" işlemlerini sırayla komut istemine uygulayınız.

İlk olarak npm kurulumunu nodjs kurulumunu yaptım.Daha sonra ionic frame work kurulumunu yaptım.
Bundan sonra bir ionic projesi oluşturdum oluşturuken angular vs yapılarını proje içerisine kurdum.
Daha sonra veritabanı  kullanmak için firebase de bir veritabanı oluşturdum oradaki configurasyon bilgilerini aldım.
Bunları environments içerisine kayıt ettim.
Daha sonra cloud içerisinde maile gönderme işlemi yapacağım için izinlerini etkinleştirdim.
Daha sonra firebase i kullanmak için kütüphanelerini yani  aut,store ve service vb. yapılarını ekledim.
Daha sonra auth servis içine kullanıcının login register home bölümlerinin yazılımını yaptım.
Öncelikle login ekranında eğer kaydımız yoksa yeni kayıt almamızı sağlayan navigate kullanarak register kısmına geçişini sağladım.
Kayıt olunduğu zaman verilen maile bir onay mesajı gidiyor bu onay mesajını kullanıcı kendi mail adresinden onayladığı zaman kayıt yapmış sayılıyor.
Ve kayıt ol işleminden sonra sistem direk login ekranına yine navigate ile atıyor. Kayıt olunduğu an firebase veritabanı üzerinden kişinin bilgileri görünüyor.
Ve birde eğer şifreyi unutursak forgot-password işlemi yapabiliyoruz buda navigate ile şifre yenileme sayfasına yönlendiriyor ve orada işlemimizi yapabiliyoruz.
Daha sonra ekrandaki görüntüler için html kullanarak mesela kayıt yerindeki mail kullanıcı adı şifre vb. yazılarını gösterdim.
Local host üzerinden login kısmında giriş yapabiliyorum.Kayıt olma kısmıda register olarak geçebiliyoruz.
Login kısmınında componentler kullanılarak html de yazdıklarımıda birleştirebiliyorum.

Yani buraya kadar servisler kullanıldı,component kullanıldı,navigate ile sayfalar arası geçişler yapıldı, 
giriş –kayıt ol-şifre yenile yapısı kuruldu , firebase ile veritabanına veri ekleyip-çıkarma yapıldı.
