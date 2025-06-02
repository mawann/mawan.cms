# MAWAN CMS

* Ini adalah *Static CMS* yang tidak perlu pemrograman di sisi server dan tidak perlu database, yang berarti tidak perlu PHP, Node.js, PostgreSQL dan MySQL.
* Hanya perlu upload 1 file bernama index.html karena datanya dapat berada di mana pun, termasuk di Github.
* Data dibaca oleh JavaScript dan disajikan juga oleh JavaScript yang ada di peramban pengguna.
* Cocok ditempatkan di Cloudflare Pages.

Saran: Lebar gambar sebaiknya maksimal 720 pixel. Jangan lebih lebar agar loading halaman menjadi lebih cepat.

Petunjuk instalasi cepat:
```
cd /home/username
mkdir domain.com
cd domain.com
git clone https://github.com/mawann/mawan.cms.git

sudo cp mawan.cms/nginx.conf /etc/nginx/sites-available/domain.com
sudo vim /etc/nginx/sites-available/domain.com
sudo ln -s /etc/nginx/sites-available/domain.com /etc/nginx/sites-enabled/domain.com
sudo nginx -t
sudo ngins -s reload
```
Ganti *username* dan *domain.com* dengan kondisi yang ada di server anda.

Bila terjadi perbaikan kode di repository github.com/mawann/mawan.cms dan anda ingin mendapatkan versi terbaru, maka sila ketik:
```
cd /home/username/domain.com/mawan.cms
git pull
```

(C) Mawan A. Nugroho. 
