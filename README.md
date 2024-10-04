# **Linux Komutları Eğitim Dokümanı**

## **1. Giriş**

### **Linux Nedir?**

- Linux işletim sisteminin tanımı ve genel özellikleri.
- Linux dağıtımları (Ubuntu, Fedora, CentOS, vs.)

### **Terminal ve Komut Satırı Arayüzü (CLI)**

- Terminalin ne olduğu ve nasıl kullanılacağı.
- GUI ile CLI arasındaki farklar.

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


