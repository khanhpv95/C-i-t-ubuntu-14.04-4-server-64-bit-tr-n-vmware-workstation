# Thiết lập IP tĩnh và động bằng cách sửa file và câu lệnh.
##[1. Gán ip tức thời bằng câu lệnh](#caulenh)
##[2. Đặt ip tĩnh bằng cách sửa file](#iptinh)
##[3. Đặt ip động bằng cách sửa file](#dong)


<a name="caulenh"></a>
##1. Gán ip tức thời bằng câu lệnh
-Để gán ip tức thời cho card mạng ta sử dụng câu lệnh: 
<ul>
<li>**ifconfig ethX** `IP-address` **netmask** `subnet-mask`</li>
</ul>
-Sau khi gán thành công, ta sử dụng câu lệnh `ip a` để kiểm tra.

<img src="http://i.imgur.com/RcoeVR0.png">

-Để gán gateway cho card mạng ta sử dụng câu lệnh:
<ul>
<li>**route add default gw** `địa chỉ gateway`</li>
</ul>
-Sau khi gán gateway ta `ping ra 8.8.8.8` để kiểm tra. 

<img src="http://i.imgur.com/7fTo2Ua.png">


<a name="iptinh"></a>
##2. Đặt ip tĩnh bằng cách sửa file

-Để đặt ip tĩnh bằng câu lệnh, ta sử dụng câu lệnh : `vi /etc/network/interfaces` và thiết lập IP, netmask, gateway,..:

<img src="http://i.imgur.com/IUHAe3Y.png">

-Sau khi thiết lập ip cho card mạng, ta reboot máy và `ping 8.8.8.` để kiểm tra.


<a name="dong"></a>

##3. Đặt ip động bằng sửa file:

Để đặt ip động, ta sử dụng câu lệnh sau: 
`vi/ etc/network/interfaces`
Và sửa file cấu hình network như sau:

<img src="http://i.imgur.com/f9umTNs.png">

-Sau khi thiết lập dhcp ta reboot máy.

##3. Tổng kết
<li>Bài viết tổng hợp cách Thiết lập IP tĩnh và động bằng cách sửa file và câu lệnh.</li>
Cảm ơn đã theo dõi.
































