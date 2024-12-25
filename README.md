### ATM Uygulaması README

#### Proje Hakkında
Bu proje, bir **ATM simülasyonu** geliştirmek amacıyla Python kullanılarak yazılmıştır. Kullanıcılar, mevcut bakiyelerini görüntüleyebilir, para yatırabilir, para çekebilir veya işlemleri sonlandırarak sistemden çıkış yapabilir.

#### Çalıştırma Talimatları
1. Python'un bilgisayarınıza kurulu olduğundan emin olun (3.6 veya üzeri sürüm önerilir).
2. Proje dosyasını indirin ve bir Python IDE veya metin düzenleyicisi kullanarak açın.
3. Aşağıdaki komutu terminalde çalıştırarak uygulamayı başlatabilirsiniz:
   ```bash
   python <dosya_adı>.py
   ```
4. Program çalışmaya başladığında, kullanıcıdan menü seçeneklerinden birini seçmesi istenecektir.

#### Kullanıcı Menü Seçenekleri
Program çalıştırıldığında aşağıdaki menü seçenekleri görüntülenecektir:

1. **Bakiye Görüntüle**: Mevcut hesap bakiyenizi gösterir.
2. **Para Yatır**: Hesabınıza para yatırmanızı sağlar.
3. **Para Çek**: Hesabınızdan belirttiğiniz miktarda para çekmenizi sağlar.
4. **Çıkış**: Programdan çıkış yapar.

#### Fonksiyonlar
1. **`__init__(self, balance=1000)`**  
   - ATM sınıfının başlangıç bakiyesini (`balance`) belirler. Varsayılan bakiye 1000 TL'dir.

2. **`display_balance(self)`**  
   - Mevcut bakiyeyi ekrana yazdırır.

3. **`deposit(self, amount)`**  
   - Belirtilen miktarı hesaba ekler. Geçersiz (negatif veya sıfır) miktarlarda uyarı mesajı verir.

4. **`withdraw(self, amount)`**  
   - Belirtilen miktarı hesaptan çeker. Eğer çekim yapılmak istenen miktar, mevcut bakiyeyi aşarsa uyarı verir. Negatif veya sıfır miktarlarda da işlem gerçekleştirilmez.

5. **`atm_menu()`**  
   - Kullanıcı etkileşim menüsünü oluşturur ve kullanıcı girişine göre ilgili işlemleri gerçekleştirir.

#### Örnek Kullanım
```plaintext
ATM İşlemleri:
1. Bakiye Görüntüle
2. Para Yatir
3. Para Çek
4. Çikiş
Seçiminiz (1/2/3/4): 1
Mevcut Bakiye: 1000 TL
```

#### Önemli Notlar
- Para yatırma ve çekme işlemleri sırasında negatif veya sıfır değerler kabul edilmez.
- Çekim yapmak için bakiyenizin yeterli olması gerekir.
- Kullanıcı **4** seçeneğini seçtiğinde programdan çıkış yapılır.

#### Gereksinimler
- Python 3.6 veya üzeri

#### Katkıda Bulunma
Bu projeyi geliştirmek veya katkıda bulunmak istiyorsanız, dosyayı fork'layarak kendi değişikliklerinizi yapabilir ve geri bildirimde bulunabilirsiniz.
