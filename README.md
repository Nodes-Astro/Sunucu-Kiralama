# Sunucu-Kiralama


### ℹ️ Daha önce node kurmak için sunucu kiralayıp node kurmadıysanız bu rehberden faydalanabilirsiniz.



![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/7288623f-763c-4d23-a571-b932fea4dd5a)

#### Öncelikle ben node operasyonları için Hetzner'i kullanıyorum, size sunucu kiralamayı Hetzner üzerinden göstereceğim.

#### ℹ️ Bu ref kodu ile kayıt olup 20€'luk sunucu kiralama hakkı kazanabilirsiniz:

https://hetzner.cloud/?ref=zKv7TRa1TOGx

## Neden Hetzner?

#### ℹ️ Hetzner size saatlik ücret çıkarır, yani sadece 1 saatlik işinizi görecek kiralamalar için 1 aylık kiralama ücreti ödemezsiniz. Saatlik kesilen ücrete göre ayda 1 faturanızı ödersiniz.

#### ℹ️ Ayrıca oldukça yeterli bir internet hizmeti vermektedir, bandwith ve hız konusunda problem çıkarmamaktadır.

#### ℹ️ Bunlara nazaran kiralama ücretleri de uygundur.

## Gereklilikler

#### ℹ️ Öncelikle linkten üyelik oluşturmamız gerekli. Üyeliği başarılı bir şekilde oluşturduktan sonra karşımıza Passport bölümü çıkacaktır. Burada KYC yapmanız gerekmektedir. Gerekli bilgilerinizi girerken doğruluğuna özen gösterin yoksa birkaç gün sonra sorun yaşayabilirsiniz.

#### ℹ️ KYC aşaması için bütün bilgileri girdikten sonra onaylanması için beklememiz gerekiyor, onay aldığımızda artık sunucu kiralayabiliriz.

## Sunucumuzu Seçiyoruz

#### Anasayfada sağ yukarıda Cloud sekmesine tıklayalım.

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/da074369-3f1c-490a-b367-128cb1af2b99)

#### New Project diyoruz, isim veriyoruz.

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/6d98fc9f-8cc9-41b0-84d5-b290da1b151a)

#### Add Server diyoruz

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/0a2243ab-3a31-4b8b-920c-e89176d92ba8)

#### Lokasyonumuzu seçiyoruz, sistem olarak Ubuntu 22.04 seçiyoruz.

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/d11b7203-1e60-4798-b854-cfe23857f4d5)

#### ℹ️ Makinemizi seçerken bizi Shared ve Dedicated vCPU karşılıyor. Shared x86 işaretliyoruz ve bize uygun sistem özelliklerine göre bir makine seçip devam ediyoruz. (Dedicated daha çok hassas operasyonlar için terich edilir ve daha pahalıdır.)

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/9678d140-4f11-4c00-9c3a-86abe64eb4f8)

#### Ardından başka bir değişiklik yapmadan mouse'umuzu en aşağıya kadar kaydırıyoruz, makinemizin ismini giriyoruz ve en sağ altta "Create & Buy Now" diyoruz ve böylelikle makinemizi kiralıyoruz.

## Terminal Kullanımı

#### ℹ️ Makinemiz bizim için kullanıma hazır hale geldikten sonra terminal kullanıp ssh ile bu makineye uzaktan erişerek node'umuzu kurabiliriz.

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/e464cd8d-46d7-4466-b93b-d1d8dab63584)

#### Bunun için bir uygulama kullanmamız gerekiyor, ben kullanışı pratik olduğu için Termius'u tercih ediyorum ve rehberde Termius üzerinden anlatacağım. Aşağıdaki linkten windows için indirebilirsiniz:

https://termius.com/download/windows

#### Öncelikle Hetzner'e kayıt olduğunuz maili kontrol edin, kiraladıktan sonra size ip ve hashli şifre veriyor.

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/afb7bc72-bed4-4463-9ebe-cb0e34f307e7)

#### Termius'u indirip kurduktan sonra içine girelim ve "Create Host"'a tıklayalım.

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/60a5b2af-52fb-4fff-89b4-8aeba8d4f908)

#### Gerekli yerleri aldığımız maile göre dolduralım:

##### - Address: Ipv4 adresimiz

##### - SSH için "22" nolu port

##### - Username: root

##### - Şifre: Mailden gelen hashli şifremiz

#### Ardından sağ aşağıdan connect diyoruz ve continue diyip terminale giriş yapıyoruz.

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/1bcac9eb-6ded-4d09-af50-a0af41017bea)

#### Bizi böyle bir ekran karşılıyor ve yine mailden aldığımız şifremizi giriyoruz

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/cac71b25-020d-4587-978d-f82be9d44f87)

#### Ardından bizden yeni şifre istiyor 2 kez şifremizi giriyoruz (güçlü şifre oluşturalım)

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/84d3467d-e4eb-4af3-abd1-dda0ef15a2f3)

#### Yeni şifremizi girdikten sonra artık ssh ile bağlantı kurduğumuz makinemize kendi bilgisayarımızdan uzaktan erişebiliriz 🎉

#### Konsolu kapatın ve yeniden bağlanmayı deneyin. Termius sizin için kaydedecektir, üzerine çift tıklayın ve yeni oluşturduğunuz şifrenizi girin. Artık node kurulumları yapabilirsiniz, hayırlı olsun!

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/c9480fd6-3cc0-48bf-9ab7-e3d538b073a9)


## Terminal Hakkında Ek bilgiler

#### ℹ️ Sağ taraftan gözünüze hitap eden temayı seçebilirsiniz.

![image](https://github.com/Nodes-Astro/Sunucu-Kiralama/assets/105454859/e76f0839-67c4-483f-a67d-0ef1abfb2311)

#### ℹ️ Ayrıca Termius yazdığınız komutların datasını tutarak size kolaylık sağlar ve varsayılan ayarlarında timeout 0'dır yani disconnect olmazsınız.



















