# Add 2 card mạng trên máy Ubuntu Server, cấu hình cho 2 card mạng
##Các bước tiến hành
**Bước 1:**  Power off và add thêm 2 card vmnet1 và vmnet 2

<img src="http://i.imgur.com/WvW7QtR.png">

<img src="http://i.imgur.com/xNsAaAv.png">

img src="http://i.imgur.com/eEOx7XR.png">

**Bước 2:** Power on và dùng lệnh `ip a` để kiểm tra xem đã nhận card hay chưa. 

<img src="http://i.imgur.com/RAXNmgk.png">

**Bước 4:** Dùng lệnh `vi /etc/network/interfaces` để cấu hình card mạng.

<img src="http://i.imgur.com/WtKHTmb.png">

**Bước 5:** Dùng lệnh sau để restart card mạng:
```
ifdown -a
ifup -a
```
sau khi restart card mạng thì sử dụng lệnh `ip a` để kiểm tra xem card đã nhận ip chưa.

<img src="http://i.imgur.com/FtehZWS.png">

#Tổng kết
<li>Bài viết ghi chép về cách add card mạng và cấu hình card mạng trên Ubuntu server.</li>
<li>Cảm ơn đã theo dõi.</li>


