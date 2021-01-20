Berkay CILIZ 130202013 

Başlatmak için

"npm install -g @ionic/cli",
"git clone https://github.com/BerkayCiliz/130202013.git",
"cd 130202013",
"npm install firebase",
"ionic serve" komutlarını sırayla komut istemine uygulayınız.

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

Burada giriş yapılıyor eğer kayıt yoksa kayıt yapmak için register, şifre unutulduysa da forgot password diyerek diğer işlemlere geçebiliriz.
![giriş](https://user-images.githubusercontent.com/41726535/105178292-e0a2e480-5b38-11eb-8851-4cb36aa38259.png)




Login kısmında forgot password dediğimizde şifremizi değiştirmemiz için burası açılıyor.
![şifre unuttum](https://user-images.githubusercontent.com/41726535/105178867-a38b2200-5b39-11eb-8589-3d58709ed28e.png)




Eğer bir kaydımız yoksada register now dedikten sonra bu sayfaya yönlendiriliyoruz ve kaydımızı yapıyoruz.
![kayıt](https://user-images.githubusercontent.com/41726535/105178971-c9b0c200-5b39-11eb-97ee-c6a98a9d7cd8.png)




Kayıt yapıldıktan sonra  kişinin mailine aktivasyon mesajı geliyor ve tıkladığında kayıt tamamlanıyor ve burada firebase veritabanında kullanıcının bilgilerini görebiliyoruz.
![firebase veritabanı](https://user-images.githubusercontent.com/41726535/105179075-e4833680-5b39-11eb-9d6b-877b0f6be422.png)




Burada da kullanıcının oturum açma vaktini, kayıt tarihini ve diğer bilgilerini görebiliyoruz.
![firebase email mesaj](https://user-images.githubusercontent.com/41726535/105179167-07154f80-5b3a-11eb-8d59-a905c447a8eb.png)




En sonda da kaydı olan kullanıcı giriş yaptığında home sayfasına yönlendiriliyor.
![giriş home sayfası](https://user-images.githubusercontent.com/41726535/105179463-6f643100-5b3a-11eb-8265-5d4aa2f6bda4.png)
