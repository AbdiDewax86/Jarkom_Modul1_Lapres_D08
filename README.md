# Jarkom_Modul1_Lapres_D08
## Display Filter
#### 1
http.host == "testing.mekanis.me"

![alt text](images/1_1.png)

Klik kanan pada salah satu hasil lalu Follow -> HTTP stream

![alt text](images/1_2.png)

Ditemukan webserver adalah nginx
#### 2
klik File > Export Object > HTTP > pada Text Filter ketik “Tim_Kunjungan_Kerja_BAKN_DPR_RI_ke_Sukabumi141436.jpg”

![alt text](images/2_1.png)
![alt text](images/2_2.png)
![alt text](images/2_3.png)
#### 3
http.request.uri contains "login" && http.host == "ppid.dpr.go.id"

![alt text](images/3.png)

Ditemukan username dan password:
username = 10pemuda
password = guncangdunia
#### 4
http.authbasic

![alt text](images/4.png)
#### 5
http.host == “aku.pengen.pw”
Pada salah satu hasil, cari Hypertext Transfer Protocol > Authorization

![alt text](images/5_1.png)
![alt text](images/5_2.png)
#### 6
ftp-data.command == "STOR Answer.zip"

![alt text](images/df answer.png)

di Answer.zip klik kanan > follow > TCP stream > ubah save data as dalam bentuk raw kemudian save
![alt text](images/dwld answer.png)

hasil download
< img src="images/6_2.png">

ftp-data.command == "STOR zipkey.txt"

![alt text](images/ftp zipkey.png)

di zipkey.txt klik kanan > follow > TCP stream > ubah save data as dalam bentuk raw kemudian save

![alt text](images/dwnld zipkey.png)

hasil open this

![alt text](images/6_4.png)
#### 7
frame contains "Yes.pdf"
![alt text](images/7_1.png)

Setelah ditemukan, klik kanan pada salah satu lalu klik Follow > TCP Stream > lalu save as raw dan save dalam bentuk .zip

![alt text](images/7_2.png)
![alt text](images/7_3.png)
![alt text](images/7_4.png)
#### 8
ftp.request.command == RETR

![alt text](images/8_1.png)
![alt text](images/8_2.png)

karena di follow > tcp stream pada readme menunjukkan Microsoft FTP service maka yang mendownload readme tersebut adalah Microsoft FTP service 
#### 9
ftp.request.command == USER || ftp.request.command == PASS

![alt text](images/9.png)

user = dhana
pass = dhana123
#### 10
frame contains "application/pdf"

![alt text](images/10_1.png)
![alt text](images/10_2.png)

hasil

![alt text](images/10_3.png)
## Capture Filter
#### 11
port 21
Pilih adapter for loopback traffic capture dan ketik port 21 di capture filter nya

![alt text](images/11_1.png)

muncul hasil ftp

![alt text](images/11_2.png)
#### 12
src port 80

![alt text](images/12.png)
#### 13
dst port 443

![alt text](images/13.png)
#### 14
src host 192.168.1.5
IP didapat dari command ipconfig di command prompt(Windows)

![alt text](images/14.png)
#### 15
dst host monta.if.its.ac.id

![alt text](images/15.png)
