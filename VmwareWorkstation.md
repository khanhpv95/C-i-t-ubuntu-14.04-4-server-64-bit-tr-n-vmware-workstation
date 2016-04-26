#Tìm hiểu về VmWare Workstation
##Mục lục
###[1. Tổng quan về vmware workstation](#tongquan)
###[1.1 Giới thiệu về vmware workstation](#gioithieu)
###[1.2 Tính năng nổi bật](#tinhnang)
###[2. Hướng dẫn cài đặt máy ảo](#caidat)
###[2.1 Tạo môi trường cài đặt máy ảo](#moitruong)
###[2.2 Hướng dẫn cài đặt win 7](#caidat1)
###[3. Giới thiệu về network](#net)
###[4. Tổng kết](#tongket)

======================================================
<a name="tongquan"></a>
#1. Tổng quan về vmware workstation
<a name="gioithieu"></a>
##1. Giới thiệu về vmware workstation
VMware workstation là một phần mềm giả lập mấy ảo của VMware, nó là một phần mềm tạo ra những máy tính ao, giống như một máy vật lý , chạy một hệ điều hành và các ứng dụng . Máy ảo sử dụng các nguồn tài nguyên phần cứng của máy vật lý mà nó chạy trên đó , những máy vật lý này được gọi là hệ thống máy chủ ảo hóa . Máy ảo có thiết bị ảo cung cấp các chức năng tương tự như vật lý phần cứng , nhưng  với những lợi ích bổ sung của nó là tính di động, dể quản lý và bảo mật.
VMware workstation có nhiều phiên bản cho nhiều hệ điếu hành khác nhau như Windows, Linux, Mac OS… VMware workstation là phần mềm có tính phí.
<a name="tinhnang"></a>
##2. Các tính năng nổi bật:
<ul> 
<li>Hỗ trợ đa dạng các nền tảng hệ điều hành khác nhau, bao gồm Windows, Macs, Linux…</li>
<li>Tích hợp khả năng Snapshot và Clone đối với máy ảo, hỗ trợ tối đa cho việc kiểm tra, chạy thử các ứng dụng, đồng thời tiết kiệm dung lượng và sử dụng hiệu quả bộ nhớ được cấp</li>
</ul>

======================================================
<a name="caidat"></a>

#2. Hướng dẫn cài đặt máy ảo
Ở đây, ta sẽ dùng vmware workstation 12 để cài đặt hệ điều hành win 7. 
<a name="moitruong"></a>
##2.1 Tạo môi trường
-**Bước 1:** Vào file chọn new virtual machine
<img src="http://imgur.com/0ke4amy">

-**Bước 2: ** Chọn custom và chọn next
<img src="http://imgur.com/8H7eZPc">

-**Bước 3:** Chọn Next.
<img src="http://imgur.com/7PesiFr">

-**Bước 4:** Chọn I will install the operating system later và chọn next.
-**Bước 5:** Chọn hệ điều hành muốn cài đặt và chọn next.
<img src="http://imgur.com/HwxXPLg">

-**Bước 6:** lưu tên máy cần cài đặt bà browser đến file lưu máy ảo.
<img src="http://imgur.com/aBA6FGs">

-**Bước 7:** Chọn BIOS và next.
<img src="http://imgur.com/ux1uUIb">

-**Bước 8:** Chọn số vi xử lí, số lõi và chọn next.
<img src="http://imgur.com/5vqBHSr">

-**Bước 9:** Chọn dung lượng RAM và chọn next.
<img src="http://imgur.com/yLrt47a">

-**Bước 10:** Chọn loại mạng muốn sử dụng, ta chọn mặc định là NAT và chọn next.
<img src="http://imgur.com/dkE3QKm">

-**Bước 11:** Chọn LSI logic SAS và chọn next.
<img src="http://imgur.com/8oCebD7">

-**Bước 12:** Chọn chuẩn disk SCSI và chọn next.
<img src="http://imgur.com/H49tzYq">

-**Bước 13:** Chọn Create a new virtual disk và chọn next. 
<img src="http://imgur.com/ZMVHSMd">

-**Bước 14:** Chọn dung lượng ổ cứng và chọn next. 
<img src="http://imgur.com/icsrIK5">

-**Bước 15:** Browser đến nơi lưu file disk ( tìm đến file lưu máy cần cài đặt) và chọn next. 
<img src="http://imgur.com/l7bbPzI">

-**Bước 16: ** Chọn Customize hardware để thiết lập đường dẫn file iso của hệ điều hành cần cài đặt. 
<img src="http://imgur.com/7u3GNui">

-**Bước 17:** Chọn finish và kết thúc việc tạo môi trường cài đặt máy ảo.
<img src="http://imgur.com/xWeUsNf">

<a name="caidat1"></a>
##2.2  Hướng dẫn cài đặt win 7 trên vmware workstation 12.
-**Bước 1:**  Chọn Power on this virtual machine.
<img src="http://imgur.com/ztDw1vE">

-**Bước 2:** Chọn next.
<img src="http://imgur.com/ONoEYMg">

-**Bước 3: ** Chọn I accept the license term và chọn next. 
<img src="http://imgur.com/QmadUnK">

-**Bước 4: ** Chọn next và chờ quá trình cài đặt. 
<img src="http://imgur.com/7i0kIMQ">

======================================================
<a name="net"></a>
#3. Giới thiệu về network.
Để configure network trên vmware ta chọn **edit** , **Virtual Network Editor..**
<img src="http://imgur.com/Ckm0qb6">


Trên tab Virtual Network Editor ta có thể thấy sau khi cài đặt Vmware Workstation thì ngay lập tức sinh ra cho ta 3 card đó là card Bridge, card NAT (vmnet8) và card host-only (vmnet1).
<img src="http://imgur.com/itb54vi">

**Ví dụ: configure card NAT:**
Để configure card NAT, t chọn vào card NAT, khi chọn card NAT, thì ta nhập vào dải IP cho card NAT, subnet mask và chọn NAT setting để thay đổi gateway cho card NAT. 

<img src="http://imgur.com/2e4tztP">
<img src="http://imgur.com/pmDONHT">

Chọn Ok để kết thúc việc cấu hình card NAT.


<a name="tongket"></a>
#4. Tổng kết
Bài viết nhằm mục đích giới thiệu tổng quát về Vmware workstation, cách cài đặt máy ảo và giới thiệu về netwok trên vmware.
Cảm ơn mọi người đã theo dõi.  











	



