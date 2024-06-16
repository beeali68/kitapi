# Kitapi
Türkiye'nin ilk ve tek Türkçe kitap API'si.

## Sorgular
### Kitap İsmi ile Sorgu:

``http://digitall.mercusysddns.com:5095/kitapi/v1/?kitap=<kitap_ismi>``

<kitap_ismi> yerine aramak istediğiniz kitabı yazabilirsiniz.

Örnek Sorgu:

> http://digitall.mercusysddns.com:5095/kitapi/v1/?kitap=nutuk

Sorgu Çıktısı:

``
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
``

### Yazar İsmi ile Sorgu:

``http://digitall.mercusysddns.com:5095/kitapi/v1/?yazar=<yazar_ismi>``

<yazar_ismi> yerine aramak istediğiniz yazarı yazabilirsiniz.

Örnek Sorgu:

> http://digitall.mercusysddns.com:5095/kitapi/v1/?yazar=Albert%20Camus

Sorgu Çıktısı:

``
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
``

\#python \#api \#kitap \#nodejs \#javascript \#typescript \#go \#C#
