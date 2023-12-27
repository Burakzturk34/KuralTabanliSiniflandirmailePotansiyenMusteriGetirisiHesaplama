# Potansiyel Müşteri Getirisi Hesaplama

Bu proje, bir oyun şirketinin müşterilerinin özelliklerini kullanarak seviye tabanlı (level based) yeni müşteri tanımları (persona) oluşturmayı ve bu tanımlara göre segmentler oluşturup potansiyel gelecek müşterilerin şirkete ortalama kazandırabileceği miktarı tahmin etmeyi amaçlar.

## İş Problemi

Bir oyun şirketi, müşterilerinin demografik özellikleri ve harcama alışkanlıkları üzerinden yeni müşteri profilleri oluşturmak ve bu profillere göre gelecek müşterilerin şirkete ortalama ne kadar gelir sağlayabileceğini tahmin etmek istemektedir.

## Veri Seti Hikayesi

"persona.csv" veri seti, uluslararası bir oyun şirketinin sattığı ürünlerin fiyatlarını ve bu ürünleri satın alan kullanıcıların bazı demografik bilgilerini içermektedir.

- **Price:** Müşterinin harcama tutarı
- **Source:** Müşterinin bağlandığı cihaz türü
- **Sex:** Müşterinin cinsiyeti
- **Country:** Müşterinin ülkesi
- **Age:** Müşterinin yaşı

## Proje Görevleri

### Görev 1

1. `persona.csv` dosyasını okutunuz ve veri seti ile ilgili genel bilgileri gösteriniz.
2. Kaç unique SOURCE vardır? Frekansları nedir?
3. Kaç unique PRICE vardır?
4. Hangi PRICE'dan kaçar tane satış gerçekleşmiş?
5. Hangi ülkeden kaçar tane satış olmuş?
6. Ülkelere göre satışlardan toplam ne kadar kazanılmış?
7. SOURCE türlerine göre satış sayıları nedir?
8. Ülkelere göre PRICE ortalamaları nedir?
9. SOURCE'lara göre PRICE ortalamaları nedir?
10. COUNTRY-SOURCE kırılımında PRICE ortalamaları nedir?

### Görev 2

- COUNTRY, SOURCE, SEX, AGE kırılımında ortalama kazançlar nedir?

### Görev 3

- Çıktıyı PRICE'a göre sıralayınız.

### Görev 4

- Indekste yer alan isimleri değişken ismine çeviriniz.

### Görev 5

- AGE değişkenini kategorik değişkene çeviriniz ve agg_df'e ekleyiniz.

### Görev 6

- Yeni level based müşterileri tanımlayınız ve veri setine değişken olarak ekleyiniz.

### Görev 7

- Yeni müşterileri (USA_ANDROID_MALE_0_18) segmentlere ayırınız.

### Görev 8

- Yeni gelen müşterileri sınıflandırınız ve ne kadar gelir getirebileceğini tahmin ediniz.

## Kurulum

1. Depoyu yerel makinenize klonlayın: `git clone https://github.com/kullaniciadi/projeadi.git`
2. Proje dizinine gidin: `cd projeadi`
3. Gerekli bağımlılıkları yükleyin: `pip install -r requirements.txt`
4. Veritabanını oluşturun: `python manage.py migrate`
5. Projeyi başlatın: `python manage.py runserver`

## Kullanım

Projeyi başlattıktan sonra, tarayıcınızda http://localhost:8000 adresine giderek projeyi görüntüleyebilirsiniz.
