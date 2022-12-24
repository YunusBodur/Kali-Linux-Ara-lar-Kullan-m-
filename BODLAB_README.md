

![hata](https://diskyver.com/wp-content/uploads/2022/03/Illustration-Wireshark-png_Plan-de-travail-1.png) 

# Bilgi Toplama Araçları
Bir sisteme veya bir ortama sızmanın en temel ve birinci aşaması o sistem veya ortam hakkında bilgi toplamaktır. Bu aşama ne kadar iyi şekilde yapılırsa hedef sistem veya ortama saldırmak o kadar kolaylaşır.

İzlediğiniz eğitim içeriklerinde bu aşamayı muhtemelen çok kısa şekilde görmüş olabilirsiniz. Ama inanın bu aşama görüldüğü gibi kolay bir aşama değildir. Bu aşamayı şu şekilde hayal edebilirsiniz. Saldırmak istediğiniz yap, sizin için en başta tamamen karanlık bir ortam ve sizin elinizde de bir tane fener bulunsun. Siz ne kadar çok noktaya ışık tutup arama yaparsanız sonuca yani çıkışa ulaşmanız o kadar kolay olur.

Bu aşama saldırganlar için belki bir gün, belki bir ay belki de bir yıl sürebilir. Ağın iç yapısını anlamak, topolojisini çıkarmak ve aralarında ilişki kurmak bu aşamanın bir parçasıdır.

Bu aşamalarda sizlere yardımcı olabilecek araçlardan bahsetmeye çalışacağım.

# Wireshark:
Ağ protokolü analizörüdür.
Ücretsizdir.
Ağınızda olan biten ne küçük ayrıntıyı bile görmenizi sağlar.
Ağ koklama içinde kullanılabilen en iyi Kali Linux araçlarından biridir.,
Anlık olarak ağ trafiğini izlemenize ve daha sonra da çevrimdışı analiz etmenize imkan tanır.
# Nikto:
Güçlü bir web sunucusu tarayıcısıdır.
Saldırı yapmayı planladığınız web sitesi hakkında zafiyet taraması gerçekleştirir.
Ayrıca bu tarama sonucu size site içinde bulduğu belgeler, dizinler ve diğer bulgular hakkında bilgi verir.
‘nikto –h’ komutunu terminale yazarak araç hakkında bilgi edinebilirsiniz.
# Nmap:
Bu program ağ araştırması ve güvenlik denetimi yapabilen bir araçtır.
Açık kaynaklı olup ücretsizdir.
Ana bilgisayar, ağ güvenliği ayrıntıları gibi bilgiler sunmaktadır.
GUI ekranına sahip versiyonu da vardır.(Zenmap)
Şu anda tüm işletim sistemlerinde aktif olarak çalışmaktadır.
# Unicornscan:
Nmap aracına yerine geliştirilmiş ve hemen hemen benzer işlemleri yapabilen bir araçtır.
Nmap aracını kullanım aşamasındaki parametre fazlalığı burada yoktur.
İşletim sistemi belirleme, ağ haritalama işlemleri yapabilir.
Zaman uyumsuz TCP taraması yapabilir.
# Fierce:
Hedef sistem veya domain hakkında bilgi toplama aşamasında yardımcı olan bir araçtır.
DNS enumeration için kullanılan bir araçtır.
Zone-Transfer, DNS Brute-Force denemeleri de yapabilir.
Fierce bir IP tarayıcısı veya DDoS aracı değildir.
# Maltego:
Veri madenciliği aracıdır.
Çevrimiçi bilgileri analiz etmeyi sağlar.
Veri parçaları arasındaki bağlantıları incelemeye yardımcı olur.
Aktif ve pasif bilgi toplama özelliği vardır.
# Dnsrecon:
Hedef site hakkında bilgi toplama aşamasında yardımcı olur.
Subdomain, IP adresleri gibi bilgiler elde edebiliriz.
Açık kaynak kodludur.
Zone transfer, reverse lookup önemli kayıtları da tarar.
# Dnsenum:
Bu araç whois bilgileri, reverse lookup gibi bilgilere ulaşmamızı sağlar.
MX kaydı, NS kaydı, zone transfer birçok bilgi bulmaya da yardımcı olur.
Bu bilgileri analiz etmenize olanak tanır.
# Urlcrazy:
Bu araç ile hedef domain’e benzer domainleri listeleyebiliriz.
Ayrıca bu aracın değişik bir özelliği ise hedef domain’nin popülerliğini ölçebiliyor olmasıdır.
# Dmitry:
Hedef hakkında bilgi toplamaya yarayan bir backtrack aracıdır.
Subdomaion, uptime bilgi, email adresleri whois gibi bilgileri de toplamaktadır.
# Angry IP Scanner:
IP adresi ve port tarayıcısı görevi görür.
Herhangi bir aralıktaki IP adreslerini tarama özelliğine sahiptir.
Tarama hızını artırmak için multl-threat bir yaklaşım kullanır. Burada taranan her IP adresi için ayrı bir tarama threat oluşturulur.
Buraya kadar olan kısımda bilgi toplama araçlarından bahsettim. Şimdi diğer araç türlerinden bahsedeceğim.

# Password Saldırıları
# John The Ripper:
Hızlı bir şifre kırıcıdır.
Ücretsiz ve açık kaynak kodludur.
Sızma testlerinde elde edilen HASH değerlerinin kırılması için kullanabiliriz.
# THC-Hydra:
Kaba kuvvet kullanarak parolaları kırmaya çalışan bir araçtır.
SSL kullanan protokoller için de kullanımı vardır. Bu şifreli trafiğe de kaba kuvvet saldırısı uygulayabiliriz.
Çok hızlı ve esnektir.
# Kablosuz Ağ Saldırıları
# Aircrack-ng:
WEP ve WPA-PSK şifre kırma aracıdır.
Ağ trafiği sezilebilir.
Modeme bağlı olan bir aracın modeme bağlanması engellenebilir.
#Zaafiyet Analizi Araçları
# sqlmap:
Web uygulamalarında SQL injection tespiti yapabilen bir araçtır.
Açık kaynak kodludur.
Tespit ettiği açıkları istismar etme özelliğine de sahiptir.
Veri tabanı sunucularını ele geçirmek gibi bir sürü işlevi bulunmaktadır.
# Yersinia:
TCP-IP modelinde bulunan ikinci katmana yönelik saldırıları gerçekleştirmede kullanılır.
STP, CDP, DTP gibi çeşitli ağ protokollerine odaklanır.
# Web Uygulamalarına Yönelik Saldırı araçları
# Burp Suite:
Web güvenliği analizi aracıdır.
Bir uygulamanın saldırı yüzeyinin ilk haritalandırılmasında yardımcı olur.
Daha sonra bu harita ile analiz yapmak, güvenlik açıklarının detaylı şekilde bulunması gibi pek çok aktivitede destek sağlar.
# WPScan:

Wordpress tabanlı web sitelerinde tarama faaliyetlerini gerçekleştirir.
WordPress versiyon numarası hakkında bilgi edinmemizi sağlar.
Yetkili kullanıcı adlarını ve diğer kullanıcı adlarını bulabilir.
Sitedeki güvenlik açıklarını tespit edebilir.
# Dirb:
DIRB, Web içerik tarayıcısıdır.
Bütün içerikleri veya linkleri çıkarıp liste halinde size sunan bir araçtır.
Görünen veya görünmeyen, bütün içerikleri listelemek istersek, DIRB bu konuda bize yardımcı olur.


# #Eminim bu araçların birazını biliyorsunuz ya da bazılarını yeni duydunuz. Ama her zaman daha fazlasını öğrenmeye çalışmakta fayda var. Kali Linux’un resmi hesabında bu araçların tanıtımı yapılmaktadır.
  

  
  
  
  
  
  
