# Library API RajaOngkir Akun Pro untuk CodeIgniter
Merupakan library CodeIgniter untuk mengkonsumsi API dari [RajaOngkir](http://rajaongkir.com). Library ini hanya dapat digunakan untuk API RajaOngkir dengan tipe akun **PRO**
## Instalasi
Copy file sesuai dengan lokasinya masing-masing.
## Konfigurasi
Buka "**application/config/rajaongkir.php**" dan masukkan API key Anda.
```php
$config['rajaongkir_api_key'] = "";
```
## Contoh Penggunaan
### Memuat library
```php
$this->load->library('rajaongkir');
```
### Melakukan request
```php
//Mendapatkan nama semua propinsi
$provinces = $this->rajaongkir->province();

//Mendapatkan nama semua kota
$cities = $this->rajaongkir->city();

//Mendapatkan nama kecamatan yang ada di Kabupaten Bantul (39)
$subdistrict = $this->rajaongkir->subdistrict(39);
```
### Response
Response yang dihasilkan berupa string JSON balasan dari RajaOngkir.
### Dokumentasi lebih lanjut
Silakan lihat code di dalam library, di dalamnya terdapat komentar yang dapat membantu Anda.
### Referensi
* [Dokumentasi RajaOngkir](http://rajaongkir.com/dokumentasi)
* [Petunjuk Penggunaan](https://makruvadigital.com/blog)
### Demo
[Web Demo Library API RajaOngkir CodeIgniter](http://app.makruvadigital.com)
