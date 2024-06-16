# Kitapi
Türkiye'nin ilk ve tek Türkçe kitap API'si.

<p align="left"> <img src="https://komarev.com/ghpvc/?username=beeali68&label=Repository%20views&color=0e75b6&style=flat" alt="beeali68" /> </p>

## Sorgular
### Kitap İsmi ile Sorgu:

``http://digitall.mercusysddns.com:5095/kitapi/v1/?kitap=<kitap_ismi>``

<kitap_ismi> yerine aramak istediğiniz kitabı yazabilirsiniz.

Örnek Sorgu:

> http://digitall.mercusysddns.com:5095/kitapi/v1/?kitap=nutuk

Sorgu Çıktısı:

```json
{
  "code": 200,
  "dt": "2024-06-16 15:20:13.479537",
  "message": [
    {
    "fiyat": "181.25",
    "id": 1337,
    "kategori": "Kitap ; Siyaset ; Araştırma-İnceleme ; ",
    "kitap_adi": "Nutuk",
    "yayinevi": "CAN YAYINLARI",
    "yazar": "Mustafa Kemal Atatürk"
    }
  ],
  "method": "GET",
  "status": "success"
}
```

### Yazar İsmi ile Sorgu:

``http://digitall.mercusysddns.com:5095/kitapi/v1/?yazar=<yazar_ismi>``

<yazar_ismi> yerine aramak istediğiniz yazarı yazabilirsiniz.

Örnek Sorgu:

> http://digitall.mercusysddns.com:5095/kitapi/v1/?yazar=Albert%20Camus

Sorgu Çıktısı:

```json
{
  "code": 200,
  "dt": "2024-06-16 15:20:13.479537",
  "message": [
    {
    "fiyat": "66.70",
    "id": 189,
    "kategori": "Kitap ; Edebiyat ; Roman (Çeviri) ; ",
    "kitap_adi": "Yabancı",
    "yayinevi": "CAN YAYINLARI",
    "yazar": "Albert Camus"
    }
  ],
  "method": "GET",
  "status": "success"
}
```

### Hem Yazar Hem de Kitap İsmi ile Sorgu:

``http://digitall.mercusysddns.com:5095/kitapi/v1/?yazar=<yazar_ismi>&kitap=<kitap_ismi>``

<yazar_ismi> yerine aramak istediğiniz yazarı, <kitap_ismi> yerine de aramak istediğiniz kitabı yazabilirsiniz.

Örnek Sorgu:

> http://digitall.mercusysddns.com:5095/kitapi/v1/?yazar=charles%20dickens&kitap=Oliver%20Twist

```json
{
  "code": 200,
  "dt": "2024-06-16 15:42:20.612382",
  "message": [
    {
    "fiyat": "62.50",
    "id": 2035,
    "kategori": "Kitap ; Ãocuk KitaplarÄą ; 6-12 YaÅ ; Hikaye, Roman ; Masal ; Kitap ; Ãocuk KitaplarÄą ; 12+ YaÅ ; Hikaye, Roman ; Masal ; Kitap ; Ãocuk KitaplarÄą ; 100 Temel Eser ; ",
    "kitap_adi": "Oliver Twist",
    "yayinevi": "BİLGİ ÇOCUK KİTAPLARI",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "34.38",
    "id": 2548,
    "kategori": "Kitap ; Çocuk Kitapları ; 6-12 Yaş ; Hikaye, Roman ; Masal ; Kitap ; Çocuk Kitapları ; 12+ Yaş ; Hikaye, Roman ; Masal ; Kitap ; Çocuk Kitapları ; 100 Temel Eser ; ",
    "kitap_adi": "Oliver TwistDünya Çocuk Klasikleri",
    "yayinevi": "ERDEM ÇOCUK YAYINLARI",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "105.13",
    "id": 3099,
    "kategori": "Kitap ; Çocuk Kitapları ; 100 Temel Eser ; Kitap ; Edebiyat ; Roman (Çeviri) ; ",
    "kitap_adi": "Oliver Twist",
    "yayinevi": "CAN YAYINLARI",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "9.90",
    "id": 7370,
    "kategori": "Kitap ; Çocuk Kitapları ; Hikaye ; Kitap ; Çocuk Kitapları ; 100 Temel Eser ; ",
    "kitap_adi": "Oliver Twist (Resimli Çocuk Klasikleri) (Cep boy)",
    "yayinevi": "KARBON KİTAPLAR",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "15.00",
    "id": 12032,
    "kategori": "Kitap ; Çocuk Kitapları ; Hikaye ; Kitap ; Çocuk Kitapları ; 100 Temel Eser ; ",
    "kitap_adi": "Oliver Twist (Illustrated Children’s Classics)",
    "yayinevi": "KARBON KİTAPLAR",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "165.02",
    "id": 12686,
    "kategori": "Kitap ; Çocuk Kitapları ; 100 Temel Eser ; Kitap ; Edebiyat ; Roman (Çeviri) ; ",
    "kitap_adi": "Oliver Twist (İngilizce)",
    "yayinevi": "KARBON KİTAPLAR",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "13.00",
    "id": 13611,
    "kategori": "Kitap ; Çocuk Kitapları ; Hikaye ; Kitap ; Çocuk Kitapları ; 100 Temel Eser ; ",
    "kitap_adi": "Oliver Twist (Resimli Çocuk Klasikleri)",
    "yayinevi": "KARBON KİTAPLAR",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "192.50",
    "id": 37867,
    "kategori": "Kitap ; Çocuk Kitapları ; 100 Temel Eser ; ",
    "kitap_adi": "Oliver Twist (Tam Metin)",
    "yayinevi": "BEYAN YAYINLARI",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "80.00",
    "id": 39125,
    "kategori": "Kitap ; Çocuk Kitapları ; 6-12 Yaş ; Hikaye, Roman ; Masal ; Kitap ; Çocuk Kitapları ; 100 Temel Eser ; ",
    "kitap_adi": "Oliver Twist 100 Temel Eser",
    "yayinevi": "NAR ÇOCUK YAYINLARI",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "41.65",
    "id": 44324,
    "kategori": "Kitap ; DiÄer Dildeki YayÄḟnlar ; ÄḞngilizce ; ",
    "kitap_adi": "Oliver Twist Stage 4 İngilizce Hikaye (Alıştırma Ve Sözlük İlaveli)",
    "yayinevi": "DORLİON YAYINLARI",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "41.65",
    "id": 53228,
    "kategori": "Kitap ; Çocuk Kitapları ; 6-12 Yaş ; Hikaye, Roman ; Masal ; Kitap ; Çocuk Kitapları ; 100 Temel Eser ; ",
    "kitap_adi": "Oliver Twist Dünya Çocuk Klasikleri (7 - 12 Yaş)",
    "yayinevi": "DORLİON YAYINLARI",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "80.00",
    "id": 58857,
    "kategori": "Kitap ; Çocuk Kitapları ; Roman ; Kitap ; Çocuk Kitapları ; 100 Temel Eser ; ",
    "kitap_adi": "Oliver Twist İlk Gençlik Dizisi",
    "yayinevi": "NAR ÇOCUK YAYINLARI",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "-",
    "id": 87596,
    "kategori": "Kitap ; Çocuk Kitapları ; Roman ; Kitap ; Çocuk Kitapları ; 100 Temel Eser ; ",
    "kitap_adi": "Oliver Twist (4-E-12)",
    "yayinevi": "YENİ ZAMANLAR SAHAF (2. El Kitaplar)",
    "yazar": "Charles Dickens"
    },
    {
    "fiyat": "195.00",
    "id": 97904,
    "kategori": "Kitap ; Diğer Dildeki Yayınlar ; İngilizce ; ",
    "kitap_adi": "Oliver Twist",
    "yayinevi": "PAPER BOOKS",
    "yazar": "Charles Dickens"
    }
  ],
  "method": "GET",
  "status": "success"
}
```
