# Kitapi

Türkiye'nin ilk ve tek Türkçe kitap API'si.

<p align="left"> <img src="https://komarev.com/ghpvc/?username=beeali68&label=Repository%20views&color=0e75b6&style=flat" alt="beeali68" /> </p>

## Sorgular

### ISBN ile Sorgu:

`http://digittall.duckdns.org:5010/kitapi/v1/?isbn=<isbn_no>`

<isbn_no> yerine aramak istediğiniz ISBN no yazabilirsiniz.

Örnek Sorgu:

> http://digittall.duckdns.org:5010/kitapi/v1/?isbn=9789750738883

Sorgu Çıktısı:

```json
{
  "code": 200,
  "dt": "2024-06-19 02:56:49.402662",
  "message": [
    {
      "favori_sayisi": "3094",
      "fiyat": "105.13",
      "kategori": [
        "Kitap",
        "ÇocukKitapları",
        "100TemelEser",
        "Kitap",
        "Edebiyat",
        "Roman(Çeviri)"
      ],
      "kitap_adi": "Oliver Twist",
      "kitap_bilgileri": {
        "Boyut:": "12.5 x 19.5 cm",
        "Cilt Tipi:": "Karton Kapak",
        "Dil:": "TÜRKÇE",
        "ISBN:": "9789750738883",
        "Kağıt Cinsi:": "Kitap Kağıdı",
        "Sayfa Sayısı:": "576",
        "Yayın Tarihi:": "20.02.2024",
        "Çevirmen:": "Nihal Yeğinobalı"
      },
      "satis_sayisi": "3718",
      "yayinevi": "CAN YAYINLARI",
      "yazar": "Charles Dickens",
      "yorum_sayisi": "135"
    }
  ],
  "method": "GET",
  "status": "success"
}
```

### Kitap İsmi ile Sorgu:

`http://digittall.duckdns.org:5010/kitapi/v1/?kitap=<kitap_ismi>`

<kitap_ismi> yerine aramak istediğiniz kitabı yazabilirsiniz.

Örnek Sorgu:

> http://digittall.duckdns.org:5010/kitapi/v1/?kitap=nutuk

Sorgu Çıktısı:

```json
{
  "code": 200,
  "dt": "2024-06-16 15:20:13.479537",
  "message": [
    {
      "favori_sayisi": "1202",
      "fiyat": "181.25",
      "kategori": ["Kitap", "Siyaset", "Araştırma-İnceleme"],
      "kitap_adi": "Nutuk",
      "kitap_bilgileri": {
        "Boyut:": "15.5 x 23 cm",
        "Cilt Tipi:": "Karton Kapak",
        "Dil:": "TÜRKÇE",
        "ISBN:": "9789750760716",
        "Kağıt Cinsi:": "Kitap Kağıdı",
        "Sayfa Sayısı:": "1096",
        "Yayın Tarihi:": "26.10.2023"
      },
      "satis_sayisi": "820",
      "yayinevi": "CAN YAYINLARI",
      "yazar": "Mustafa Kemal Atatürk",
      "yorum_sayisi": "12"
    }
  ],
  "method": "GET",
  "status": "success"
}
```

### Yazar İsmi ile Sorgu:

`http://digittall.duckdns.org:5010/kitapi/v1/?yazar=<yazar_ismi>`

<yazar_ismi> yerine aramak istediğiniz yazarı yazabilirsiniz.

Örnek Sorgu:

> http://digittall.duckdns.org:5010/kitapi/v1/?yazar=Albert%20Camus

Sorgu Çıktısı:

```json
{
  "code": 200,
  "dt": "2024-06-16 15:20:13.479537",
  "message": [
    {
      "favori_sayisi": "6279",
      "fiyat": "63.81",
      "kategori": ["Kitap", "Edebiyat", "Roman(Çeviri)"],
      "kitap_adi": "Yabancı",
      "kitap_bilgileri": {
        "Boyut:": "12.5 x 19.5 cm",
        "Cilt Tipi:": "Karton Kapak",
        "Dil:": "TÜRKÇE",
        "ISBN:": "9789750748677",
        "Kağıt Cinsi:": "Kitap Kağıdı",
        "Sayfa Sayısı:": "112",
        "Yayın Tarihi:": "09.04.2021",
        "Çevirmen:": "Ayça Sezen"
      },
      "satis_sayisi": "10321",
      "yayinevi": "CAN YAYINLARI",
      "yazar": "Albert Camus",
      "yorum_sayisi": "110"
    }
  ],
  "method": "GET",
  "status": "success"
}
```

### Hem Yazar Hem de Kitap İsmi ile Sorgu:

`http://digittall.duckdns.org:5010/kitapi/v1/?yazar=<yazar_ismi>&kitap=<kitap_ismi>`

<yazar_ismi> yerine aramak istediğiniz yazarı, <kitap_ismi> yerine de aramak istediğiniz kitabı yazabilirsiniz.

Örnek Sorgu:

> http://digittall.duckdns.org/kitapi/v1/?yazar=charles%20dickens&kitap=Oliver%20Twist

```json
{
  "code": 200,
  "dt": "2024-06-19 02:52:41.087285",
  "message": [
    {
      "favori_sayisi": "382",
      "fiyat": "34.38",
      "kategori": [
        "Kitap",
        "ÇocukKitapları",
        "6-12Yaş",
        "Hikaye,Roman",
        "Masal",
        "Kitap",
        "ÇocukKitapları",
        "12+Yaş",
        "Hikaye,Roman",
        "Masal",
        "Kitap",
        "ÇocukKitapları",
        "100TemelEser"
      ],
      "kitap_adi": "Oliver TwistDünya Çocuk Klasikleri",
      "kitap_bilgileri": {},
      "satis_sayisi": "1690",
      "yayinevi": "ERDEM ÇOCUK YAYINLARI",
      "yazar": "Charles Dickens",
      "yorum_sayisi": "17"
    },
    {
      "favori_sayisi": "3094",
      "fiyat": "105.13",
      "kategori": [
        "Kitap",
        "ÇocukKitapları",
        "100TemelEser",
        "Kitap",
        "Edebiyat",
        "Roman(Çeviri)"
      ],
      "kitap_adi": "Oliver Twist",
      "kitap_bilgileri": {
        "Boyut:": "12.5 x 19.5 cm",
        "Cilt Tipi:": "Karton Kapak",
        "Dil:": "TÜRKÇE",
        "ISBN:": "9789750738883",
        "Kağıt Cinsi:": "Kitap Kağıdı",
        "Sayfa Sayısı:": "576",
        "Yayın Tarihi:": "20.02.2024",
        "Çevirmen:": "Nihal Yeğinobalı"
      },
      "satis_sayisi": "3718",
      "yayinevi": "CAN YAYINLARI",
      "yazar": "Charles Dickens",
      "yorum_sayisi": "135"
    },
    {
      "favori_sayisi": "322",
      "fiyat": "9.90",
      "kategori": [
        "Kitap",
        "ÇocukKitapları",
        "Hikaye",
        "Kitap",
        "ÇocukKitapları",
        "100TemelEser"
      ],
      "kitap_adi": "Oliver Twist (Resimli Çocuk Klasikleri) (Cep boy)",
      "kitap_bilgileri": {},
      "satis_sayisi": "1300",
      "yayinevi": "KARBON KİTAPLAR",
      "yazar": "Charles Dickens",
      "yorum_sayisi": "10"
    },
    {
      "favori_sayisi": "235",
      "fiyat": "15.00",
      "kategori": [
        "Kitap",
        "ÇocukKitapları",
        "Hikaye",
        "Kitap",
        "ÇocukKitapları",
        "100TemelEser"
      ],
      "kitap_adi": "Oliver Twist (Illustrated Children’s Classics)",
      "kitap_bilgileri": {},
      "satis_sayisi": "535",
      "yayinevi": "KARBON KİTAPLAR",
      "yazar": "Charles Dickens",
      "yorum_sayisi": "5"
    },
    {
      "favori_sayisi": "123",
      "fiyat": "13.00",
      "kategori": [
        "Kitap",
        "ÇocukKitapları",
        "Hikaye",
        "Kitap",
        "ÇocukKitapları",
        "100TemelEser"
      ],
      "kitap_adi": "Oliver Twist (Resimli Çocuk Klasikleri)",
      "kitap_bilgileri": {},
      "satis_sayisi": "534",
      "yayinevi": "KARBON KİTAPLAR",
      "yazar": "Charles Dickens",
      "yorum_sayisi": "6"
    }
  ],
  "method": "GET",
  "status": "success"
}
```
