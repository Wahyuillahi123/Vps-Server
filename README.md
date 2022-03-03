# Vps Untuk Web Server nodejs
Konfigurasi VPS Server untuk nodejs web server dengan Sistem Operasi Debian 9

## Instal ZIP
digunakan untuk mengexstrak file zip
``` html
  $ apt-get install unzip
```

## Instal Node
digunakan untuk menjalankan server nodejs kita
``` html
  $ curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
  $ apt-get install build-essential nodejs -y
  $ sudo apt-get update && sudo apt-get upgrade
  $ sudo apt-get install -y nodejs
  $ node -v
  $ npm -v
```

## Instal MongoDB
digunakan untuk menginstal database pada server
``` html
  $ apt-get install dirmngr
  $ sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 9DA31620334BD75D9DCB49F368818C72E52529D4
  $ echo "deb http://repo.mongodb.org/apt/debian "$(lsb_release -sc)"/mongodb-org/4.0 main" | sudo tee /etc/apt/sources.list.d/mongodb.list
  $ apt-get update
  $ apt-get install mongodb-org -y

  $ sudo systemctl start mongod
  $ sudo systemctl enable mongod
  $ mongod -v
```

## Instal NPM Init
``` html
  $ npm init
```

## Instal PM2
digunakan untuk membuat server terus berjalan pada saat ssh ditutup
``` html
  $ npm install pm2 -g
```




