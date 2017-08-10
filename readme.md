## Simple Android Web View ##

1. Projeyi Android Studio'ya açın
2. En azından Android Studio V2.0 kullandığınızdan emin olun
3. res / değerlere göz atın ve strings.xml dosyasını açın
4. "app_name" dizesindeki yer tutucuyu, uygulamanızın adıyla değiştirin.
5. "dialog_about" yer tutucusunu kendi metninizle değiştirin (CDATA [] içinde tümü temel html'ye sahip olabilir).
6. İsteğe bağlı olarak Admob Afiş Reklam Birimi Kimliğinizi ve Admob Geçiş Birimi Kimliğinizi girin.
7. res / değerlere göz atın ve colors.xml dosyasını açın.
8. Renklerin yer tutucu değerlerini kendi renklerinizle değiştirin (# ile başlayan).
9. com.sherdle.webtoapp'a gidin ve Config.java dosyasını açın.
10. Analytics'i kullanmak istiyorsanız, ANALYTICS_ID için bir değer girebilirsiniz
11. İsteğe bağlı olarak 'yenilemek için çek' ve 'çekmece modu' gibi diğer parametreleri yapılandırın ve ayarlayın.
12A. Uygulamanızda tek bir url görüntülemek istiyorsanız, url dizisine bir URL girebilirsiniz, örneğin:
 Public static final String [] BAŞLIKLAR = new String [] {"MySite"};
 Public static final String [] URLS = new String [] {"http://mysite.com"};
12B. Uygulamanızda birden fazla bağlantı görüntülemek istiyorsanız, url dizininde tüm URL'lerinizi girebilirsiniz, örneğin:
 Public static final String [] BAŞLIKLAR = new String [] {"Google", "Yahoo", "DuckDuckGo"};
 Public static final String [] URLS = yeni String [] {"http://google.com", "http://yahoo.com", "http://hasanatilan.com.tr"};
13. OneSignal push bildirimlerini kullanmak isterseniz build.gradle (giriş / uygulama) 'yı açın ve' onesignal_app_id 've' onesignal_google_project_number 'için bir değer girin

Artık yalnızca varlıklarınızı değiştirmeniz (simge ve açılış ekranı) gerekir.

Simgesi
1. Önce bir uygulama simgesine ihtiyacınız olacak, bu uygulama bir kare .png resmi olmalıdır.
2. Simgenizi, Google Play Store gönderimi için 512x512 png bir resme ve uygulamanız için bir 124x124 resme yeniden boyutlandırmanız gerekir.
3. 124x124 resmini ic_launcher.png'ye yeniden adlandırın (ic_launcher.png.png olmamasına dikkat edin, bazen uzantı gizlidir).
4. 'uygulama' adı verilen bir klasörü göreceksiniz, açın ve 'res / mipmap-xhdpi /' klasörüne göz atın.
5. Şimdi bu klasöre ait ic_launcher.png dosyasını ic_launcher.png dosyanızla değiştirin.

Başlangıç ekranı
En iyi performans için, şeffaf bir arka plana sahip bir logoyu, ekran görüntüsü olarak kullanmanızı öneririz. Bu daha kolay ve çok daha iyi görünüyor.
1. Tabletlerde en iyi performansı elde etmek için logonuzu, tercihen yüksek kaliteli bir imajı alın ve adı vert_loading.png
2. Şimdi masaüstünüzdeki şablonun klasörü içindeki 'uygulama' adlı klasörü tekrar açın
Ve 'res / drawable-nodpi /' öğesine göz atın




Türkçeliştirme Hasan Atılan 

Yapımcı WEB2 Team.
