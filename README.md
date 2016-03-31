#Tìm hiểu cấu trúc ổ đia

##1.Khái niệm

<img src="http://i.prntscr.com/57178bf769aa4d8e863d23c9c605fa72.png">

-Là thiết bị dùng để lưu trữ dữ liệu trên bề mặt các tấm đĩa hình tròn phủ vật liệu từ tính.

##2.Cấu trúc

Bao gồm 4 phần:Cụm đĩa,cụm đầu đọc,cụm mạch điện,vỏ đĩa cứng

**a.Cụm đĩa**

Bao gồm 2 phần:Đĩa từ (platter) ,động cơ và trục quay.

-Đĩa từ(platter):Thường bằng nhôm hoặc thuỷ tinh, trên bề mặt được phủ một lớp vật liệu từ tính để chứa dữ liệu

<img src="http://i.prntscr.com/1509d791ca0642659b97d9b1e640f2ad.png">

- Sector:Sector là đơn vị chứa dữ liệu nhỏ nhất. Theo các chuẩn thông thường thì một sector chứa (dung lượng) 512 byte.
- Cluster:Cluster (liên cung) là một đơn vị lưu trữ gồm một hoặc nhiều sector.
- Track:-
 <ul>
  <li>Là vòng tròn đồng tâm trên một mặt của đĩa</li>
  <li>Track trên ổ đĩa cứng không cố định từ khi sản xuất, chúng có thể thay đổi vị trí khi định dạng cấp thấp ổ đĩa</li>
 </ul>
- Cylinder:
<ul>
  <li>Tập hợp các track cùng bán kính ở các mặt đĩa khác nhau tạo thành các cylinder (trụ)</li>
  <li>Nói một cách chính xác hơn thì: khi đầu đọc/ghi đầu tiên làm việc tại một track nào thì tập hợp toàn bộ các track trên các bề mặt đĩa còn lại mà các đầu đọc còn lại đang làm việc tại đó gọi là cylinder (cách giải thích này chính xác hơn bởi có thể xảy ra thường hợp các đầu đọc khác nhau có khoảng cách đến tâm quay của đĩa khác nhau do quá trình chế tạo).</li>
 </ul>
 
 -Động cơ và trục quay:
 
 <img src="http://i.prntscr.com/ac7e47a4dab84c48b51743a18f13f487.png">
 
 Các đĩa từ được gắn lên trục quay nối trực tiếp với động cơ quay đĩa cứng. Trục quay có nhiệm vụ truyền chuyển động quay từ động cơ đến các đĩa từ. Trục quay được chế tạo bằng các vật liệu nhẹ như hợp kim nhôm và được chế tạo tuyệt đối chính xác để đảm bảo trọng tâm của chúng không bị sai lệch.

**b.Cụm đầu đọc**

Bao gồm 2 phần:Đầu đọc/ghi và cần di chuyển đầu/đọc ghi

-Đầu đọc ghi:Cấu tạo gồm lõi ferit và cuộn dây,có công dụng đọc dữ liệu dưới dạng từ hoá trên bề mặt đĩa từ hoặc từ hoá lên các mặt đĩa khi ghi dữ liệu.

 <img src="http://i.prntscr.com/8b8c792e5ba8407182db77e406cb5271.png">
 
 -Cần di chuyển đầu đọc/ghi:
 <ul>
 <li>Để gắn đầu đọc/ghi vào.</li>
 <li>Có nhiệm vụ di chuyển theo phương song song với các đĩa từ ở một khoảng cách nhất định, dịch chuyển và định vị chính xác đầu đọc tại các vị trí từ mép đĩa đến vùng phía trong của đĩa (phía trục quay)</li>
 <li>Các cần di chuyển đầu đọc được di chuyển đồng thời với nhau do chúng được gắn chung trên một trục quay (đồng trục)</li>
 </ul>
 
 <img src="http://i.prntscr.com/3d46f56f50b140ef9f7e70afce4c69d4.png">
 
 **c.Cụm mạch điện**
 
 Bao gồm 4 phần:Mạch điều khiển,mạch xử lý dữ liệu,Bộ nhớ đệm và Jumper(cầu nối)
 
 -Mạch điều khiển:Có nhiệm vụ điều khiển động cơ đồng trục, điều khiển sự di chuyển của cần di chuyển đầu đọc để đảm bảo đến đúng vị trí trên bề mặt đĩa.
 
 -Mạch xử lý dữ liệu:Dùng để xử lý những dữ liệu đọc/ghi của ổ đĩa cứng.
 
  <img src="http://i.prntscr.com/88bdeadf4e914ac78de425b218ed894d.png">
  
  -Bộ nhớ đệm:Là nơi tạm lưu dữ liệu trong quá trình đọc/ghi dữ liệu. Dữ liệu trên bộ nhớ đệm sẽ mất đi khi ổ đĩa cứng ngừng được cấp điện.
  
  <img src="http://i.prntscr.com/9fb1f952f2814348a5b11fde9a0027a6.png">
  
  -Jumper(cầu nối):Lựa chọn chế độ làm việc của ổ đĩa cứng (SATA 150 hoặc SATA 300) hay thứ tự trên các kênh trên giao tiếp IDE (master hay slave hoặc tự lựa chọn), lựa chọn các thông số làm việc khác…
  
  <img src="http://i.prntscr.com/17a89cd20f9b404d8f72bb28fd999f39.png">
  
  **d.Vỏ đĩa cứng**
  
  Phần đế chứa các linh kiện gắn trên nó, phần nắp đậy lại để bảo vệ các linh kiện bên trong. Vỏ ổ đĩa cứng có chức năng chính nhằm định vị các linh kiện, chịu đựng sự va chạm (ở mức độ thấp) để bảo vệ ổ đĩa cứng và đảm bảo độ kín khít để không cho phép bụi được lọt vào bên trong của ổ đĩa cứng. Trên vỏ bảo vệ có các lỗ thoáng đảm bảo cản bụi và cân bằng áp suất giữa môi trường bên ngoài và môi trường không khí có độ sạch cao bên trong.
  
  <img src="http://i.prntscr.com/5c4de36528244ec89de25462d023edb9.png">

##3.Các câu lệnh hay dùng để thao tác với ổ cứng
* fdisk:Hiển thị các phân vùng và các chi tiết như kiểu hệ thống tập tin.
* cfdisk:Sfdisk là một tiện ích với một mục đích tương tự như fdisk, nhưng với nhiều tính năng hơn. Nó có thể hiển thị kích thước của mỗi phân vùng.
* parted:Hiển thị các phân vùng và các chi tiết như kiểu hệ thống tập tin,có thể thao tác với các ổ cứng dung lượng lớn (>2T) và nó cũng hiểu GPT Parition Table
* lsblk:Liệt kê ra tất cả các khối lưu trữ, trong đó bao gồm các phân vùng đĩa và ổ đĩa
