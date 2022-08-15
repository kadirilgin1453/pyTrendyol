# ![pyTrendyol](https://www.trendyol.com/frontend/web/assets/images/favicon.ico) pyTrendyol

![Repo Boyutu](https://img.shields.io/github/repo-size/keyiflerolsun/pyTrendyol)
![Görüntülenme](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https://github.com/keyiflerolsun/pyTrendyol&title=Görüntülenme)
<a href="https://KekikAkademi.org/Kahve" target="_blank"><img src="https://img.shields.io/badge/☕️-Kahve Ismarla-ffdd00" title="☕️ Kahve Ismarla" style="padding-left:5px;"></a>
[![Gitpod](https://img.shields.io/badge/Gitpod-Çalıştır-blue?logo=gitpod)](https://gitpod.io/#https://github.com/keyiflerolsun/pyTrendyol)
[![Repl.it](https://img.shields.io/badge/Replit-Çalıştır-green?logo=replit)](https://repl.it/github/keyiflerolsun/pyTrendyol)

![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyTrendyol)
![PyPI - Status](https://img.shields.io/pypi/status/pyTrendyol)
![PyPI](https://img.shields.io/pypi/v/pyTrendyol)
![PyPI - Downloads](https://img.shields.io/pypi/dm/pyTrendyol)
![PyPI - Wheel](https://img.shields.io/pypi/wheel/pyTrendyol)
![PyPI - License](https://img.shields.io/pypi/l/pyTrendyol)

*Trendyol'dan veri almayı kolaylaştırmak için tasarlanan kütüphane.*

[![ForTheBadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)
[![ForTheBadge built-with-love](http://ForTheBadge.com/images/badges/built-with-love.svg)](https://GitHub.com/keyiflerolsun/)

## 🚀 Kurulum

```bash
# Yüklemek
pip install pyTrendyol

# Güncellemek
pip install -U pyTrendyol
```

## 📝 Kullanım

```python
from pyTrendyol import Kategori, Urun

trend_kategori = Kategori()
trend_urun     = Urun()

telefon_aksesuarlari = trend_kategori.urunleri_ver(kategori_adi='telefon aksesuarları', sayfa_tara=3)
print(telefon_aksesuarlari)
    # » [{'link': 'https://www.trendyol.com/glassy/iphone-6s-plus-tam-kaplayan-kirilmaz-cam-9d-siyah-p-63170604', 'marka': 'GLASSY', 'yildiz': 4, 'baslik': 'Iphone 6s Plus Tam Kaplayan Kırılmaz Cam 9d Siyah', 'indirim': None, 'indirimsiz': None, 'fiyat': '8,96 TL'}, {'link': 'https://www.trendyol.com/teknoceri/xiaomi-redmi-note-9-ici-kadife-lansman-silikon-kilif-p-62180786', 'marka': 'Teknoçeri', 'yildiz': 4, 'baslik': 'Xiaomi Redmi Note 9 Içi Kadife Lansman Silikon Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '14,53 TL'}, {'link': 'https://www.trendyol.com/mopal/asker-yesili-pro-silikon-airpods-kilif-p-43869432', 'marka': 'Mopal', 'yildiz': 3, 'baslik': 'Asker Yeşili Pro Silikon Airpods Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '15,29 TL'}, {'link': 'https://www.trendyol.com/esnafstore/iphone-12-mini-kirilmaz-cam-iphone-12-mini-ekran-koruyucu-seffaf-tam-kaplama-p-77703589', 'marka': 'ESNAFSTORE', 'yildiz': 4, 'baslik': 'Iphone 12 Mini Kırılmaz Cam, Iphone 12 Mini Ekran Koruyucu Şeffaf Tam Kaplama', 'indirim': None, 'indirimsiz': None, 'fiyat': '9,97 TL'}, {'link': 'https://www.trendyol.com/teknoceri/iphone-11-6-1-3d-kamera-korumali-ici-kadife-lansman-silikon-kilif-p-86732434', 'marka': 'Teknoçeri', 'yildiz': 4, 'baslik': 'Iphone 11 6.1" 3d Kamera Korumalı Içi Kadife Lansman Silikon Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '12,34 TL'}, {'link': 'https://www.trendyol.com/ucuzmi/xiaomi-mi-band-5-5d-tam-kaplayan-nano-ekran-koruyucu-filmi-p-49331222', 'marka': 'ucuzmi', 'yildiz': 2, 'baslik': 'Xiaomi Mi Band 5 5d Tam Kaplayan Nano Ekran Koruyucu Filmi', 'indirim': None, 'indirimsiz': None, 'fiyat': '55,00 TL24,70 TL'}, {'link': 'https://www.trendyol.com/gsmclub/xiaomi-redmi-note-8-gorunmez-hayalet-full-kaplayan-ekran-koruyucu-cam-p-57554392', 'marka': 'Gsmclub', 'yildiz': 3, 'baslik': 'Xiaomi Redmi Note 8 Görünmez Hayalet Full Kaplayan Ekran Koruyucu Cam', 'indirim': None, 'indirimsiz': None, 'fiyat': '59,00 TL19,99 TL'}, {'link': 'https://www.trendyol.com/ekolaks/xiaomi-poco-x3-ekran-koruyucu-9d-mat-parmak-izi-birakmayan-tam-kaplayan-kirilmaz-cam-p-93690300', 'marka': 'Ekolaks', 'yildiz': 3, 'baslik': 'Xiaomi Poco X3 Ekran Koruyucu 9d Mat Parmak Izi Bırakmayan Tam Kaplayan Kırılmaz Cam', 'indirim': None, 'indirimsiz': None, 'fiyat': '40,00 TL18,90 TL'}, {'link': 'https://www.trendyol.com/ttec/minicable-iphone-uyumlu-icin-sarj-senkronizasyon-kablosu-p-2900579', 'marka': 'Ttec', 'yildiz': 4, 'baslik': 'MiniCable™ iPhone Uyumlu için Şarj/Senkronizasyon Kablosu', 'indirim': 'Sepette %2 İndirim', 'indirimsiz': '19,99 TL', 'fiyat': '19,59 TL'}, {'link': 'https://www.trendyol.com/telefon-aksesuarlari/iphone-xs-max-gizli-hayalet-5d-tam-kaplayan-kirilmaz-cam-siyah-p-45321400', 'marka': 'Telefon Aksesuarları', 'yildiz': 4, 'baslik': 'Iphone Xs Max Gizli Hayalet 5d Tam Kaplayan Kırılmaz Cam ( Siyah )', 'indirim': None, 'indirimsiz': None, 'fiyat': '49,99 TL19,99 TL'}, {'link': 'https://www.trendyol.com/hypercep/dayanikli-figurlu-sevimli-sarj-kablo-duzenleyici-sarma-aparati-kablo-koruyucu-seti-takim-p-51018248', 'marka': 'HyperCep', 'yildiz': 4, 'baslik': 'Dayanıklı Figürlü Sevimli Şarj Kablo Düzenleyici Sarma Aparatı + Kablo Koruyucu Seti Takım', 'indirim': 'Sepette %2 İndirim', 'indirimsiz': '15,40 TL', 'fiyat': '15,09 TL'}, {'link': 'https://www.trendyol.com/okmore/iphone-7-8-plus-x-11-uyumlu-soket-cogaltici-kulaklik-adaptoru-p-38582242', 'marka': 'OKMORE', 'yildiz': 3, 'baslik': 'Iphone 7 8 Plus X 11 Uyumlu Soket Çoğaltıcı Kulaklık Adaptörü', 'indirim': 'Sepette %2 İndirim', 'indirimsiz': '12 TL', 'fiyat': '11,76 TL'}, {'link': 'https://www.trendyol.com/teknosepetim/iphone-7-nano-mat-seramikceramic-6d-flexible-ekran-koruyucu-kirilmaz-cam-tam-kaplayan-p-60123581', 'marka': 'teknosepetim', 'yildiz': 4, 'baslik': 'Iphone 7 Nano Mat Seramik(ceramic) 6d Flexible Ekran Koruyucu Kırılmaz Cam Tam Kaplayan', 'indirim': None, 'indirimsiz': None, 'fiyat': '40,00 TL13,79 TL'}, {'link': 'https://www.trendyol.com/ttec/powerup-duo-20-000-mah-tasinabilir-sarj-cihazi-p-36825031', 'marka': 'Ttec', 'yildiz': 4, 'baslik': 'Powerup Duo 20.000 Mah Taşınabilir Şarj Cihazı', 'indirim': 'Sepette %2 İndirim', 'indirimsiz': '135,90 TL', 'fiyat': '133,18 TL'}, {'link': 'https://www.trendyol.com/auris/2600-mah-power-bank-p-38156131', 'marka': 'Auris', 'yildiz': 3, 'baslik': '2600 Mah Power Bank', 'indirim': None, 'indirimsiz': None, 'fiyat': '15 TL'}, {'link': 'https://www.trendyol.com/bilisim-aksesuar/xiaomi-poco-x3-nfc-lansman-silikon-kilif-p-91139390', 'marka': 'Bilişim Aksesuar', 'yildiz': 4, 'baslik': 'Xiaomi Poco X3 Nfc Lansman Silikon Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '16,62 TL'}, {'link': 'https://www.trendyol.com/inteknoloji/iphone-11-11-pro-11-pro-max-icin-uyumlu-sarj-aleti-seti-18w-usbc-adaptor-usbc-lightning-kablo-p-45595353', 'marka': 'inteknoloji', 'yildiz': 3, 'baslik': 'Iphone 11/11 Pro/11 Pro Max Için Uyumlu Şarj Aleti Seti 18w Usbc Adaptör Usbc Lightning Kablo', 'indirim': None, 'indirimsiz': None, 'fiyat': '89,00 TL71 TL'}, {'link': 'https://www.trendyol.com/teknoceri/xiaomi-redmi-note-9s-note-9-pro-ici-kadife-lansman-silikon-kilif-p-62202409', 'marka': 'Teknoçeri', 'yildiz': 4, 'baslik': 'Xiaomi Redmi Note 9s / Note 9 Pro Içi Kadife Lansman Silikon Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '12,50 TL'}, {'link': 'https://www.trendyol.com/teknoparkta/xiaomi-redmi-note-9-pro-mat-tam-full-kaplayan-seramik-nano-cam-ekran-koruyucu-p-78544308', 'marka': 'TEKNOPARKTA', 'yildiz': 4, 'baslik': 'Xiaomi Redmi Note 9 Pro Mat Tam Full Kaplayan Seramik Nano Cam Ekran Koruyucu', 'indirim': None, 'indirimsiz': None, 'fiyat': '49,90 TL24,88 TL'}, {'link': 'https://www.trendyol.com/kvk-privacy/iphone-se-2020-logolu-lansman-kilif-alti-kapali-ic-kismi-kadife-p-96942228', 'marka': 'KVK PRİVACY', 'yildiz': 4, 'baslik': 'Iphone Se 2020 Logolu Lansman Kılıf Altı Kapalı Iç Kısmı Kadife', 'indirim': None, 'indirimsiz': None, 'fiyat': '69,00 TL27,55 TL'}, {'link': 'https://www.trendyol.com/teknoceri/iphone-11-6-1-kenarlari-renkli-kamera-korumali-transparan-kilif-p-79058928', 'marka': 'Teknoçeri', 'yildiz': 4, 'baslik': 'Iphone 11 6.1" Kenarları Renkli Kamera Korumalı Transparan Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '15,40 TL'}, {'link': 'https://www.trendyol.com/bizimgross/xiaomi-mi-10t-pro-arka-kamera-lens-koruma-ve-5d-ekran-koruyucu-kirilmaz-cam-p-72385661', 'marka': 'BizimGross', 'yildiz': 3, 'baslik': 'Xiaomi Mi 10t Pro Arka Kamera Lens Koruma Ve 5d Ekran Koruyucu Kırılmaz Cam', 'indirim': None, 'indirimsiz': None, 'fiyat': '119,00 TL68,90 TL'}, {'link': 'https://www.trendyol.com/aqua-aksesuar/xiaomi-poco-x3-pro-kilif-zirhli-kamera-surgulu-lux-kapak-p-114540515', 'marka': 'AQUA AKSESUAR', 'yildiz': 3, 'baslik': 'Xiaomi Poco X3 Pro Kılıf Zırhlı Kamera Sürgülü Lüx Kapak', 'indirim': None, 'indirimsiz': None, 'fiyat': '69,90 TL42,50 TL'}, {'link': 'https://www.trendyol.com/link-tech/iphone-kulaklik-ve-sarj-aparati-cogaltici-lightning-splitter-p-39963307', 'marka': 'Link Tech', 'yildiz': 3, 'baslik': 'Iphone Kulaklık Ve Şarj Aparatı& Çoğaltıcı - Lightning Splitter', 'indirim': None, 'indirimsiz': None, 'fiyat': '49,00 TL12,79 TL'}, {'link': 'https://www.trendyol.com/intouch/10-000-mah-prime-dijital-gostergeli-dahili-coklu-kablolu-powerbank-kirmizi-p-68363666', 'marka': 'İntouch', 'yildiz': 4, 'baslik': '10.000 Mah Prime Dijital Göstergeli Dahili Çoklu Kablolu Powerbank,kırmızı', 'indirim': 'Sepette %2 İndirim', 'indirimsiz': '88 TL', 'fiyat': '86,24 TL'}, {'link': 'https://www.trendyol.com/zore/ipad-8-nesil-uyumlu-10-2-tablet-temperli-ekran-koruyucu-p-52915790', 'marka': 'zore', 'yildiz': 3, 'baslik': 'Ipad 8.nesil Uyumlu 10.2 Tablet Temperli Ekran Koruyucu', 'indirim': None, 'indirimsiz': None, 'fiyat': '39,00 TL17 TL'}, {'link': 'https://www.trendyol.com/hypercep/spiral-kablo-koruyucu-silikon-set-sarj-kablosu-kulaklik-kablosu-koruyucu-p-104036727', 'marka': 'HyperCep', 'yildiz': 4, 'baslik': 'Spiral Kablo Koruyucu Silikon Set Şarj Kablosu Kulaklık Kablosu Koruyucu', 'indirim': 'Sepette %2 İndirim', 'indirimsiz': '6,99 TL', 'fiyat': '6,85 TL'}, {'link': 'https://www.trendyol.com/go-aksesuar/iphone-se-2020-logolu-antrasit-ici-kadife-aa-kalite-lansman-p-106921294', 'marka': 'Go Aksesuar', 'yildiz': 5, 'baslik': 'Iphone Se 2020 Logolu Antrasit Içi Kadife Aa Kalite Lansman', 'indirim': None, 'indirimsiz': None, 'fiyat': '23,99 TL19,99 TL'}, {'link': 'https://www.trendyol.com/santa-maria-jewels/siyah-renk-iphone-samsung-micro-usb-type-c-miknatisli-manyetik-sarj-kablosu-3-in-1-p-43827158', 'marka': 'Santa Maria Jewels', 'yildiz': 3, 'baslik': 'Siyah Renk Iphone Samsung Micro Usb Type-c Mıknatıslı Manyetik Şarj Kablosu 3 In 1', 'indirim': None, 'indirimsiz': None, 'fiyat': '23 TL'}, {'link': 'https://www.trendyol.com/my-murdum/iphone-uyumlu-sevimli-karakterler-sarj-kablo-koruyucusu-p-42172346', 'marka': 'MY MÜRDÜM', 'yildiz': 4, 'baslik': 'Iphone Uyumlu Sevimli Karakterler Şarj Kablo Koruyucusu', 'indirim': 'Sepette %2 İndirim', 'indirimsiz': '10,21 TL', 'fiyat': '10,01 TL'}, {'link': 'https://www.trendyol.com/mesear/iphone-11-cep-telefonu-uyumlu-kulaklik-cevirici-lightning-aux-donusturucu-otg-p-98239126', 'marka': 'Mesear', 'yildiz': 3, 'baslik': 'Iphone 11 Cep Telefonu Uyumlu Kulaklık Çevirici Lightning Aux Dönüştürücü Otg', 'indirim': None, 'indirimsiz': None, 'fiyat': '59,90 TL29,90 TL'}, {'link': 'https://www.trendyol.com/teknoceri/samsung-a51-seffaf-silikon-kilif-p-66763320', 'marka': 'Teknoçeri', 'yildiz': 4, 'baslik': 'Samsung A51 Şeffaf Silikon Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '10,35 TL'}, {'link': 'https://www.trendyol.com/suppo/iphone-11-kamera-korumali-logolu-lansman-kilif-kablo-koruyucu-p-87709352', 'marka': 'SUPPO', 'yildiz': 4, 'baslik': 'Iphone 11 Kamera Korumalı Logolu Lansman Kılıf+kablo Koruyucu', 'indirim': None, 'indirimsiz': None, 'fiyat': '28,40 TL'}, {'link': 'https://www.trendyol.com/suppo/iphone-11-kamera-korumali-model-logolu-lansman-kilif-kablo-koruyucu-p-87709021', 'marka': 'SUPPO', 'yildiz': 4, 'baslik': 'Iphone 11 Kamera Korumalı Model, Logolu Lansman Kılıf Kablo Koruyucu', 'indirim': None, 'indirimsiz': None, 'fiyat': '28,49 TL'}, {'link': 'https://www.trendyol.com/ttec/recharger-duo-iphone-lightning-dahili-kablolu-tasinabilir-sarj-aleti-powerbank-siyah-10-000mah-p-36888865', 'marka': 'Ttec', 'yildiz': 4, 'baslik': 'Recharger Duo+ Iphone Lightning Dahili Kablolu Taşınabilir Şarj Aleti / Powerbank Siyah 10.000mah', 'indirim': 'Sepette %2 İndirim', 'indirimsiz': '84,50 TL', 'fiyat': '82,81 TL'}, {'link': 'https://www.trendyol.com/teknoceri/redmi-note-8-ici-kadife-lansman-silikon-kilif-p-48547813', 'marka': 'Teknoçeri', 'yildiz': 4, 'baslik': 'Redmi Note 8 Içi Kadife Lansman Silikon Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '19,50 TL14,15 TL'}, {'link': 'https://www.trendyol.com/longline/3-uclu-ios-android-manyetik-miknatisli-usb-hizli-sarj-kablosu-p-85933694', 'marka': 'LONGLINE', 'yildiz': 4, 'baslik': '3 Uçlu Ios Android Manyetik Mıknatıslı Usb Hızlı Şarj Kablosu', 'indirim': None, 'indirimsiz': None, 'fiyat': '39,00 TL29 TL'}, {'link': 'https://www.trendyol.com/bilisim-aksesuar/apple-airpods-360-koruyucu-siyah-lux-deri-kilif-1-2-nesil-uyumlu-p-50512220', 'marka': 'Bilişim Aksesuar', 'yildiz': 4, 'baslik': 'Apple Airpods 360 Koruyucu Siyah Lüx Deri Kılıf 1 2 Nesil Uyumlu', 'indirim': None, 'indirimsiz': None, 'fiyat': '35,62 TL'}, {'link': 'https://www.trendyol.com/telehome/iphone-12-pro-max-uyumlu-hayalet-cam-tam-kaplayan-kirilmaz-cam-p-82976691', 'marka': 'Telehome', 'yildiz': 3, 'baslik': 'Iphone 12 Pro Max uyumlu Hayalet Cam Tam Kaplayan Kırılmaz Cam', 'indirim': None, 'indirimsiz': None, 'fiyat': '18,89 TL'}, {'link': 'https://www.trendyol.com/gomax/10000-mah-cift-usb-girisli-gercek-kapasite-beyaz-renk-powerbank-tasinabilir-sarj-aleti-p-79236958', 'marka': 'Gomax', 'yildiz': 4, 'baslik': '10000 Mah Çift Usb Girişli Gerçek Kapasite Beyaz Renk Powerbank Taşınabilir Şarj Aleti', 'indirim': None, 'indirimsiz': None, 'fiyat': '49,90 TL'}, {'link': 'https://www.trendyol.com/mislina/iphone-11-tam-kapatan-cam-ekran-koruyucu-p-105123754', 'marka': 'Mislina', 'yildiz': 4, 'baslik': 'Iphone 11 Tam Kapatan Cam Ekran Koruyucu', 'indirim': None, 'indirimsiz': None, 'fiyat': '59,90 TL35,90 TL'}, {'link': 'https://www.trendyol.com/apple/iphone-orijinal-sarj-aleti-cihazi-usb-kablosu-orjinal-lightning-p-58064305', 'marka': 'Apple', 'yildiz': 3, 'baslik': 'Iphone Orijinal Şarj Aleti Cihazı + Usb Kablosu Orjinal Lightning', 'indirim': None, 'indirimsiz': None, 'fiyat': '149,00 TL67,99 TL'}, {'link': 'https://www.trendyol.com/benks/iphone-12-pro-max-uyumlu-integrated-kamera-lens-koruyucu-cam-p-94115774', 'marka': 'Benks', 'yildiz': 3, 'baslik': 'Iphone 12 Pro Max Uyumlu Integrated Kamera Lens Koruyucu Cam', 'indirim': None, 'indirimsiz': None, 'fiyat': '11,87 TL'}, {'link': 'https://www.trendyol.com/telefon-aksesuarlari/zengin-carsim-apple-iphone-xr-ultra-ince-seffaf-airbag-anti-sok-s-p-6530941', 'marka': 'Telefon Aksesuarları', 'yildiz': 4, 'baslik': 'Zengin Çarşım Apple Iphone Xr Ultra Ince Şeffaf Airbag Anti Şok S', 'indirim': None, 'indirimsiz': None, 'fiyat': '13,87 TL'}, {'link': 'https://www.trendyol.com/ekoodukkan/airpods-silikon-kilif-yumusak-mat-360-koruma-p-76358192', 'marka': 'Ekoodukkan', 'yildiz': 4, 'baslik': 'Airpods Silikon Kılıf Yumuşak Mat 360 Koruma', 'indirim': None, 'indirimsiz': None, 'fiyat': '13,77 TL'}, {'link': 'https://www.trendyol.com/dijimedia/samsung-galaxy-a51-ekrani-tam-kaplayan-5d-kirilmaz-cam-ekran-koruyucu-p-35473836', 'marka': 'dijimedia', 'yildiz': 3, 'baslik': 'Samsung Galaxy A51 Ekranı Tam Kaplayan 5d Kırılmaz Cam Ekran Koruyucu', 'indirim': None, 'indirimsiz': None, 'fiyat': '29,99 TL10,70 TL'}, {'link': 'https://www.trendyol.com/baseus/grain-serisi-minimal-tasarim-cift-usb-3-1a-arac-sarj-cihazi-siyah-p-4491044', 'marka': 'Baseus', 'yildiz': 4, 'baslik': 'Grain Serisi Minimal Tasarım Çift Usb 3.1a Araç Şarj Cihazı Siyah', 'indirim': 'Sepette %2 İndirim', 'indirimsiz': '58,75 TL', 'fiyat': '57,58 TL'}, {'link': 'https://www.trendyol.com/yilmazstore/iphone-uyumlu-beyaz-isiyla-daralan-makaron-1-m-100-cm-p-46417940', 'marka': 'YılmazStore', 'yildiz': 3, 'baslik': 'Iphone Uyumlu Beyaz Isıyla Daralan Makaron 1 m 100 cm', 'indirim': 'Sepette %2 İndirim', 'indirimsiz': '7,67 TL', 'fiyat': '7,52 TL'}, {'link': 'https://www.trendyol.com/kilifsiparis/apple-iphone-11-alt-cizgili-kilif-p-107267433', 'marka': 'Kılıfsiparis', 'yildiz': 0, 'baslik': 'Apple Iphone 11 Alt Çizgili Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '29,99 TL23,74 TL'}, {'link': 'https://www.trendyol.com/mooodcase/iphone-11-pro-max-premium-electrolize-silikonlu-beyaz-telefon-kilifi-p-96364300', 'marka': 'mooodcase', 'yildiz': 4, 'baslik': 'Iphone 11 Pro Max Premium Electrolize Silikonlu Beyaz Telefon Kılıfı', 'indirim': None, 'indirimsiz': None, 'fiyat': '44,90 TL29,90 TL'}, {'link': 'https://www.trendyol.com/telehome/iphone-11-lansman-kilif-ici-kadife-p-68460342', 'marka': 'Telehome', 'yildiz': 4, 'baslik': 'Iphone 11 Lansman Kılıf Içi Kadife', 'indirim': None, 'indirimsiz': None, 'fiyat': '13,20 TL'}, {'link': 'https://www.trendyol.com/motto/aux-usb-donusturucu-adaptor-aparat-disi-aux-cevirici-3-5-mm-p-104207520', 'marka': 'MOTTO', 'yildiz': 1, 'baslik': 'Aux Usb Dönüştürücü Adaptör Aparat Dişi Aux Çevirici 3.5 Mm', 'indirim': None, 'indirimsiz': None, 'fiyat': '42,18 TL'}, {'link': 'https://www.trendyol.com/polhammobile/ipad-iphone-sarj-cogaltici-donusturucu-iphone-11-pro-x-xs-xr-7-8-plus-sarj-muzik-ve-sarj-p-49997838', 'marka': 'Polhammobile', 'yildiz': 5, 'baslik': 'Ipad Iphone Şarj Çoğaltıcı Dönüştürücü Iphone 11 Pro X Xs Xr 7 8 Plus Şarj Müzik Ve Şarj', 'indirim': None, 'indirimsiz': None, 'fiyat': '79,00 TL29 TL'}, {'link': 'https://www.trendyol.com/teknoceri/iphone-11-yumusak-renkli-silikon-kilif-p-54582854', 'marka': 'Teknoçeri', 'yildiz': 4, 'baslik': 'Iphone 11 Yumuşak Renkli Silikon Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '11,40 TL'}, {'link': 'https://www.trendyol.com/heyo-cover/iphone-11-zincir-askili-aynali-kilif-p-69067769', 'marka': 'HEYO COVER', 'yildiz': 5, 'baslik': 'Iphone 11 Zincir Askılı Aynalı Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '60,00 TL49,45 TL'}, {'link': 'https://www.trendyol.com/sepetzy/apple-iphone-se-2020-tam-kaplayan-ekran-koruyucu-cam-siyah-p-56057310', 'marka': 'sepetzy', 'yildiz': 4, 'baslik': 'Apple Iphone Se 2020 Tam Kaplayan Ekran Koruyucu Cam Siyah', 'indirim': None, 'indirimsiz': None, 'fiyat': '29,90 TL'}, {'link': 'https://www.trendyol.com/kilifsiparis/apple-iphone-7-plus-8-plus-aynali-pembe-prizma-kilif-p-99133339', 'marka': 'Kılıfsiparis', 'yildiz': 5, 'baslik': 'Apple Iphone 7 Plus / 8 Plus Aynalı Pembe Prizma Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '28,40 TL'}, {'link': 'https://www.trendyol.com/suppo/iphone-7-plus-ve-8-plus-modellere-uyumlu-logolu-lansman-kilif-kablo-koruyucu-p-81807780', 'marka': 'SUPPO', 'yildiz': 4, 'baslik': 'Iphone 7 Plus Ve 8 Plus Modellere Uyumlu, Logolu Lansman Kılıf Kablo Koruyucu', 'indirim': None, 'indirimsiz': None, 'fiyat': '28,40 TL'}, {'link': 'https://www.trendyol.com/telehome/iphone-11-aynali-pembe-prizma-kilif-p-94054225', 'marka': 'Telehome', 'yildiz': 3, 'baslik': 'Iphone 11 Aynalı Pembe Prizma Kılıf', 'indirim': None, 'indirimsiz': None, 'fiyat': '27,54 TL'}, {'link': 'https://www.trendyol.com/bilisim-aksesuar/apple-airpods-koruyucu-kilif-kahve-canta-airpods-1-ve-2-p-70253111', 'marka': 'Bilişim Aksesuar', 'yildiz': 4, 'baslik': 'Apple Airpods Koruyucu Kılıf Kahve Çanta - Airpods 1 Ve 2', 'indirim': None, 'indirimsiz': None, 'fiyat': '37,99 TL'}, {'link': 'https://www.trendyol.com/syrox/c93-2-0a-iphone-lightning-sarj-ve-data-kablosu-siyah-p-38429934', 'marka': 'Syrox', 'yildiz': 4, 'baslik': 'C93 2.0a Iphone Lightning Şarj Ve Data Kablosu Siyah', 'indirim': None, 'indirimsiz': None, 'fiyat': '25,00 TL14,75 TL'}, {'link': 'https://www.trendyol.com/rangmobil/boyun-askili-kilif-ipi-orgulu-carpraz-kilif-satista-degildir-p-63171204', 'marka': 'rangmobil', 'yildiz': 4, 'baslik': 'Boyun Askılı Kılıf Ipi Örgülü Çarpraz [kılıf Satısta Değildir]', 'indirim': None, 'indirimsiz': None, 'fiyat': '79,00 TL29,90 TL'}, {'link': 'https://www.trendyol.com/gramaphone/mi-10t-pro-kilif-hd-desen-baskili-tam-korumali-silikon-arka-kapak-st-stok254-p-103849358', 'marka': 'Gramaphone', 'yildiz': 0, 'baslik': 'Mi 10t Pro Kılıf Hd Desen Baskılı Tam Korumalı Silikon Arka Kapak St - Stok254', 'indirim': None, 'indirimsiz': None, 'fiyat': '29,90 TL'}, {'link': 'https://www.trendyol.com/happycase/samsung-a50-a30s-a50s-lansman-silikon-kilif-sari-p-107396361', 'marka': 'HappyCase', 'yildiz': 4, 'baslik': 'Samsung A50 / A30s / A50s Lansman Silikon Kılıf Sarı', 'indirim': None, 'indirimsiz': None, 'fiyat': '14,72 TL'}, {'link': 'https://www.trendyol.com/dijimedia/apple-iphone-11-seffaf-sert-kilif-kamera-korumali-koseleri-kalin-coss-kapak-p-39194449', 'marka': 'dijimedia', 'yildiz': 3, 'baslik': 'Apple Iphone 11 Şeffaf Sert Kılıf Kamera Korumalı Köşeleri Kalın Coss Kapak', 'indirim': 'Sepette %1 İndirim', 'indirimsiz': '17,40 TL', 'fiyat': '17,23 TL'}, {'link': 'https://www.trendyol.com/shoptocase/iphone11-mavi-ejderha-telefon-kilifi-p-59302718', 'marka': 'shoptocase', 'yildiz': 4, 'baslik': 'Iphone11 Mavi Ejderha Telefon Kılıfı', 'indirim': None, 'indirimsiz': None, 'fiyat': '35,10 TL'}, {'link': 'https://www.trendyol.com/mkteknomarket/xiaomi-redmi-note-9-pro-9s-kirilmaz-ekran-koruyucu-temperli-cam-p-97090103', 'marka': 'Mkteknomarket', 'yildiz': 4, 'baslik': 'Xiaomi Redmi Note 9 Pro / 9s Kırılmaz Ekran Koruyucu Temperli Cam', 'indirim': None, 'indirimsiz': None, 'fiyat': '19,90 TL9 TL'}, {'link': 'https://www.trendyol.com/ecr/apple-watch-seri-6-se-5-4-44mm-ile-uyumlu-hd-seffaf-ekran-koruyucu-film-neo-flex-2-adet-p-104294176', 'marka': 'Ecr', 'yildiz': 2, 'baslik': 'Apple Watch Seri 6/se/5/4 (44mm) Ile Uyumlu Hd Şeffaf Ekran Koruyucu Film Neo Flex (2 Adet)', 'indirim': None, 'indirimsiz': None, 'fiyat': '59,90 TL26 TL'}, {'link': 'https://www.trendyol.com/fibaks/xiaomi-mi-8-lite-uyumlu-9h-temperli-cam-sert-seffaf-ekran-koruyucu-p-79674006', 'marka': 'Fibaks', 'yildiz': 3, 'baslik': 'Xiaomi Mi 8 Lite Uyumlu 9h Temperli Cam Sert Şeffaf Ekran Koruyucu', 'indirim': None, 'indirimsiz': None, 'fiyat': '30,00 TL9,90 TL'}, {'link': 'https://www.trendyol.com/bilisim-aksesuar/apple-airpods-pro-kilif-ince-slim-zar-silikon-p-56490781', 'marka': 'Bilişim Aksesuar', 'yildiz': 3, 'baslik': 'Apple Airpods Pro Kılıf Ince Slim Zar Silikon', 'indirim': None, 'indirimsiz': None, 'fiyat': '18,90 TL'}, {'link': 'https://www.trendyol.com/bca/xiaomi-redmi-9c-kirilmaz-ekran-koruyucu-temperli-cam-p-49313445', 'marka': 'BCA', 'yildiz': 4, 'baslik': 'Xiaomi Redmi 9c Kırılmaz Ekran Koruyucu Temperli Cam', 'indirim': None, 'indirimsiz': None, 'fiyat': '19,80 TL'}, {'link': 'https://www.trendyol.com/mtncover/iphone-x-icin-boyun-askili-seffaf-cok-sik-kilif-beyaz-ipli-p-42391091', 'marka': 'mtncover', 'yildiz': 4, 'baslik': 'Iphone X Için Boyun Askılı Şeffaf Çok Şık Kılıf Beyaz Ipli', 'indirim': None, 'indirimsiz': None, 'fiyat': '59,00 TL23 TL'}]

urun_detay = trend_urun.detay_ver('https://www.trendyol.com/glassy/iphone-6s-plus-tam-kaplayan-kirilmaz-cam-9d-siyah-p-63170604')
print(urun_detay)
    # » {'link': 'https://trendyol.com/glassy/iphone-6s-plus-tam-kaplayan-kirilmaz-cam-9d-siyah-p-63170604', 'marka': 'GLASSY', 'baslik': 'Iphone 6s Plus Tam Kaplayan Kırılmaz Cam 9d Siyah sbdcwey8rfh', 'resim': 'https://cdn.dsmcdn.com/mnresize/415/622/ty26/product/media/images/20201123/23/30612094/110618929/0/0_org_zoom.jpg', 'gercek': '29,99 TL', 'indirimli': '8,96 TL', 'kampanya': None, 'son_fiyat': None, 'yorumlar': [{'kullanici': 'Ceren Kalay', 'elit': False, 'tarih': '16 Haziran 2021', 'satici': 'Adaman', 'yildiz': 5, 'yorum': 'Çok güzel iPhone 6 Plus a da oluyor kaliteli fiyatı gayet uygun kırık gelmedi teşekkürler 😊'}, {'kullanici': 'Mehmet Akif KARABAYAZIT', 'elit': False, 'tarih': '9 Haziran 2021', 'satici': 'GO AKSESUAR', 'yildiz': 5, 'yorum': 'Fiyat olarak muhtemelen bundan uygununu bulamazsınız ve çok harika duruyor ürün.'}, {'kullanici': 'A** K**', 'elit': False, 'tarih': '3 Mayıs 2021', 'satici': 'Baysam', 'yildiz': 5, 'yorum': 'çok iyi ve sağlam ucuz'}, {'kullanici': 'emine yıldız', 'elit': True, 'tarih': '27 Mayıs 2021', 'satici': 'enuygun01', 'yildiz': 5, 'yorum': 'Ürün güzel kalın cam 6s plus a uygun. Ekranı tam kapatıyor sondaki kavisli küçük kısmı kapatmıyor düz bir ürün. Bu fiyata alınabilecek güzel bir ürün tavsiye ederim.kendiniz yapacaksanız hiçbir toz kalmayacak şekilde temizledikten sonra uygulayın çok kolay uygulaması'}, {'kullanici': 'Ozge Durmus', 'elit': True, 'tarih': '22 Haziran 2021', 'satici': 'JoyPlus', 'yildiz': 5, 'yorum': 'Mükemmel paketleme ve kaliteli ürün iyi ki almışım indirimde aldım fakat fiyatıda pahalı olsa satıcı son kuruşuna kadar hakediyor teşekkür ederim.'}, {'kullanici': 'B** B**', 'elit': False, 'tarih': '13 Mart 2021', 'satici': 'Baysam', 'yildiz': 5, 'yorum': 'Kötü yorumlara rağmen 2 adet sipariş ettim satıcıyla da güzel paketlemesi için iletişime geçtim. Ürün gayet güzel uygun fiyatlı kırılmadan elime ulaştı👍🏻'}, {'kullanici': 't** s**', 'elit': False, 'tarih': '23 Haziran 2021', 'satici': 'iphonoloji iletişim ', 'yildiz': 5, 'yorum': 'Kırılmaz Cam koruyucu alacaksanız . Bunu tercih etmelisiniz . Gördüklerimin en iyisi . 10 numara özel kabı bile diğerlerinde farklı . Teşekkür ederim'}, {'kullanici': '**** ****', 'elit': False, 'tarih': '19 Haziran 2021', 'satici': 'JoyPlus', 'yildiz': 4, 'yorum': 'Telefon camı tam olarak kaplamıyor. Ama bu fiyata gayet normal'}, {'kullanici': 'F** K** D**', 'elit': False, 'tarih': '26 Haziran 2021', 'satici': 'JoyPlus', 'yildiz': 5, 'yorum': 'Hem fiyatı iyi hem görünüşü'}, {'kullanici': 'Yunus Kolip', 'elit': False, 'tarih': '9 Haziran 2021', 'satici': 'Adaman', 'yildiz': 5, 'yorum': 'Ürün 10 numara 5 yıldız kesinlikle şu zamana kadar telefonuma taktığım en iyi ekran koruyucu 10/10 puan veriyorum'}, {'kullanici': 'Beyza Arıcan', 'elit': False, 'tarih': '18 Haziran 2021', 'satici': 'JoyPlus', 'yildiz': 5, 'yorum': 'Teşekkür ederim çok güzel paketlenmiş ve kalitesi baya güzel böyle işini yapan insanları çok seviyorum işin rast gitsin'}, {'kullanici': 'B** Y**', 'elit': False, 'tarih': '2 Haziran 2021', 'satici': 'JoyPlus', 'yildiz': 5, 'yorum': '6 adet aldım hepsi sorunsuz ulaştı ürünlerde bitane bile çizik yok,teşekkürler'}, {'kullanici': 'M** Ş**', 'elit': False, 'tarih': '15 Mart 2021', 'satici': 'Baysam', 'yildiz': 5, 'yorum': 'ekranı tam kaplayan muhteşem ürün memnun kaldık tavsiye ederiz'}, {'kullanici': 'feyza ozturk', 'elit': False, 'tarih': '21 Haziran 2021', 'satici': 'JoyPlus', 'yildiz': 5, 'yorum': 'çok kolay taktım 10 tl ye alınabilecek en güzel cam'}, {'kullanici': 'İbrahim Bosnalı', 'elit': False, 'tarih': '25 Nisan 2021', 'satici': 'JoyPlus', 'yildiz': 5, 'yorum': 'Muhteşem cidden'}, {'kullanici': '**** ****', 'elit': False, 'tarih': '26 Nisan 2021', 'satici': 'Adaman', 'yildiz': 1, 'yorum': 'İphone 6s plus cam sipariş verdim ama çok küçük geldi ve kargo hizli gelmedi Çok geçti'}, {'kullanici': '**** ****', 'elit': False, 'tarih': '16 Haziran 2021', 'satici': 'iphonoloji iletişim ', 'yildiz': 4, 'yorum': 'İlk defa internetten kırılmaz cam aldım ve gayet kaliteli çıktı.'}, {'kullanici': '**** ****', 'elit': False, 'tarih': '8 Aralık 2020', 'satici': 'Telehome', 'yildiz': 5, 'yorum': 'Sağlam geldi boyutları tam'}, {'kullanici': 'nevroz arslan', 'elit': False, 'tarih': '12 Mayıs 2021', 'satici': 'JoyPlus', 'yildiz': 5, 'yorum': 'İkinci siparişim 🤌🏻 Paketleme süper takmak çok rahattı teşekkürler 🙏🏻'}, {'kullanici': 'S** A**', 'elit': True, 'tarih': '8 Haziran 2021', 'satici': 'Adaman', 'yildiz': 5, 'yorum': 'ürünün hem figsti uygun hem görüldüğü gibi kaliteli bir ürün'}, {'kullanici': '**** ****', 'elit': False, 'tarih': '12 Mayıs 2021', 'satici': 'iphonoloji iletişim ', 'yildiz': 1, 'yorum': 'Ekranı tam kaplamıyor. Kenarları açık kalıyor.'}, {'kullanici': 's** O**', 'elit': False, 'tarih': '27 Mayıs 2021', 'satici': 'JoyPlus', 'yildiz': 5, 'yorum': 'Hızlı teslimat özenli paketlenmişti teşekkürler'}, {'kullanici': 'AHMET CELAL AKDOĞAN', 'elit': False, 'tarih': '22 Nisan 2021', 'satici': 'JoyPlus', 'yildiz': 5, 'yorum': 'Gayet başarılı ürün hızlı kargo teşekkürler'}, {'kullanici': '**** ****', 'elit': True, 'tarih': '26 Aralık 2020', 'satici': 'Telehome', 'yildiz': 3, 'yorum': 'Kutulama iyiydi, normal sert koruma fiyati karsiligi guzel'}, {'kullanici': 'Diyar Hekimoğlu', 'elit': False, 'tarih': '17 Nisan 2021', 'satici': 'JoyPlus', 'yildiz': 5, 'yorum': 'Çok iyi kutuları da çok hoş'}, {'kullanici': 'Muhammet Çavlan', 'elit': True, 'tarih': '8 Mart 2021', 'satici': 'Baysam', 'yildiz': 1, 'yorum': '2 tanesi kırık geldi paketide bıçak ile sanki 3 4 yerden kesmişler. bence indirimli diye kırık gönderildi'}, {'kullanici': 'Seda Kavran', 'elit': False, 'tarih': '9 Mart 2021', 'satici': 'Telehome', 'yildiz': 5, 'yorum': 'Tam istediğim gibi'}, {'kullanici': '**** ****', 'elit': False, 'tarih': '22 Mart 2021', 'satici': 'Baysam', 'yildiz': 1, 'yorum': 'Ben sizden iphone 6 s plus kırılmaz camını istedim siz başka telefonunkini göndermissiniz ön kamerayı kapatıyor'}, {'kullanici': '**** ****', 'elit': False, 'tarih': '21 Haziran 2021', 'satici': 'JoyPlus', 'yildiz': 2, 'yorum': 'Ürün şekil olarak güzel . Video izleyip güzelce taktım. 1 hafta oldu , kırılmaz camın kenarları çatlamaya başlamış. (Düşme vs olmadı) İyice çatlayacak,çöp olana kadar da öyle kullanacaksınız. Ucuz etin yahnisi hesabı. Ucuz zaten diyen alsın, yoksa tavsiye etmem'}, {'kullanici': 'S** K**', 'elit': False, 'tarih': '13 Haziran 2021', 'satici': 'JoyPlus', 'yildiz': 3, 'yorum': 'Cam güzel tam oldu ama paramparça geldi ya neden güzel paketleme yok bunun sonucu ne olucak şimdi yorumumu da yayınlatmıyorsunuz'}]}
```

## 💸 Bağış Yap

**[☕️ Kahve Ismarla](https://KekikAkademi.org/Kahve)**

## 🌐 Telif Hakkı ve Lisans

* *Copyright (C) 2022 by* [keyiflerolsun](https://github.com/keyiflerolsun) ❤️️
* [GNU GENERAL PUBLIC LICENSE Version 3, 29 June 2007](https://github.com/keyiflerolsun/pyTrendyol/blob/master/LICENSE) *Koşullarına göre lisanslanmıştır..*

## ♻️ İletişim

*Benimle iletişime geçmek isterseniz, **Telegram**'dan mesaj göndermekten çekinmeyin;* [@keyiflerolsun](https://t.me/KekikKahve)

##

> **[@KekikAkademi](https://t.me/KekikAkademi)** *için yazılmıştır..*