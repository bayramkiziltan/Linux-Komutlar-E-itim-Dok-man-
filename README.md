# **Linux Komutları Eğitim Dokümanı**

## **1. Giriş**

### **Linux Nedir?**

Linux, açık kaynak kodlu ve özgür bir işletim sistemi çekirdeğidir. 1991 yılında Finlandiyalı bilgisayar mühendisi Linus Torvalds tarafından geliştirilmeye başlanmıştır. İlk olarak Unix işletim sistemine alternatif olarak tasarlanan Linux, zaman içinde geniş bir geliştirici topluluğunun katkılarıyla büyümüş ve dünya genelinde yaygın bir kullanım alanı bulmuştur.

#### **Linux'un Özellikleri ve Avantajları**

- **Açık Kaynaklı ve Özgür Yazılım:**
  - Linux'un kaynak kodu herkese açıktır. GNU Genel Kamu Lisansı (GPL) altında dağıtılır, bu sayede kullanıcılar yazılımı istedikleri gibi inceleyebilir, değiştirebilir ve dağıtabilirler.
- **Güvenilirlik ve Kararlılık:**
  - Linux sistemleri, yüksek kararlılıkları ve uzun çalışma süreleri ile bilinir. Sunucular ve kritik görevler için idealdir.
- **Güvenlik:**
  - Linux, güçlü güvenlik özelliklerine sahiptir. Kullanıcı izinleri ve erişim kontrol mekanizmaları sayesinde virüs ve zararlı yazılımlara karşı daha dayanıklıdır.
- **Esneklik ve Özelleştirilebilirlik:**
  - Kullanıcılar, ihtiyaçlarına göre sistemi özelleştirebilir. Farklı masaüstü ortamları, pencere yöneticileri ve uygulamalar arasından seçim yapabilirler.
- **Donanım Desteği ve Performans:**
  - Geniş bir donanım yelpazesini destekler ve eski veya düşük özellikli cihazlarda bile verimli çalışabilir.
- **Topluluk ve Destek:**
  - Dünya çapında aktif bir geliştirici ve kullanıcı topluluğuna sahiptir. Sorunlar için hızlı çözümler ve sürekli güncellemeler sunulur.

#### **Linux'un Tarihçesi**

- **Başlangıç (1991):**
  - Linus Torvalds, Helsinki Üniversitesi'nde öğrenciyken kendi kişisel kullanımına yönelik bir işletim sistemi çekirdeği geliştirmeye başladı.
- **İlk Yayın ve Katkılar:**
  - Torvalds, projesini İnternet üzerinden paylaştı ve diğer programcıların katkılarına açtı. Bu, Linux'un hızlı bir şekilde gelişmesini sağladı.
- **GNU Projesi ile Entegrasyon:**
  - Richard Stallman tarafından başlatılan GNU Projesi'nin araçları ve yardımcı programları ile birleştirilen Linux çekirdeği, tam bir işletim sistemi haline geldi.
- **Gelişim ve Yaygınlaşma:**
  - 1990'ların sonları ve 2000'li yıllarda, birçok şirket ve kuruluş Linux'u benimsemeye başladı. Sunucu pazarında önemli bir pay elde etti.

#### **Linux Dağıtımları**

Linux çekirdeği üzerine inşa edilmiş, farklı ihtiyaç ve tercihlere yönelik birçok dağıtım (distro) bulunmaktadır:

- **Ubuntu:**
  - Kullanıcı dostu arayüzü ve geniş paket deposu ile özellikle yeni başlayanlar için popüler bir seçenektir.
- **Fedora:**
  - Güncel yazılım ve teknolojileri deneyimlemek isteyen kullanıcılar için idealdir. Red Hat tarafından desteklenir.
- **Debian:**
  - Kararlılığı ve güvenilirliği ile bilinir. Birçok diğer dağıtımın temelini oluşturur (örneğin, Ubuntu).
- **CentOS / Red Hat Enterprise Linux (RHEL):**
  - Kurumsal düzeyde destek ve uzun vadeli güncellemeler sunar. Sunucular ve iş istasyonları için uygundur.
- **Arch Linux:**
  - Kullanıcılara sistemi en ince ayrıntısına kadar özelleştirme imkanı sunar. Rolling release modelini takip eder.
- **openSUSE:**
  - Hem yeni başlayanlar hem de deneyimli kullanıcılar için tasarlanmıştır. Güçlü yönetim araçları sunar.

#### **Linux'un Kullanım Alanları**

- **Sunucular ve Veri Merkezleri:**
  - Web sunucuları, veri tabanları ve bulut hizmetleri genellikle Linux tabanlıdır.
- **Masaüstü Bilgisayarlar:**
  - Kullanıcılar, Windows veya macOS'a alternatif olarak Linux dağıtımlarını tercih edebilirler.
- **Gömülü Sistemler ve IoT Cihazları:**
  - Router'lar, akıllı televizyonlar, otomotiv sistemleri ve diğer gömülü cihazlarda kullanılır.
- **Mobil Cihazlar:**
  - Android işletim sistemi, Linux çekirdeği üzerine inşa edilmiştir.
- **Süper Bilgisayarlar:**
  - Dünyanın en hızlı bilgisayarlarının büyük bir çoğunluğu Linux kullanır.
- **Eğitim ve Araştırma:**
  - Üniversiteler ve araştırma kuruluşları, esnekliği ve maliyet etkinliği nedeniyle Linux'u tercih eder.

#### **Linux ve Açık Kaynak Felsefesi**

- **Özgür Yazılım Hareketi:**
  - Linux, özgür yazılım hareketinin önemli bir parçasıdır. Kullanıcıların yazılımı çalıştırma, inceleme, değiştirme ve dağıtma özgürlüğünü savunur.
- **Topluluk Katkısı:**
  - Binlerce geliştirici, projeye kod, dökümantasyon ve destek sağlayarak katkıda bulunur.
- **Şeffaflık ve Güvenlik:**
  - Kaynak kodunun açık olması, güvenlik açıklarının hızlı bir şekilde tespit edilip düzeltilmesini sağlar.

#### **Linux Öğrenmeye ve Kullanımına Başlamak**

- **Linux Kurulumu:**
  - **Canlı USB/DVD:** İşletim sistemini kurmadan önce denemek için kullanılabilir.
  - **Sanal Makineler:** VirtualBox veya VMware gibi araçlarla Linux'u mevcut işletim sisteminiz üzerinde çalıştırabilirsiniz.
  - **Çift Önyükleme (Dual Boot):** Bilgisayarınıza hem mevcut işletim sisteminizi hem de Linux'u kurabilirsiniz.
- **Temel Komutlar ve Terminal Kullanımı:**
  - Linux'un gücü terminaldedir. Temel komutları öğrenmek, sistem üzerinde daha fazla kontrol sağlar.
- **Masaüstü Ortamları:**
  - GNOME, KDE Plasma, XFCE, LXDE gibi farklı masaüstü ortamlarını deneyebilirsiniz.
- **Paket Yönetimi:**
  - Yazılımları kurmak, güncellemek ve kaldırmak için kullanılan araçlardır (örneğin, `apt`, `yum`, `dnf`, `pacman`).
- **Kaynaklar ve Topluluklar:**
  - **Forumlar ve Siteler:** Stack Overflow, Linux Mint Forums, Arch Linux Forums.
  - **Eğitim Platformları:** Linux Academy, Coursera, edX.
  - **Belgelendirme:** Her dağıtımın kendi resmi belgeleri ve wiki sayfaları vardır.

#### **Neden Linux Tercih Edilmeli?**

- **Maliyet:**
  - Çoğu Linux dağıtımı ücretsizdir. Lisans maliyeti olmadan kullanılabilir.
- **Güncelleme ve Destek:**
  - Sürekli güncellemeler ve uzun vadeli destek seçenekleri mevcuttur.
- **Kişiselleştirme:**
  - İhtiyaçlarınıza ve zevklerinize göre sistemi özelleştirebilirsiniz.
- **Öğrenme ve Kariyer Fırsatları:**
  - Linux bilgisi, bilişim sektöründe önemli bir beceridir. Sistem yönetimi, siber güvenlik, yazılım geliştirme gibi alanlarda avantaj sağlar.

---

### **Terminal ve Komut Satırı Arayüzü (CLI)**

**Terminal**, işletim sisteminizle metin tabanlı komutlar aracılığıyla etkileşim kurmanızı sağlayan bir uygulamadır. **Komut Satırı Arayüzü (CLI)** ise terminal üzerinden girilen komutların yorumlanması ve çalıştırılması sürecini ifade eder. CLI, grafiksel kullanıcı arayüzüne (GUI) alternatif olarak, sistemle daha doğrudan ve hızlı bir şekilde iletişim kurmanızı sağlar.

#### **Terminal ve CLI'nin Önemi**

- **Verimlilik ve Hız:**
  - Komut satırı, belirli görevleri grafiksel arayüze göre daha hızlı ve verimli bir şekilde gerçekleştirmenize olanak tanır.
- **Güç ve Esneklik:**
  - CLI, sistem üzerinde daha fazla kontrol sağlar ve karmaşık işlemleri otomatikleştirmek için script yazmanıza imkan tanır.
- **Kaynak Kullanımı:**
  - Terminal uygulamaları genellikle daha az sistem kaynağı tüketir, bu da özellikle düşük donanımlı sistemlerde avantajlıdır.
- **Uzak Erişim ve Yönetim:**
  - SSH gibi protokoller aracılığıyla uzak sunuculara bağlanarak yönetim işlemlerini gerçekleştirebilirsiniz.

#### **Terminal Uygulamaları**

- **GNOME Terminal:**
  - GNOME masaüstü ortamının varsayılan terminal uygulamasıdır.
- **Konsole:**
  - KDE masaüstü ortamı için varsayılan terminal uygulamasıdır.
- **xterm, rxvt, Terminator, Tilix:**
  - Farklı özellikler sunan diğer terminal emülatörleridir.

#### **Temel Komut Satırı Yapısı**

Bir komut satırı genellikle aşağıdaki yapıyı izler:

```bash
komut [seçenekler] [argümanlar]
```

## **2. Temel Komutlar**

### **Navigasyon Komutları**

- `pwd` - Geçerli dizini gösterir.
  ```bash
  pwd
   ```
- `ls` - Dizindeki dosya ve klasörleri listeler.
  ```bash
  ls -al
  ```
- `cd` - Dizinler arasında geçiş yapar.
  ```bash
  cd /home/kullanici
  ```
### **Dosya ve Klasör İşlemleri**

- `mkdir` - Yeni bir klasör oluşturur.
  ```bash
  mkdir yeni_klasor
  ```
- `touch` - Yeni bir dosya oluşturur veya mevcut dosyanın erişim zamanını günceller.
  ```bash
  touch yeni_dosya.txt
   ```
- `cp` - Dosya veya klasör kopyalar.
  ```bash
  cp kaynak_dosya.txt hedef_dosya.txt
  ```
- `mv` - Dosya veya klasör taşır veya yeniden adlandırır.
  ```bash
  mv eski_ad.txt yeni_ad.txt
    ```
- `rm` - Dosya veya klasör siler.
  ```bash
  rm dosya.txt
  rm -r klasor
  rmdir klasör
   ```
### **Dosya Görüntüleme ve Düzenleme**

- `cat` - Dosya içeriğini görüntüler.
  ```bash
  cat dosya.txt
  ```
- `nano, vim, gedit` - Metin düzenleyicileri ile dosya düzenleme.
  ```bash
  nano dosya.txt  
   ```
### **Sistem Bilgileri ve Yönetimi**

- `top ve htop` - Sistem süreçlerini ve kaynak kullanımını izler.
  ```bash
  top
  htop
  ```
- `ps` - Çalışan süreçleri listeler.
  ```bash
  ps
  ```
- `uname` - Sistem bilgilerini gösterir.
  ```bash
  uname -a
   ```
- `df` - Disk kullanımını gösterir.
  ```bash
  df -h
  ```
### **Dosya İzinleri ve Sahipliği**

- `chmod ` - Dosya izinlerini değiştirir.
  ```bash
  chmod 755 script.sh
  ```
- `chown` - Dosya sahibini değiştirir.
  ```bash
  chown kullanici:kullanici_grubu dosya.txt
  ```
- `chgrp` - Dosya grubunu değiştirir.
  ```bash
  chgrp grup dosya.txt
  ```
### **Arama ve Filtreleme Komutları**

- `grep ` - Metin içinde arama yapar.
  ```bash
  grep "aranan_kelime" dosya.txt
  ```
- `find` - Dosya ve dizin arar.
  ```bash
  find /home/kullanici -name "dosya.txt"
  ```
### **Dosya Sıkıştırma ve Arşivleme**

- `tar` - Dosyaları arşivler ve sıkıştırır.
  ```bash
  tar -czvf arsiv.tar.gz klasor/
  ```
- `zip ve unzip` - ZIP arşivlerini oluşturur ve açar.
  ```bash
  zip -r arsiv.zip klasor/
  unzip arsiv.zip
  ```
### **Kullanıcı Yönetimi**
  
- `adduser ve useradd` - Yeni kullanıcı ekler.
  ```bash
  sudo adduser yeni_kullanici
  ```
- `passwd` - Kullanıcı şifresini değiştirir.
  ```bash
  sudo passwd kullanici_adi
  ```  
- `usermod` - Kullanıcı bilgilerini değiştirir.
  ```bash
  sudo usermod -aG grup kullanici_adi
  ```
## **3. Bash ve Shell İpuçları**

Bash, Unix ve Linux sistemlerinde en yaygın kullanılan komut satırı kabuğudur. Shell script'leri yazarak görevleri otomatikleştirebilir, sistem yönetimi yapabilir ve verimliliğinizi artırabilirsiniz. Bu bölümde, Bash ve shell programlama ile ilgili ipuçları, komut açıklamaları ve örnekler bulacaksınız.

### **Değişkenler ve Çevresel Değişkenler**

**Değişkenler**, script'ler içinde veri saklamak için kullanılır.

- **Değişken Tanımlama:**

  ```bash
  # Değişken atama (eşittir işaretinin etrafında boşluk olmamalı)
  degisken_adi="deger"

  # Örnek:
  mesaj="Merhaba Dünya"
  echo $mesaj  # Çıktı: Merhaba Dünya
  ```
- **Çevresel Değişkenler:** `export` komutu, bir değişkeni tüm alt süreçlerde kullanılabilir hale getirir.

  ```bash
  # Çevresel değişken atama
  export YENI_DEGISKEN="deger"
  
  # Mevcut çevresel değişkenleri listeleme
  printenv
  ```

### **Kullanıcı Girdisi ve Okuma**

- **`read`Komutu ile Girdi Alma:**`read` komutu, kullanıcıdan girdi alır.`-p` seçeneği ile bir prompt mesajı gösterebilirsiniz.

  ```bash
  # Kullanıcıdan isim alma
  read -p "İsminiz nedir? " isim
  echo "Merhaba, $isim!"
  ```

### **Koşullu İfadeler**

- **if...then...fi Yapısı:** Koşul doğruysa then bloğundaki komutlar çalışır.

  ```bash
  if [ koşul ]; then
      # Koşul doğruysa çalışacak komutlar
  fi
  ```
- **Sayı Karşılaştırma Operatörleri:** `export` komutu, bir değişkeni tüm alt süreçlerde kullanılabilir hale getirir.

| Operatör        | Anlamı           |
|:----------------|:-----------------|
| -eq             | Eşit             |
| -ne             | Eşit değil       |
| -gt             | Büyüktür         |
| -ge             | Büyük veya eşit  |
| -lt             | Küçüktür         |
| -le             | Küçük veya eşit  |


```bash
  sayi=10
  
  if [ $sayi -gt 5 ]; then
      echo "Sayı 5'ten büyüktür."
  else
      echo "Sayı 5'e eşit veya küçüktür."
  fi  
```
Açıklama: sayi değişkeni 5’ten büyükse, ilk mesajı yazdırır; değilse, ikinci mesajı.

### **Döngüler**

- **for Döngüsü:**

```bash
  for i in {1..5}; do
    echo "Sayı: $i"
  done 
 ```
Açıklama: i değişkeni 1’den 5’e kadar değerler alır ve her seferinde echo komutu çalışır.

- **while Döngüsü:** `export` komutu, bir değişkeni tüm alt süreçlerde kullanılabilir hale getirir.

```bash
    count=1
  while [ $count -le 5 ]; do
      echo "Count: $count"
      count=$((count + 1))
  done
```
Açıklama: count 5’e eşit veya küçük olduğu sürece döngü devam eder.

### **Fonksiyonlar**

- **Fonksiyon Tanımlama ve Kullanma:**

```bash
    f# Fonksiyon tanımlama
  selamla() {
      echo "Merhaba, $1!"
  }
  
  # Fonksiyonu çağırma
  selamla "Ahmet"  # Çıktı: Merhaba, Ahmet! 
 ```
Açıklama: selamla fonksiyonu, ilk parametre olarak verilen ismi kullanarak bir mesaj yazdırır.

### **Diziler**

- **Dizi Tanımlama:**

```bash
    meyveler=("Elma" "Armut" "Muz")
 ```
Açıklama: meyveler adlı bir dizi oluşturur ve içine üç meyve ekler.


- **Dizi Elemanlarına Erişim:**

```bash
    echo ${meyveler[0]}  # Çıktı: Elma
 ```
Açıklama: Diziler 0’dan indekslenir. [0] ilk elemanı verir.

### **Dosya Testleri**

- **Dosya Varlık Kontrolü:**

```bash
    dosya="dosya.txt"

if [ -e $dosya ]; then
    echo "Dosya mevcut."
else
    echo "Dosya bulunamadı."
fi
 ```
Açıklama: -e operatörü, dosya veya dizinin var olup olmadığını kontrol eder.


| Operatör | Anlamı                            |
|:---------|:----------------------------------|
| -e       | Dosya veya dizin mevcut mu?       |
| -f       | Normal bir dosya mı?              |
| -d       | Dizin mi?                         |
| -r       | Okunabilir mi?                    |
| -w       | Yazılabilir mi?                   |
| -x       | Çalıştırılabilir mi?              |


