# HEADLESS CMS

* Ini adalah contoh CMS yang tidak perlu PHP, MySQL, Node.JS, dan sebagainya.
* Hanya perlu upload 1 file bernama index.html karena datanya dapat berada di mana pun, termasuk di Github. 
* Cocok ditempatkan di Cloudflare Page.

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
sudo ngins -x reload
```
Ganti *username* dan *domain.com* dengan kondisi yang ada di server anda.

(C) Mawan A. Nugroho. 
