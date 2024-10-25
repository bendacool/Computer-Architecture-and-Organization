# Computer-Architecture-and-Organization 

Bilgisayar, yüksek hızda aritmetik ve mantıksal işlemleri art arda yapabilen ve karar verebilme yetisine sahip hafızalı bir elektronik cihazdır.

## 1. Kuşak Bilgisayarlar - Vacuum Tube Bilgisayarlar
- Vakum Tüp Lambalı elektronik anahtar elemanlarının kullanıldığı bilgisayarlardır.
- İlki; Atanasoff- Berry Bilgisayar (ABC)‘dır. Lineer denklem takımlarını çözmek için kullanıldı.
- ABC, mekanik anahtarlar yerine vakum tüplerinin kullanıldığı ilk bilgisayardır. 
- İlk sayısal bilgisayardır.
## 2. Kuşak: Transistörlü Bilgisayarlar
- Transistörün icadıyla vakum tüp devri kapanıyor.
- Transistör; Vakum tüpten çok daha küçük (1/13), daha az enerji harcıyor, daha hızlı anahtarlıyor.
## 3. Kuşak: Entegre Devreli Bilgisayarlar
- Texas Instruments’da çalışan Jack Kilby ve Fairchild Semiconductor’da çalışan Robert Noyce’un birbirlerinden bağımsız olarak çalışmaları sonucunda “entegre devre” (Integrated Circuits – IC) ortaya çıktı.

__Entegre Devre Teknolojisi__
- Entegre devre teknolojisi, transistör, diyot vb. statik elektronik devre elemanının yüzlercesinin bir silisyum veya germanyum yüzeye kimyasal yollarla yerleştirilmesi şeklindedir. 

### İlk Üçüncü Kuşak Programlama Dilleri
- Programcıların istedikleri işlemleri kolay yapabilmelerine imkan sağlayacak programlama dil arayışları da sürmekteydi.
- İlk olarak FORTRAN (Formula Translator) programlama dili mühendislik hesapları için ortaya çıktı.
- Ticari uygulamalarda kullanılmak üzere COBOL (Common Business Oriented Language) programlama dili ortaya çıktı.

### İşletim Sisteminin Doğuşu
- Bir programda kullanılan bir alt program, geliştirilen başka bir programda da yeniden yazılmaktaydı. Her programda standart olan alt programları bir kütüphane yapısı içinde toplamak ve ihtiyaç duyulduğunda o alt programları oradan çağırıp işlemleri gerçekleştirebilmenin yollarını aramaya başladılar. “İşletim Sistemi” yazılımları ortaya çıktı. 
- Her bilgisayar üreticisi kendi işletim sistemini geliştirerek kullanıcılara daha rahat program yazabilecekleri ortamlar sağlamaya başladılar.

## 4. Kuşak VLSI (Very Large Scale Integration) entegre devreli Bilgisayarlar (1980 - ????) (Microprocessors- Mikroişlemciler)
- Çok büyük çaplı entegre devrelerin içinde en az 10.000 adet bağlaca eşdeğer eleman vardır.
- Mikroişlemci gelişimi bu dönemde çok hız kazanmıştır.
- İlk 4 bit işlemci olan INTEL 4004 gerçekleşmiştir. Intel 8088 de "personal computer“ fikrinin ilk uygulaması.

#### Xerox Alto
- Kullanıcı için grafiksel arayüzlü ilk bilgisayardır.
- Ayrıca bizim bildiğimiz, fare, klavye özellikli ve "masaüstü" monitörlü ilk yapıdır.

#### Moore Yasası
Entegre devredeki transistör yoğunluğu her yıl iki katına çıkacak. 
__`Günümüz versiyonu:`__ silikon çip yoğunluğu her 18 ayda iki katına çıkar.
	Fakat bu yasa sonsuza kadar geçerli olamaz. 

<hr>

## Von Neumann Bilgisayar Modeli
- Von Neumann mimarisi veri ve komutları tek bir veri depolama biriminde barındıran bilgisayar tasarı örneğidir. Belleğin, işlemciden ayrılması Von Neumann mimarisi olarak ifade edilir. 
- İlk hesap makineleri değişmez yazılımlara sahiptiler. Bir makine hangi işlemi gerçekleştirmesi için tasarlandıysa sadece onu yerine getirebiliyordu. Bu tür bilgisayarların yeni bir görevi yerine getirebilmesi için donanımlarının tekrar tasarlanması zorunludur. Bu zorlukların aşılması "saklı yazılım bilgisayarı" ilkesi ile gerçekleşmiştir. 
- Makinenin yürütebileceği bir dizi komutun tanımlanması ile bilgisayarlar çok daha esnek bir yapıya kavuştular. Komut ve verinin aynı biçimde saklanması ise, bu ilke sayesinde yazılımın kolayca değiştirilebilmesine olanak tanımıştır. Saklı yazılım tasarımı, ayrıca yazılımların çalıştırılmaları esnasında kendilerini değiştirebilmelerini mümkün kılar.

__Central Processing Unit (CPU - MİB):__ Kontrol Birimi (komut kodlarının çözülmesİ, İşlemlerin sıraya konması v.b), Datapath (Register’lar, Aritmetik ve mantıksal işlem birimi , Veri yolları) alt birimleri vardır.

__Memory:__ Komutların ve verilerin saklandığı ortam.

__Input/Output (I/O) sub-system:__ I/O BUS’ları, Arayüzler, Elemanlar.

<hr>

## Bilgisayarın hiyerarşik yapısı
Bilgisayarların çalışmasını anlamak için sanal katmanlı bir yapı modeli uygundur. Her bir katman belirli görevleri gerçekleştirmek içindir ve kendi komutları vardır. Katmanlar gerektiğinde alt seviyelerdeki komutları çağırabilirler. Esas işi en alt tabakadaki sayısal devreler yapacaktır.
##### Seviye 6: Kullanıcı seviyesi
Kullanıcı ile bilgisayarın etkileştiği arayüzdür.
##### Seviye 5: Yüksek-seviyeli dil seviyesi
C, Java vb. programla dilleri ile yazdığımız programlarla bilgisayarla etkileşimde bulunduğumuz seviyedir. 
##### Seviye 4: Assembler dili seviyesi
`5.seviye`deki yüksek-seviye dilinde yazılmış program assembler diline çevrilir. 
##### Level 3: Sistem yazılımı seviyesi
Sistemde işlenen işlemleri kontrol eder. Sistem kaynaklarını korur. 
Assembler dili komutları fazla değişikliğe uğramadan bu seviyeye geçer.
##### Seviye 2: Makine dili seviyesi
Instruction Set Architecture (ISA – Komut Seti Mimarisi) seviyesi olarak bilinir.
- Makine mimarisine özel komutların oluşturulduğu seviyedir. Makine dilinde yazılmış programlar hiçbir şekilde derleyiciye, yorumlayıcıya veya assembler’a ihtiyaç duymazlar. 
##### Seviye 1: Kontrol Seviyesi
Bir kontrol ünitesi komutları decode eder ve işler. Verileri sistem üzerinde hareket ettirir.
Kontrol üniteleri mikro programlanabilir olabilir veya sadece devrelendirilmiş(Hardwired) yapıdadır. Bir mikro program donanım tarafından uygulanabilen, bir düşük seviyeli bir dilde yazılmış bir programdır. Devrelendirilmiş(Hardwired) üniteler, doğrudan makine komutlarını çalıştırır donanımlardır.
##### Seviye 0: Digital Logic Seviyesi
Bu seviyede birbirine uygun bir şekilde bağlanmış sayısal mantıksal devreler bulunur (IC’nin içinde)
Bu bileşenler, diğer üst seviyelerdeki matematiksel ve Mantıksal işlemleri gerçekleştirir. 

<hr>

__Hertz =__ Bir saniyedeki clock sayısı (frequency)

__Byte =__ Hafıza kapasite birimidir.

__Milisaniye =__ 1/100.000 saniye. Bir Hard disk sürücünün erişim zamanı 5 - 20 ms’dir.

__Nanosaniye =__ 1/1.000.000.000 saniye. Bir RAM’ın erişim zamanı 30 ile 70 nanosaniyedir.

__Micron (micrometre) =__ 1 metrenin milyonda biri. Bir işlemci teknolojisini belirtmek için iki komponent arasındaki mesafeyi verir. Örnek: 1 mikron teknolojisi.

<img src="./Pasted image 20241024135139.png" alt="example" />

## Chipset
- Anakart trafiğini yöneten birim

Parçaların aralarında iletişim kurmasını ve gerekli işlemlerin gerçekleşmesini sağlamak için anakartlar üzerinde harici işlemci yanında kart işlemcileri de bulunmaktadır. Chipset olarak da adlandırılan bu işlemcilerin bilgisayar performansı üzerinde çok etkili oldukları bilinmektedir. Chipset’lerdeki gelişmeler işlemcilerdeki gelişmelere paralel olarak ilerlemektedir. Yeni bir RAM ya da bus geliştirildiği zaman bunu işlemciye aktaracak olan Chipsetler de geliştirilir
##### Kuzey Köprüsü (North Bridge)
Anakart üzerinde bulunan, bellek ve AGP ve Güney Köprüsünü işlemciye bağlayan yongadır.
##### Güney Köprüsü (South Bridge)
North Bridge aracılığı ile işlemciye bağlanarak paralel, seri, usb, ps2 gibi düşük hızlı çıkış ve ara birimlerin işlemciye bağlanmasını sağlayan çip'in ismidir. 

<img src="./Pasted image 20241024135325.png" alt="example" />

## ANA kart
#### Bus (Veri yolu)
Bilgisayardaki veri yoluna verilen isimdir. Paralel iletken yollardan oluşur. Byte’ı oluşturan bitleri; paralel olarak 0 veya 1 seviyesinde elektriksel işaretler şeklinde taşır. Anakart üzerinde birçok çeşit bus yapısı vardır. Bu farklılık her bileşenin farklı ihtiyacından kaynaklanmaktadır. Örneğin hafıza veri yolu (memory bus), kuzey köprü (hafıza kontrolcüsü) ile hafıza arasındaki veri yoludur. 

Yeni nesil bilgisayarlarda hafıza ile CPU arasındaki veri yoluna FSB(front-side bus), CPU ile level 2 bellek arasındaki veri yoluna BSB(back-side bus) ismi verilmektedir. Günümüzde PCI, AGP, PCI Express, USB, SCSI, SATA, firewire ve PCMCIA gibi veri yolları vardır. Verileri, bazıları seri bazıları ise paralel olarak iletir. Her bir veri yolu yapısı kendisine has bir slot veya soket yapısına sahiptir. Veri yolları aygıt sürücüleri yardımıyla kontrol edilir. 

__SCSI(Small Computer System Interface):__ Birçok farklı donanım birimini(yazıcı, cd-rom, sabit disk, tarayıcı vb.) destekleyen, aynı veri yoluna birçok donanım biriminin bağlanmasına imkan veren bir veri yolu yapısıdır. SCSI veri yoluna bağlanan her bir donanımın tekil bir numarası(ID) olması gerekmektedir. SCSI-3 versiyonunda Maksimum veri yolu genişliği 16 bit, veri yolu hızı 80 Mhz ve desteklenen donanım sayısı 16'dır. 

__IEEE1394 Firewire:__ Daha çok video, ses, görüntü işleme ve DVD dünyasında kullanılan yüksek hızlarda seri veri aktaran bir yapıdır. I-Link(Sony) ve DV(Panasonic) olarak da isimlendirilir. SCSI'nin daha da gelişmiş şeklidir. Günümüz bilgisayarlarında paralel SCSI'nin yerini almıştır. Firewire bant genişliği 400, 800 ve 3200 Mbit değerlerinde olabilmektedir. Firewire HotPlugging yapıya sahiptir.

__PCI(Peripheral Component Interconnect):__ Ses, ekran, TV ve ağ kartları bağlanabilir. Paralel iletişimi kullanılır. Anakart üzerine onboard olarak veya slotlar yardımıyla bağlanan donanım yapılarını destekler. 

__AGP(Accelerated Graphics Port):__ Hızlandırılmış grafik port'u anlamına gelen AGP, ekran kartları ve video kartları için kullanılan yeni bir veri yoludur. Paralel iletişimi kullanır. 1x, 2x, 4x ve 8x gibi sürümleri vardır. AGP yapısı bir veri yolu olmasına rağmen noktadan noktaya iletimi sağlar.
- PCI veri yolu ile aralarındaki temel fark: AGP'ler 128 KB'a varan büyük texture'ları ekran kartı belleğinin dışında, sistem belleğinden de yararlanarak işler. Bu sayede performansta artış sağlanır. AGP veri yolunun performansta bu şekilde bir artış sağlamasına __"Doğrudan Bellek Kullanımı" DIME(Direct Memory Execute)__ denir. 

__PCMCIA veya PC Card (Personal Computer Memory Card International Association):__ Dizüstü bilgisayarlarda kullanılan genişleme yuvalarının bağlandığı veri yoludur.

__USB(Universal Serial Bus):__ Evrensel seri veri yolu anlamındadır. PnP özelliğe sahiptir. Tek bir bilgisayara 127 adet donanım bağlamaya izin veren bir yapıdır. Günümüzde monitör, klavye, fare, TV kartı, Ses kartı, sabit disk gibi birçok donanım birimi bu veri yolunu kullanmaktadır. HotPlugging yapıya sahiptirler. USB 3.0 Çok yüksek hızlıdır.

__PCI Express:__ En yeni bus yapısıdır. PCI Express, PCI veri yolunda kullanılan paralel veri iletimi mimarisinin yerine seri çalışan ve noktadan noktaya iletişim mimarisini kullanan bir teknoloji getiriyor. Çarpanları, sahip olduğu hat sayısını gösterir. Veriler paketler halinde iletilir. Bus yapısından ziyade ağ mantığı ile çalışır. Veri, seri olarak birkaç hattan gönderilip alınabilir. Bu hatların her birine kanal denmektedir ve çarpanla gösterilir. Veriler anahtarlama yöntemiyle istenen noktalara kanalize edilerek bant genişliğinden bağımsız iletim oluşturulur. Yani her bir kanal için adanmış bir yol anahtarlanarak sağlanır. Haberleşme şekli seridir. Kartlara sağladığı elektriksel güç AGP'den yaklaşık iki kat fazladır. Slot uzunluğu, çarpan sayısı ile doğru orantılıdır. PCI-Express veri yolunun çalışma mimarisi aynı donanım birimlerini ortak çalıştırmak için elverişlidir. 

__Serial ATA(SATA)__, masaüstü bilgisayarlardaki, bazı sunuculardaki ve ağa bağlı depolama cihazlarındaki(HD) paralel ATA fiziksel depolama ara biriminin yenilenmiş versiyonudur. 

##### Portlar
Bilgisayarın dış dünya(modem, klavye, yazıcı, kamera vb.) ile iletişimini sağlayan giriş çıkış kapılarına port denir. Aslında bunlar da birer veri yoludur. Seri, paralel, USB, PS/2... gibi çeşitleri vardır. 

##### BIOS (Basic Input Outpu System ) 
Bilgisayar ilk açıldığında bu sistemin sahip olduğu program kodları ile başlatılır. Bu kodlar eeprom veya flash hafıza denilen yapılarda saklanır. Biosun ilk işi sistem elemanlarını(ekran kartı, sabit disk, Ram...) tanımlamak ve onları kontrol etmektir. Donanım birimleri denetlendikten ve başlangıç parametreleri yüklendikten sonra BIOS disk üzerindeki MBR (Master Boot Record) alanında işletim sistemi açılış dosyalarını arar. İşletim sistemini çağırarak kontrolü ona bırakır. 

##### Chipset
Anakart üzerinde faklı donanımların birbirleriyle iletişimini sağlayan çip'lerdir. Northbridge(kuzey köprü) ve Southbridge(güney köprü) adında iki bileşenden oluşur. Northbridge hızlı bileşenleri(CPU, RAM, PCI Express ve AGP) birbirine bağlar. SouthBridge ise yavaş bileşenleri birbirine bağlar(IDE, USB, PCI...). 

### İşlemciler

1. __ALU(Aritmetik ve Mantıksal İşlem Birimi):__ Toplama çıkarma, çarpma, bölme, mantıksal ve, veya, değil komutları ve kaydırma komutları.

2. __Komut Çözücü(Instruction Decoder):__ İşlemcinin yapması gereken kodların icrası için gerekli işlemleri başlatır ve komutun çalıştırılması için gerekli işlemleri belirler.

3. __Kaydediciler(Registeries):__ İşlemci içerisinde sayıları depolamak için kullanılan hafıza çeşididir. İşlemci veri uzunluğu kadar genişliğe(32, 64 bit) sahiptirler. Literatürde test, EBX, EAX, BX, ES, IP gibi isimler alan kaydedici hafıza gözleri vardır.

4. __Bayraklar(Flags):__ İşlemlerin sonucuna göre 1 ya da 0 değerlerini alan 1 bit genişliğe sahip hafıza gözleridir. Sıfır, işaret, elde, eşlik, taşma gibi çeşitleri vardır. Örneğin bir çıkarma işleminde sonuç sıfır çıkarsa sıfır bayrağı 1 değerini alır.

5. __Veri yolları(Buses):__ İşlemcinin diğer donanım birimleri ile bağlantısını sağlayan iletken elektriksel yollardır. Üç adet veri yolu bulunur. Bunlar veri(data), adres(address) ve kontrol(control) veri yollarıdır. 

<img src="./Pasted image 20241024135719.png" alt="example" />

__1- Klasik İşlemciler:__ Komutlar zaman üzerinde sırayla işlenir. Bir komutun işlenmesi biter. Sonraki komut işlenmeye başlar.
__2- Pipe-Line İşlemciler:__ Bir komutun işlenmesi süreci devam ederken sonraki komutun işlenmesi için hazırlık yapılır.
Bir komutun icra süreci: Fetch, Decode, Execute, write back


__Örneğin:__ 
5 ve 6 sayılarının toplanması ve ekrana yansıtılması işleminin işlemci birimleri tarafından şu şekilde gerçekleşir:
1. Komut alınır : örneğin 5 rakamı belleğin 12345 adresinden alınır.
2. Komut çözülür.
3. Komut çalıştırılır : ALU sayıyı bulur.
4. Komut saklanır : 5 rakamı belleğe geçici olarak saklanır.
5. 1, 2, 3, 4 adımları aynen 6 rakamı için de uygulanır.
6. Komut alınır : toplama işlemi çalıştırılır.
7. Komut çözülür.
8. Komut çalıştırılır : ALU 5 ve 6 sayılarını toplar
9. Komut saklanır : hesaplanan sonuç geçici olarak belleğe saklanır.
10. Komut çalıştırılır : ekranda görüntüleme emri iletilir.
11. Komut çözülür.
12. Komut çalıştırılır : sonuçta hesaplanan sonuç ekranda gösterilir.

__3- HT (Hyper threading ) İşlemciler:__ Hyper-Threading(Çoklu iş parçacıkları) teknolojisi, tek bir fiziksel işlemcinin çok sayıda komut zincirini eş zamanlı olarak işlemesi ile performans artışı sağlamasıdır. Hyper-Threading teknolojisine sahip olan bir işlemci, mantıksal olarak iki adet işlemciden oluşmaktadır. Çip üzerinde tek bir işlemci bulunmasına rağmen programları zaman paylaşımlı olarak çalıştırabilir.
- __Not:__ HT özelliğine izin veren işletim sistemleri ile HT özelliği olmayan işlemcilerle de farklı programlar eş zamanlı olarak çalıştırılabilir. Fakat performans çok iyi değildir.

__4- Çok çekirdekli İşlemciler (Örn: Dual Core İşlemciler):__ İşlemci paketi içerisinde birbirinden bağımsız olarak komutları çalıştırabilen her yapıya çekirdek ismi verilmektedir. Gerçek zamanlı olarak kendisine verilen iş akışı görevlerini aynı anda yerine getirerek performansı artırır. Her çekirdek birbirinden bağımsız FSB ye sahiptir. Tüm çekirdekler L2'yi ortak kullanırlar. Intel Pentium Dual Core, Intel Quad Core ve AMD Athlon X2 serisi çok çekirdekli yapıya sahiptir. 

#### İşlemci ile ilgili Parametreler
1. __Hız:__ Birimi frekans olarak GHz katsayısı(10003) ile değerlendirilir. İşlemcinin hızlı olması işlemlerini daha kısa sürede tamamlaması anlamına gelmektedir. Günümüzde 1.8, 3.0, 3.6 vb. GHz hızlarında olanları vardır.

2. __Bit Genişliği:__ İşlem yapabilme boyutunu gösterir. Günümüzde 64 ve 32 bit işlemciler vardır. İşlemcinin sahip olduğu kaydediciler, veri hattı ve adres hattının genişliğini gösterir.

3. __FSB Hızı:__ İşlemcinin, kuzey köprüsü ile iletişim hızını gösterir.

4. __Level 2 (L2) Cache:__ İşlemciye yakınlığından dolayı bu isim verilir. En yakın olana L1, diğerine L2, L3 gibi isimlendirmeler kullanılır. Yapısı SRAM hafıza tipindedir. SRAM hafızalar, daha hızlı fakat maliyetleri yüksek hafıza çeşitleridir. Yavaş olan RAM erişimlerini azaltmak için işlemci içerisinde yer alan daha hızlı fakat küçük boyutlardaki hafızaya verilen isimdir. İşlemcinin hafıza kontrol devresinden(MCH) istekte bulunduğu her kod bu belleğe yazılır. İşlemci aynı kodu RAM yerine daha hızlı olan bu bellekten alır. Intel Core2 Dua'larda 4MB, Intel Core2 Quad'larda ise 8MB bellek miktarı vardır. RAM'den tipik olarak 4 kat daha hızlı çalışmaktadır.

5. __Silikon teknolojisi:__ Piyasada şu anda bulunan işlemcileri oluşturan bileşenler arasındaki mesafe bir metrenin 45 milyarda biri genişliğindedir(45nm teknolojisi). Transistörlerden 2000 tanesini yan yana koyduğunuzda bir insan saç telinin çapı (0.09 mm) kadar bir genişliğe ulaşılır. Silikon dioksit yerine hafniyum oksit kullanımıyla yeni transistörlerde daha az enerji kaybı, daha az ısınma ve daha hızlı geçişler sağlanır.

<img src="./Pasted image 20241024135950.png" alt="example" />

### RAM

- Bilgisayarda verilerin geçici olarak depolandığı hafıza birimidir. CPU'nun ihtiyaç duyduğu kodları sakladığı için hızlı ve kapasitesinin çok olması performansa doğrudan etki edecektir. Rastgele erişimli olması sayesinde belleğin sıra gözetmeksizin istenen adresindeki veriler okunup yazılabilir.
- Disk, CDROM ve I/O portlarından gelen ve giden veriler geçici olarak RAM üzerinde işlenmek üzere tutulur. RAM'ler üzerindeki bilgiyi tutabilmeleri için elektrik enerjisine ihtiyaç duyarlar. Elektrik enerjisi kesildiğinde üzerilerindeki veriler de kaybolur. 
- RAM, her bir hücresi bir transistör ve kapasitörden oluşan 2 boyutlu(satır ve sütunlar) matris yapıya sahiptir. Hücreler şarj edilirken hücre hücre değil, satır satır edilir. Verileri tazeleme oranı(refresh rate) satır bazında değerlendirilir. Örneğin 2K tazeleme oranına sahip bir bellekte 2048 adet satır tazeleniyor demektir. 
- Günümüzde DDR SDRAM(double-data-rate synchronous dynamic random access memory), DDR2 SDRAM, DDR3 SDRAM ve SDRAM yapıda hafıza ürünleri kullanılmaktadır. 
- Daha ucuz ve küçük boyutta olduğundan bilgisayar ana belleğinde DRAM kullanımı tercih edilirken SRAM hızından dolayı öncelikle cache bellek için kullanılır. 

__SDRAM(Synchronous Dynamic RAM):__ 64 bit veri genişliğine sahiptir. Günümüz bellek yapılarından en az band genişliğine sahiptir. DDR çeşit RAM'lerin temelini oluşturur ve onlardan en az iki kat yavaş çalışır. Dinamik bellek yapısındadır.

__DDR SDRAM:__ 64 bit veri genişliğine sahiptir. Veri transferi için, saat(clock) işaretinin alçalan ve yükselen kenarlarını kullanan yapıya sahip, SDRAM çeşididir. Dolayısıyla SDRAM' e göre iki kat hızlıdır.

__DDR2 SDRAM:__ 64 bit veri genişliğine sahiptir. DDR SDRAM ile aynı yapıda olup aynı saat hızında çalışırlar. Aralarındaki fark latency(istenen adrese ulaşmak için harcanan zaman) değerinin DDR da daha büyük olması ve daha fazla güç gereksinimidir. Ayrıca burada belleğin, I/O bus frekansı DDR'a göre iki katı hızda çalışmaktadır. 

__DDR3 SDRAM:__ 64 bit veri genişliğine sahiptir. DDR yapıya sahiptir. Fakat en az güç gereksinimine sahiptir. DDR2 ye göre dahili geçici hafıza miktarı büyüktür. DDR3' ün, I/O bus frekansı DDR2'ye göre iki katı hızda çalışmaktadır.

<hr>

__Kapasite:__ Bir RAM’ın kapasitesi yani x-baytlık kaç tane farklı adresleme olduğudur.

__Hız:__ Bir işlemci RAM üzerindeki veriye ihtiyaç duyduğunda hafıza kontrol devresine (MCH-Memory Control Hub) istekte bulunur. MCH bu isteği RAM'e aktarır ve MCH veri okunmaya hazır olduğunda bunu CPU'ya rapor eder. RAM'in aldığı bi talebe karşılık vermesi için geçen süreye Access Time denir. Hafıza modülleri 50-80 ns arasında değişen Access Time sürelerine sahiptir. Sürenin kısa olması modülün hızını gösterir.

### Önbellek (Cache)
- Bilgisayar hızını belirleyen en önemli faktörlerden biridir.
- SRAM'lerden oluşmuş bellek topluluğudur.
- Çalışma şekli: işlenecek olan bilgi alınmak istendiğinde ilk defa buraya uğranır.
- Kullanım amacı: işlenecek olan bilgi işlemeden önce buraya getirilerek bilgilerin işlenmeye hazır hale getirilmesidir. 
- Genellikte işlemcilerde kullanılır ve işlemcinin hızını belirleyen en önemli faktörlerden birisidir. 
- Normalde işlenecek bilgilerin hepsi bilgisayarın ana bellekte yani RAM'de bulunur.
- İşlemci verileri işlemek için yol sistemleri ile ana belleğe gider, oradan işleyeceği bilgiyi alır ve işler. Ana belleğin ve yolların hızı işlemcinin hızına yetişemez. İşlemcinin her veri işleme ihtiyacında ana belleğe gitmesi zaman kaybına yol açar ve işlemci yeteri kadar verimli kullanılmaz. İşte bu yavaşlığı önlemek için önbellekler kullanılır. 

### Sabit diskler (Hard-disks)
- Sabit diskler, üzerilerine kalıcı olarak bilgi depolanabilen ve depo edilmiş verilerin okunabildiği manyetik ortamlardır. Sabit disklerin bilgi depolama kapasitesi disketlerden çok yüksektir, Günümüzde 1- 2 TB'lık sabit diskler yaygın olarak kullanılmaktadır.
- Sabit disklerde bilgi kaydedilen bölüm (disk plakaları-bunların üst üste gelmesiyle silindir oluşur), mıknatıslanmayan metal bir yüzey(alüminyum) üzerine kaplanmış demir grubu (demir, nikel, kobalt vb.) oksitlerden oluşan bir tabakadır. 
- Her bir diskin her iki yüzü için birer adet okuma/yazma kafası(head) vardır(Yani her diskte 2 tane).
- Sabit disk üretildikten sonra formatlanmadan kullanılamaz. Formatlama işlemi yapılınca disk yüzeyinde iç içe daireler şeklinde izler(track) oluşturulur. Bunlar gerçekte disk üzerine çizilmiş izler olmayıp bilgilerin adresleme biçimidir. Disk üzerinde oluşturulan izler bilgilerin kolayca bulunmasını sağlamak için sector(dilim)'lere bölünür.
- Kümeler(Cluster) ise İşletim sisteminin disk yönetimi ile alakalıdır. Dosya ve dizinlerin yerleştirildiği en küçük disk alanına denir. Boyutu dosya sistemine göre değişir.

### Disk Parametreleri
__Disk Dönüş Hızı(RPM=Rotate Per Minute):__ Diskin dakikadaki dönüş hızını gösteren bir parametredir. Günümüzde 15.000 rpm, 7200 rpm değerlere sahip diskler bulunmaktadır. 

__Tampon Bellek(Cache veya Buffer):__ Disk erişimi bellek erişiminden daha yavaş olduğu için disk performansını artırmak için HDD üzerine bellek hafıza birimleri yerleştirilmiştir. Amaç erişilmesi öngörülen verileri bellekte hazır bekletmektir. Eğer istenen veri bellekte varsa disk erişimi olmadan veriler doğrudan bellek üzerinden gönderilir.

__Konumlanma Süresi(Seek Time):__ Disk üzerinde okuma yazma kafasının, istenen adrese yazma veya okuma amaçlı ulaşmak için harcadığı süredir. Kafanın disk üzerindeki konumuna göre bu süre kısalıp uzayabilir. Bunun için ortalama konumlanma süresinden(average seek time) bahsedilir. HDD'lerde erişim süresi ms’ler mertebesindedir.

__Kapasite:__ Depolayacağı veri miktarını gösterir. Günümüzde 1 TB, 4 TB kapasiteli diskler bulunmaktadır.

__Spin Up:__ işletme hızına diski hızlandırma zamanı.

__Seek Time:__ İstenen Track’i bulma zamanı

__Rotational Time:__ istenen sektörü bulma zamanı

__Transfer Time:__ Veri okuma veya yazma zamanı.

Bir sabit diskin kapasitesi şu şekilde hesaplanır: 
 `Silindir sayısı*Sektör Sayısı*kafa sayısı*512
- 1024 silindir, 256 kafa ve 63 sektör parametrelerine sahip bir sabit diskin kapasitesi: `1024*256*63*512=845571864 byte`’dır. Bu da yaklaşık 8.4 Gigabyte’dır. 

__Serial portlar__ ile, veriyi oluşturan bitleri 1,0 sinyal katarı art arda (her bir clock süresince tek bit) olarak iki nokta arasında tek bir iletişim ortamı ile gönderebilirsiniz. 

__Parallel portlar__ ile bir baytlık(veya daha fazla) bilgiyi tekbir zaman diliminde karşı tarafa gönderebilirsiniz. Bit sayısı kadar iletişim yolu olmalıdır.

__USB (Universal Serial Bus):__ Kendisini configure edebilen akıllı bir seri arayüzdür. Tak-Çalıştır’ı destekler.

### Monitör
- Katot Işınlı Tüp(CRT-Cathode Ray Tube) denilen bu tüp, havası boşaltılmış mühürlenmiş bir cam konidir.
- Koninin geniş tarafı düz ve dikdörtgen biçimindedir. Bu, monitörün ekranını oluşturan taraftır. Koninin öbür tarafı dardır ve katot levhaları ile küçük tel ızgaraları içerir. Bu katot levhaları ısıtıldığında tüpün içinde serbestçe dolaşan elektron bulutları oluştururlar.
- Katot negatif olarak yüklenirken, dış kısmına pozitif bir yüksek gerilim uygulanarak katot ışınlı tüpün anot'u veya pozitif kutbu oluşturulur. Anot ve katot arasındaki büyük gerilim farkı, bu serbest elektronların ekrana doğru fırlatılmalarına neden olur.

__Çözünürlük(Resolution):__ Çözünürlük, ekran kartının gönderdiği görüntüyü dikey ve yatay olarak ifade ederken kullandığı piksel sayısıdır. 

__Boyut:__ Ekranın fiziksel uzunluğunu ekranın boyutları belirler. 14 inch'lik bir monitörün genişliği yaklaşık olarak 11 inch'tir.

__Tazeleme Oranı (Refresh Rate):__ Elektron tabancası, CRT'nin noktacıklarını üst sıradan başlayarak en alt sıraya kadar tarar. Bundan sonra elektron tabancası, grafik kartından kendisine gelen diğer ekran görüntüsünü CRT üzerinde oluşturmak üzere tarama işlemine devam eder. Bir tam ekran tarandıktan sonra yeni bir görüntü oluşturmak üzere tarama işleminin başlamasına ekranın tazelenmesi denir. Bu tazeleme olayının saniyede kaç kez tekrarlandığı ise tazeleme hızıyla ölçülür. Saniyede 60 Hz'lik tazeleme hızına sahip olan bir monitör, o sırada saniyede 60 ekran taramaktadır. 

- Bir monitörün satır sayısı ile düşey tarama frekansının çarpımı __yatay tarama frekansını__ verir. Bu, elektron demetinin, ekranın solundan sağına saniyede kaç defa gidileceğini gösterir. Buna göre 480 satır çözünürlüğünde ve 70 Hz düşey tarama frekansına sahip monitörün; 480*70 veya 33600 Hz (33.6 KHz)'dir. Bu durumda elektron demeti saniyede 33600 satırı tarayacaktır.

__Nokta Aralığı (Dot Pitch):__ Aynı renkteki iki noktanın, merkezleri arasındaki uzaklık nokta aralığı(dot pitch) olarak adlandırılır. Nokta aralığının değerleri 0.25 mm ve 0.28 mm arasında değişir. Nokta aralığı ne kadar küçük olursa, daha net görüntü anlamına gelir.

### LCD Liquid Crystal Display
- LCD monitörlerde görüntü sıvı kristal diyotlar yardımıyla sağlanmaktadır. Bu diyotlara gerilim uygulandığında, içlerindeki moleküllerin polarizasyonu değişmekte ve beraberinde de diyot'un geçirgenliği değişmektedir.
- Normalde şeffaf olan bu diyotlara gerilim uygulandığında geçirgenliklerini kaybederler ve siyaha dönerler. Renkli LCD monitörlerde ise çok ufak ve birden fazla diyot kamanı kullanılarak görüntü alınmaktadır.
- LCD monitörler DSTN ve TFT olmak üzere ikiye ayrılmaktadır. Ucuz olan ve “passive matrix” teknolojisini kullanan __DSTN (Dual-Scan Twisted Nematic)__’ler çözünürlükleri ve görüş açıları TFT’lerden düşük olan monitörlerdir. Bu monitörler genelde dizüstü bilgisayarlarda kullanılmaktadır. __TFT (Thin Film Transistor)__’ler ise “active matrix” adı verilen ve görüntüyü daha parlak ve keskin gösteren bir teknoloji kullanırlar. TFT’lerde her piksel bir ya da dört transistör tarafından kontrol edilir ve bu sayede flat panel ekranlar arasında en iyi çözünürlüğü sunarlar.

### Standardizasyon
 Bilgisayar donanım standartlarını belirleyen birkaç önemli organizasyon vardır:
- The Institute of Electrical and Electronic Engineers (IEEE) 
- The International Telecommunications Union (ITU) 
- The American National Standards Institute (ANSI)
- The British Standards Institution (BSI) 
- The International Organization for Standardization (ISO)

### Bellekler
Büyük ana bellek kapasitesi olan bilgisayarlar daha büyük programları, daha küçük ana bellekli bilgisayarlara göre daha hızlı çalıştırırlar. Rastgele erişim(random access), hafıza uzayındaki herhangi bir yerdeki bilgiye aynı sürede erişilebilir anlamındadır.
__Önbellek (Cache):__ RAM’den daha hızlı erişilebilir geçici bir bellek türüdür.
### SSD’ler hakkında
Mekanik olarak çalışan hard-disklerin yerini alan yeni nesil hard-diskler SSD olarak
anılmaktadır.
- SSD, Solid State Drive kelimesinden kısaltılmıştır.
- SSD diskler günümüzde SATA SSD ve NVMe SSD olarak iki farklı veri yoluyla karşımıza
çıkmaktadır.
- Türkçeye çevrildiğinde çok anlamlı bir kelime dizisi çıkmasa da önünde bulunan ön ek
NVMe daha anlamlı bir kelime dizisi oluşturmaktadır.
- __NVMe(Non-Volatile Memory Express):__ Silinmeyen(Uçucu olmayan) Süratli Bellek
anlamında kullanılır.
- NVMe’deki e harfi yeni nesil PCIe veri yolundan esinlenerek oluşturulmuştur. Başka bir ifadeyle de PCIe arayüzünün NAND belleklerinin gerçek gücünü ortaya çıkarabilmesi için geliştirilmiştir ve ismindeki express kelimesinin de bir sonucu olarak hard-diskten ziyade hızlı bellek gibi çalışarak sürücünün daha hızlı çalışmasına imkan sağlar. Ayrıca düşük güç tüketimi, ölçeklenebilirlik ve standartlara uyumluluk özelliklerine de sahiptir.
- SATA’yla birlikte PCIe destekli SSD’lerde mevcuttur. Çünkü SATA’dan sonra çalışan en yüksek bant genişliğine sahip veri yolu PCIe’dir. PCIe veri aktarımında kanal sayısının fazla olması nedeniyle hız konusunda SATA’nın önüne geçmiştir. SATA yavaş çalışan sabit diskler için oluşturulmuş AHCI protokolünü desteklediği için SSD disklerin hızları 550 MB/s ile sınırlanmıştır. Bu olumsuzluklardan ötürü geliştirilen NVMe arayüzü ise SSD diskleri 7000 MB/s gibi bir seviyeye taşımıştır.
- Teknolojik olarak incelediğimizde, hareketli parçaları olmayan ve neredeyse anında erişim süreleri olan NAND flash bellek adı verilen basit bir bellek yongası kullanırlar.
- SSD benzeri teknoloji ile ilgili ilk deneyler 50'lerde başlamış, 70-80'lere gelindiğinde askeri ve havacılık sektöründe kullanılmaya başlanmıştır. Fakat teknolojinin son derece pahalı ve depolama kapasitesinin de o oranda düşük olması (2MB-20MB) kullanıcı bilgisayarlarına girmesini geciktirmiştir.
- Bir SSD üzerindeki bellek yongaları, RAM ile karşılaştırılabilir.
- Dosyalar, manyetik bir disk yerine, NAND flash hücrelerinden oluşan bir ızgaraya kaydedilir.
- Her bir ızgara (bloklar olarak da isimlendirilir) 256 KB ile 4MB arasında veri depolayabilir.
- SSD denetleyicileri, blokların tam adresine sahip olduğu için bir dosya istediğinde (neredeyse) anında kullanılabilir hale gelir.
- Bu nedenle SSD erişim süreleri nano saniye cinsinden ölçülür.

- __NAND flash bellek__, verileri korumak için enerji gerektirmeyen, kalıcı bir depolama teknolojisidir. Birkaç transistörün seri olarak bağlandığı ve verileri kaydırmalı geçit transistörlerle bellek hücreleri dizilerinde depolayan flash bellek türüdür. Kontrol kapısı ve kayan kapı olmak üzere iki kapı içerir ve tek bir hücreyi programlamak için kontrol kapısına bir voltaj yükü uygulanır. Elektronlar daha sonra kontrol kapısına doğru çekilir, ancak kayan kapı onları normal çalışma koşullarında yıllarca kalabilecekleri alt tabaka içinde hapseder.
- Bir hücreyi silmek için, kontrol geçidi topraklanmalı ve karşı tarafa veya alt tabakaya bir voltaj uygulanmalıdır. Sürekli silme, yazma ve okuma NAND flash bileşenlerini yıpratır. Bu nedenle SSD disklerin Total Bytes Written adı verilen bir yaşam döngüsü vardır ve bu döngüye göre SSD disklerin kullanımı için okuma, yazma ve silme işlemlerinin Toplam Byte olarak bir karşılığı bulunmaktadır.

## RAM vs SSD
- RAM’ler tipik olarak 45 GB/sn hızındadırlar. SSD ise maks 7GB/sn.
- RAM bilgiyi unutma meyillidir. SSD unutmuyor.
- RAM kuzey köprüsüne bağlıdır. SSD NVMe / PCIe veri yolundadır.
- RAM 64-512GB, SSD 500GB-100TB aralıkta.
- İkisi de 64 adres limiti içindedir.
- RAM’de yazma ömrü yok, SSD belli bir ömre sahip.
- RAM 100-400 saat sinyalinde cevap verir, SSD ise farklı veriyolunda ve binlerce saat sinyali sonra cevap veriyor.

## Sanal Bellek
Şu ana kadar anlatılan bellek sisteminin üç temel sorunu vardır:
1. Sistemde tüm programların gereksinimlerini karşılayacak kadar büyük bir bellek olmayabilir.
2. Programcı programın çalışacağı sistemdeki bellek boyutunu bilemez.
3. Programcı kendi programı yanında hangi programların çalışacağını bilemez. 

	Bu sorunları çözmek için sanal bellek (virtual memory) kullanılır. Her programın kendi sanal adres uzayı vardır, programdaki adres referansları sanal adres referansıdır. Her programa atanmış bir fiziksel bellek bölümü bulunmaktadır.

- Sanal bellek yönteminde sanal adresler kullanılır. Sanal adresler farklı
fiziksel adreslere karşılık gelir. Bu sayede programcı gerçekte hangi fiziksel
adreslerin ona atandığını bilmeden program yazabilir.

- Programların birbirlerine ayrılmış belleklere doğrudan erişimi yoktur. Bu
sayede sanal bellek güvenliği de sağlar. Ayrıca sanal bellek yöntemi ile ana bellek ve ikincil bellek arasında veri akışı
ile bellek sınırsızmış yanılsaması sağlanabilir.

- İkincil bellek ile ana bellek arasındaki veri akışı sayfalar aracılığı ile yapılır.
Sayfalar sabit boyutlu bellek bloklarıdır.

- Belleğe erişim için sanal adreslerin fiziksel adreslere dönüştürülmesi
gerekir. Bu işleme adres dönüşümü(page translation) denir.

<img src="./Pasted image 20241024141235.png" alt="example" />

<img src="./Pasted image 20241024141247.png" alt="example" />

## Sayfa Tablosu
Yapılan sanal ve fiziksel sayfa eşleşmelerini daha sonra dönüşümde kullanmak için bir yerde tutmamız gerekir. Bu eşleşmeler sayfa tablosu(page table) isimli bir yapıda bellekte tutulur. Sayfa tablosunun adresi bir yazmaçta tutulur. Erişim yapılacağı zaman bu adresle tabloya erişilir.

<img src="./Pasted image 20241024141351.png" alt="example" />

## Etkin Sayfalar Önbelleği
Dönüşüm için işlemcide tutulan önbelleğe etkin sayfalar önbelleği (translation lookside buffer) denir.
#### Sayfa Hatası
Sayfa tablosunda da sayfa bulunamazsa ne olur?
Sayfa hatası(page fault) sanal sayfaya karşılık gelen fiziksel sayfa ana bellekte bulunamadığı zaman olur. İki nedeni olabilir:
1. Fiziksel sayfa ikincil bellektedir.
2. Fiziksel sayfa henüz atanmamıştır.

- Sayfa hatası olduğu zaman denetim işletim sistemine geçer. İşletim sistemi sayfayı ikincil bellekte bulmaya çalışır. Önceden hangi sayfaların ikincil belleğe alınacağını bilemediğimiz için ikincil bellekte bu sayfalar için ayrılmış bir bölüm bulunur, bu bölüme takas dosyası(swap space) denir. Aynı zamanda bu bölümdeki sayfaların nerede durduğunun da kaydını tutan bir yapı oluşturur. (Sayfa tablosunda da tutulabilir, ayrı bir tablo da olabilir.) Sayfa ikincil bellekte bulunursa belleğe getirilmesi gerekir. Bellekte yazılacak yer yoksa, bir sayfa seçilir ve ikincil belleğe yazılır. Getirilen veri de onun yerine yazılır.

- Sayfa hatasının bir diğer sebebi de henüz herhangi bir sayfanın sanal adrese eşleştirilmemiş olmasıdır.
	1. Bu durumda işletim sistemi boş bir fiziksel sayfayla sanal sayfayı eşleştirir ve eşleşmeyi sayfa tablosuna yazar.
	2. Ana bellekte boş fiziksel sayfa yoksa, bir sayfa seçilip ikincil belleğe yazılır ve boşalan yer yeni dönüşüm için ayrılır.
	3. Sayfa tablosu ve ESÖ güncellenir. 
- İşletim sistemi sayfa hatasına sebep olan buyruğu kaydettiği için oradan itibaren program yürütülmeye devam eder.

## Yazma İşlemi
Bellek hiyerarşisinde önbellek ve ana bellek için yazma işlemleri iki şekilde yapılabilir: 
1. doğrudan yazma
2. sonradan yazma

Sanal bellek için ise ikincil bellek ve ana bellek arasındaki gecikme çok fazladır. İkincil belleğe yazma işlemi çok uzun süreceği için sanal bellek sisteminde bu iki seviye arasında her zaman sonradan yazma yöntemi uygulanır.

<img src="./Pasted image 20241024141616.png" alt="example" />

## Bilgisayar Başarımı (Performans)

<img src="./Pasted image 20241024141641.png" alt="example" />

<img src="./Pasted image 20241024141654.png" alt="example" />

<img src="./Pasted image 20241024142006.png" alt="example" />

<img src="./Pasted image 20241024142016.png" alt="example" />

<img src="./Pasted image 20241024142150.png" alt="example" />

## Ortalama Clock Cycle’ı
- Bir programda execution time (yürütme zamanı) doğrudan doğruya komutların sayısına
bağımlıdır. Buna göre, bir programın yürütme zamanı hesabı için başka bir yolda; yürütülen komutların sayısı ile, her komut için harcanan ortalama zamanın çarpılmasıdır.
	__`CPU execution time = CPU clock cycles x clock cycle time`__ (CPU yürütme zamanı = CPU clock sayısı x clock periyodu) Veya
	__`CPU execution time = Programdaki komut sayısı x CPI x clock periyodu`__
Farz edin ki aynı komut seti mimarisi ile gerçekleştirilmiş iki farklı makineye sahibiz. Ama programlama için farklı komutlar kullanılabilir.

__Örneğin:__
- A makinesinin Clock cycle süresi(Clock Periyodu)=250 ps ve aynı program için 3.0 CPI'ya sahiptir.
- B makinesinin Clock cycle süresi(Clock periyodu)=500 ps ve 1.2 CPI'ya sahiptir. 
- Bu program için hangi makine daha hızlıdır. Ne kadar hızlıdır?
- Eğer iki makine aynı ISA’ya sahipse clock rate, CPI, yürütme zamanı, komutların sayısı ve MIPS daima benzer olacaklar mıdır?
	 - Verilere göre her iki bilgisayarda, aynı program için benzer sayıda komut işler. Bu sayıya I (Instruction sayısı) diyelim. 
	 - Her bir bilgisayar için clock cycle (Clock periyot) sayısını bulalım. 
	 - __`CPU clock cyclesA = I x 3.0 `__
	 - __`CPU clock cyclesB = I x 1.2`__
	 - Buradan her bir bilgisayar için CPU time’i hesaplayabiliriz.
	 - __`CPU timeA = CPU clock cyclesA x Clock cycles timeA = I x 3.0 x 250 ps = I x 750 ps`__
	 - __`CPU timeB = CPU clock cyclesB x Clock cycles timeB = I x 1.2 x 500 ps = I x 600 ps`__
	 - Anlaşılacağı gibi B bilgisayarı daha hızlıdır.
	 - __`PerformanceA / PerformanceB= Execution timeB / Execution timeA= n = Ix600ps / Ix750ps = 0.8 CPU time = komut sayısı x CPI x Clock cycle (Clok periyodu) time`__

<img src="./Pasted image 20241024142412.png" alt="example" />

## Kod Segmentlerinin karşılaştırılması

__Örneğin:__
- Bir derleyici tasarımcısı iki kod dizileri arasında karar vermeyi deniyor. Donanım aşağıdaki mimarileri desteklemektedir.
- 3 farklı komut sınıfı vardır. A, 1 cycle, B, 2 cycle, C 3 cycle ihtiyaç duyuyor.
- İlk kod dizisi 5 komuta,(A=2, B=1,ve C=2)
- İkinci kod dizisi 6 komuta sahiptir. (A=4, B=1 ve C=1.)
- Hangisi size göre daha hızlıdır. Ne kadar?
- Herbir dizi için CPI?

  	<img src="./Pasted image 20241024142436.png" alt="example" />
- Bu örnek gösterir ki; performans değerlendirme için yalnızca bir kıstas olarak kullanmak yanıltıcı olabilir. 
- İki bilgisayarı performans açısından karşılaştırmak için, (yürütme zamanı-execution time) her üç bileşeni(Komut sayısı, CPI, Clock Cycle time(periyot)) dikkate almak gerekir. 
- Eğer bileşenlerden bir kısmı özdeş ise, performans karşılaştırması özdeş olmayan bileşenlere göre yapılır. Örneğin her iki bilgisayarın frekansları ayni ise karşılaştırma, komut sayısı ve CPI’ya göre yapılabilir.
- Performansa ve CPI’ye etki eden en büyük faktör ise PIPELINE mimarisidir.

## Performans değerlendirilmesi
- İki veya daha fazla bilgisayar arasındaki performans değerlendirmesini nasıl
yaparız?
- İki bilgisayarın performansını değerlendirmek için; bu iki bilgisayarda bir workload(tanımlı bir işlemler kümesi programı)’un execution time'ları karşılaştırılır.
- __Benchmark:__ Bir ölçme veya değerlendirme standardıdır. Bir bilgisayar benchmark'ı, tipik bir şekilde tanımlı workload’u gerçekleştiren bilgisayar programıdır.
- Bilgisayar benchmark için ölçülen metrikler:
	- __Hız:__ Bir workload’ın ne kadar hızlı tamamlandığı.
	- __Throughput:__ Bir birim zamanda tamamlanan workload unit’idir.
- Birden fazla bilgisayarda aynı bilgisayar benchmark'ı çalıştırılarak bir karşılaştırma yapılmasını sağlar.

## Performans Raporu
- Hazırlıktan sonra performans ölçümleri seçilen uygun kriterler kümesinden elde edilir.
- __Tekrarlanabilirlik:__ Rapordaki diğer her şey dahil, deneyler rapor edilen sonuçları çoğaltmak için tekrarlanabilirlik gerekir. (O/S version, derleyici, giriş, bilgisayar konfigürasyonu, gibi) 
- Girişlerin seçimi çok önemlidir. Büyük girişler bellek sistemini değerlendirmek için gereklidir. 
- Ayrıca büyük iş yükü gereklidir.

<img src="./Pasted image 20241024142604.png" alt="example" />

<img src="./Pasted image 20241024142628.png" alt="example" />

<img src="./Pasted image 20241024142651.png" alt="example" />

<img src="./Pasted image 20241024142700.png" alt="example" />

<img src="./Pasted image 20241024142710.png" alt="example" />

<img src="./Pasted image 20241024142723.png" alt="example" />
