# Facebook-Api-1.0
.NET ile Yazdığınız Projelerinizde Facebook İşlemlerinizi Yapmak İçin Kullanabileceğiniz Facebook Api'si

# Kullanım
Öncelikle https://developers.facebook.com adresinden yapacağımız işlemler için facebook uygulaması oluşturuyoruz.
İndirdiğiniz Dll Dosyalarınızı Projenize Ekledikten Sonra facebook.plugin.dll kütüp hanemizin içinde 3 adet metod bulunmaktadır.

 plugin.facebook f = new plugin.facebook();
 
 f.accessToken = "XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX";


1. Metodumuz

f.SharedFeed("Merhaba Dünya");

2.Metodumuz

//byte[] img = File.ReadAllBytes(Server.MapPath("~\\Images\\facebook.jpg")); // Web Form

byte[] img = File.ReadAllBytes("C:\\1.jpg"); //Win Form

f.SharedPhoto(img,"deneme deneme"); 


3.Metodumuz

f.SharedPage("http://www.test.com", "http://www.test.com/page.jpg", "Test İnternet Sayfası","Caption text","Description Text");
