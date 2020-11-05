# 24 Ekim Ödevleri
## Hesaplarım
>- [HackerRank](https://www.hackerrank.com/meeyzt)
>- [StackOverflow](https://stackoverflow.com/users/14513359/meeyzt)

## Docker'a ve Docker'a ait kavramlara nelerdir?
>![Docker LOGO](https://d1.awsstatic.com/acs/characters/Logos/Docker-Logo_Horizontel_279x131.b8a5c41e56b77706656d61080f6a0217a3ba356d.png)
>
>Docker, yazılım geliştiriciler ve sistemciler için geliştirilen açık kaynaklı bir sanallaştırma platformudur. Docker ile Linux, Windows ve MacOSX üzerinde Linux ve Windows sanal containerler (makineler) çalıştırabilirsiniz. Bu platform sayesinde web sistemlerinin kurulumunu, testini ve dağıtımını kolaylıkla gerçekleştirebilirsiniz. En önemli özelliği belki de "Benim bilgisayarımda çalışıyordu, sunucuda neden çalışmadı acaba?" sorununu ortadan kaldırıyor olması.** 
>* **Docker Daemon:**
>  * Hypervisor’ün dockerdaki karşılığıdır. Bütün CPU ve RAM vb gibi işletim sistemine ait işlerin yapıldığı bölümdür.
>
>* **Container Nedir:** 
>  * Docker Daemon tarafından Linux çekirdeği içerisinde birbirinden izole olarak çalıştırılan process’lerin her birine verilen isimdir. Virtual Machine (Sanal Makine) analojisinde Docker’ı Hypervisor’e benzetirsek fiziksel sunucu üzerinde halihazırda çalıştırılmakta olan her bir işletim sisteminin (sanal sunucunun) Docker’daki karşılığı Container’dır. 
> 
>* **Image Nedir:**
>  * Containerlar layer halindeki Image’lardan oluşur. Docker Image ise containerlara kurulacak ve run edilecek olan uygulamaların veya OS’lerin image dosyalarıdır. Örnek verecek olursak mysql, mongodb, redis, ubuntu, mariadb.. Yüzlercesi mevcut. Buyrun: [Docker Images List.](https://hub.docker.com/search?q=&type=image)    
 Fakat burada şöyle bir ayrıntı var. Aslında container içerisindeki imagelerin içeriklerinin ve tanımlamalarının gerekli tutulduğu bir dosya var. Bu dosyamızın adı: **Dockerfile.** Tamamen bu isimde, ne büyük ne de küçük harflerden oluşan, bir bakıma containerlar içindeki imagelerın registration’ını yapan bir dosya. Burda önemli nokta şu: Her bir image Dockerfile dediğimiz bu dosyanın altında tanımlanması zorunlu.
>
>* **Docker Registry Nedir:**
>  * Gelelim bence işin en zevkli kısmına. Tıpkı github gibi geliştiriciler açık kaynaklı olarak docker imagelerini yükleyerek ve [DockerHub](https://hub.docker.com/)’ta paylaşarak imagelerin bizim de indirip kullanmamıza olanak sağlıyorlar. Kısaca imagelar Docker Registrylerde tutuluyor.
>* **Docker CLI Nedir:**
>  * Kullanıcının Docker Daemon ile konuşmasını sağlayan, docker komutlarının çalıştırıldığı CLI ekranıdır.
>* **Docker Compose Nedir:**
>  * Compose, birden fazla containere sahip docker uygulamalarını tanımlamak ve çalıştırmak için kullanılır. Compose ile uygulamanızın servislerini configure etmek için bir YAML dosyası kullanılır. Ardından, tek bir komutla configure ettiğiniz ayarlar ile tüm servislerinizi oluşturup ve başlatabilirsiniz.

## .Net Core versiyonları ve bu versiyonlar arasındaki farklar
>| Son .NET Core Versiyonları                | Çıkış Tarihleri |
>|---------------------------|--------------|
>| .NET Core 2.1.x (servis sürecinde) | UVD (Uzun Vadeli Destek) sürümü, Yaklaşık 1-2 ayda bir veya gerektiğinde. |
>| .NET Core 3.1.x (servis sürecinde) | UVD (Uzun Vadeli Destek) sürümü, Yaklaşık 1-2 ayda bir veya gerektiğinde. |
>| .NET 5.0 | Kasım 2020 için planlanan sürüm. |
>| .NET 6.0 | UVD (Uzun Vadeli Destek) sürümü, Kasım 2021 için planlanan sürüm. |
>| .NET 7.0 | Kasım 2022 için planlanan sürüm. |
>| .NET 8.0 | UVD (Uzun Vadeli Destek) sürümü, Kasım 2023 için planlanan sürüm. |
>
>* **.NET CORE 1.1**
>  * .NET Core’un performansı iyileştirildi, ASP.NET Core’un Kestrel’i iyileştirildi ve Azure desteği getirildi, Entity Framework Core’a Azure ve SQL 2016 desteği getirildi 10larca yeni özellik ve 100 lerce bug fix yapıldı. Belgelendirme(documentation) iyileştirmesi yapıldı. Performans iyileştirici çalışmalar yapıldı.
>
>* **NET CORE 2.0** 
>  * C# ve F # ' ı desteklemeye ek olarak, .NET Core 2,0 de Visual Basic destekler. MacOS üzerinde .NET Core 1. x, OpenSSL araç setinin şifreleme kitaplığını gerektirdi. .NET Core 2,0, Apple şifreleme kitaplıklarını kullanır ve OpenSSL gerektirmez, bu nedenle artık yüklemeniz gerekmez. Kodunuzu her değiştirdiğinizde Live Unit Testing otomatik olarak etkilenen birim testlerini arka planda çalıştırır ve Visual Studio ortamında sonuçları ve kod kapsamını canlı olarak görüntüler. .NET Core 2,0 artık Live Unit Testing desteklemektedir. Daha önce Live Unit Testing yalnızca .NET Framework uygulamalar için kullanılabilir.
>
>* **NET CORE 2.1**
>  * Genel araçları destekler(komut satırından kullanılabilen özel araçlar). .NET Core 'un önceki sürümlerindeki genişletilebilirlik modeli, yalnızca kullanarak bir proje temelinde bulunan özel araçları kullanıma sunulmuştur. 
>
>* **NET CORE 2.2**
>  * DLL dosyaları yerine .exe dosyaları olan çerçeveye bağımlı yürütülebilir dosyaları dağıtılabilir. .NET Core 2.2 ile başlayarak, bir uygulamanın ana metodunu çalıştırmadan önce kodu eklemek için bir başlangıç kancası kullanabilirsiniz. Başlangıç kancaları, bir konağın uygulamayı yeniden derlemenize veya değiştirmeye gerek kalmadan dağıtıldıktan sonra uygulamaların davranışını özelleştirmesini olanaklı kılar.
>
>* **NET CORE 3.0**
>  * En büyük geliştirmelerden biri, Windows Masaüstü uygulamaları için destek içerir (yalnızca Windows). .NET Core 3.0 SDK bileşeni Windows Masaüstünü kullanarak Windows Forms ve Windows Presentation Foundation(WPF) uygulamalarınızın bağlantı noktası oluşturabilirsiniz.
>
>* **NET CORE 3.1** 
>  * Eski denetimler, Visual Studio Tasarımcı araç kutusunda bir süredir kullanılamayan Windows Forms eklenmiştir. Bunlar .NET Framework 2.0'daki yeni denetimlerle değiştirilmiştir. Bunlar .NET Core 3.1 için masaüstü SDK'dan kaldırılmıştır.
>
>* **NET CORE 5.0** 
>  * Yeni uygulama geliştirme, .NET 5.0 sınıf kitaplıkları da dahil olmak üzere tüm proje türleri için hedef çerçeve bilinen adını (tfd) belirtebilir. .NET 5 iş yükleri arasında kod paylaşımı, tüm ihtiyacınız olan tfd'de basitleştirilmiştir. .Net 5 ile artık tek bir .Net olacak, yani Xamarin,Unity,ML.Net dahil olmak üzere tüm framework’ler tek bir çatı altında birleşiyor. .Net 5 mobil, Xbox ve diğer oyun platformları için oyun geliştirilebilen Unity’i destekleyecek.

## .Net 5 geçilme ihtiyaçları nelerdir, geçiş sürecinin tamamlanmasıyla neler hedeflenmektedir.
> Şimdiye kadar .Net Core için yazdığımız kütüphaneler .Net Framework’te çalışmayabiliyordu.Net Framework ile yazılmış bir uygulamayı .Net Core’a geçirirken shared library olarak bazı tanımlamalar yapmak gerekebiliyor. Çözüm olarak tanımlamalarımızı .Net Standart ile geliştirmemiz gerekiyordu ancak .Net 5 ile birlikte artık tek bir Base Class Library olacak. Şu anda Xamarin uygulamaları Mono Base Class Library kullanırken artık .Net 5 ile .Net Core Base Class Library kullanabilecek.
> Kod yazmak ve kodu taşımak daha kolay olacak.
## Markdown yazımı ve kullanımı 
> Markdown, yazılarımızı düz metin olarak yazmamıza imkan veren işaretleme/biçimlendirme dilidir (markup language). Markdown'ın temel amacı, metnimizi kolayca hazırlamak ve düz metin haliyle bile metnin rahatça okunmasını sağlamaktır.
> * Kullanımı
>   * Html de <h1></h1> Şeklinde yazmak herine "h"'ın yanındaki sayı kadar "#" kullanmaktayız.
>   * Bir alıntı yapacağımız zaman ">" Kullanabiliriz.
>   * Tablo oluşturacağımız zaman; 
> ``` |   | Fiyat   | Adet  |
> | --|:-------:| -----:|
> | A | 1000TL  | 1     |
> | B | 100TL   | 10    |
> | C | 1TL     | 1000  | b
> ```
> Daha fazla Detaylı bilgiye [MarkDown Kullanımı](https://www.markdownguide.org/basic-syntax/) tıklayarak ulaşabilirsiniz.

## Yazılım alanında takip ettiğiniz kişiler kimlerdir?
> Selman Kahya [Youtube](https://www.youtube.com/channel/UC9Z-Gc_BkYuW75jKcTJICJA), [Github](https://github.com/SelmanKahya), [Blog](https://medium.com/@selmankahya)   
>  Murat Yücedağ [Youtube](https://www.youtube.com/user/YazilimHerYerde), [Blog](https://muratyucedag.com/), [Udemy](https://www.udemy.com/join/login-popup/?next=/course/sifirdan-ileri-seviye-csharp-programlama/learn/%3FcouponCode%3DMAYIS2020)
## Microsoft Azure tarafında ne gibi hizmetler vardır?
>![Azure Hizmetleri](https://www.mshowto.org/images/articles/2015/03/032115_0557_MicrosoftAz3.png)
## Kodun kalitesinin metrik olarak ölçülmesinden ne anlamaktasınız?
> Yazacağımız kodun bazı prensiplere uygun olması gerekiyor ve bu prensiplere uyduğumuzda kodumuzun kalitesi git gide artıyor. Örneğin; Solid prensipleri.
### Kaynaklar
> * [Docker Kavramları](https://medium.com/batech/docker-nedir-docker-kavramlar%C4%B1-avantajlar%C4%B1-901b37742ee0)
> * [Kod Kalite ölçümleri](https://www.baranbayram.net.tr/kod-kalite-olcumleri-ve-sik-kullanilan-metrikler.html)
> * [.NET CORE versiyonları](https://github.com/dotnet/core/blob/master/roadmap.md)
> * [.NET CORE Bilgilendirme](https://en.wikipedia.org/wiki/.NET_Framework_version_history)
> * [Azure Servisleri](https://www.mshowto.org/0dan-100e-azure-servisleri-azure-vm-monitor.html)
> * [MarkDown](https://www.markdownguide.org)


