# Futbolcu Tahmin Oyunu

Bu proje, Avrupa'nın 5 büyük liginden futbolcularla oynanan Wordle tarzı bir tahmin oyunudur.

## Özellikler

- Lig seçme ekranı ve logolar (isim olmadan!)
- Doğru futbolcu ismini harf harf tahmin etme
- Her yanlış tahminle sırayla: Mevki, Yaş, Takım ve Uyruk ipuçları açılır
- Tüm oyuncu verileri JSON dosyasından yüklenir
- Arayüzde Python'un Tkinter ve Pillow kütüphaneleri kullanılır

## Kurulum

1. Gerekli kütüphaneleri yükleyin:
   ```bash
   pip install -r requirements.txt
   ```

2. Klasör yapınızı şu şekilde düzenleyin:

   ```
   pythonodevi.py
   oyuncu_olustur.py
   secili_takim_oyuncular.json
   requirements.txt
   README.md
   logos/
       bundesliga.png
       la_liga.png
       ligue1.png
       premier_lig.png
       serie_a.png
   screenshots/
       ana_menu.png
       oyun_ekrani.png
       dogru_tahmin.png
   ```

3. Eğer güncel futbolcu verisi çekmek isterseniz:
   ```bash
   python oyuncu_olustur.py
   ```
   > Not: API limiti dolarsa, bir süre sonra tekrar çalıştırabilirsiniz.

4. Oyunu başlatmak için:
   ```bash
   python pythonodevi.py
   ```

## Oyun Nasıl Çalışır?

- İlk ekranda istediğiniz ligi simgesine tıklayarak seçin.
- Rastgele bir futbolcunun ismini tahmin etmeye başlayın.
- Her harfi klavyeden girin, doğru harfler yeşil kutuda kalır.
- 5 hakkınız var. Her yanlış hakkınızda ek ipucu açılır.
- İsim tamamen doğruysa yeni oyuncu gelir.
- Hakkınız bittiğinde doğru cevap ekranda gösterilir ve ana menüye dönebilirsiniz.

## Kullanılan Python Kütüphaneleri

- `requests` - (oyuncu_olustur.py ile API'den veri çekmek için)
- `json` - JSON veri işlemleri
- `tkinter` - Arayüz (Python ile birlikte gelir)
- `PIL` (Pillow) - Resim dosyalarını arayüzde göstermek için
- `os`, `sys`, `random` - Standart kütüphaneler

## Ekran Görüntüleri

Ana Menü:  
![Ana Menü](screenshots/ana_menu.png)

Oyun Ekranı - Tahmin ve İpucu:  
![Oyun Ekranı](screenshots/oyun_ekrani.png)

Doğru Tahmin Sonrası:  
![Doğru Tahmin](screenshots/dogru_tahmin.png)

## Katkı ve Lisans

Bu proje ödev/kişisel eğitim amaçlı hazırlanmıştır.  
Dilerseniz kendi veri setleriniz veya logolarınızla geliştirebilirsiniz.

---

İyi oyunlar!
