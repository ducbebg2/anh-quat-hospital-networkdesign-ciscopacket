# anh-quat-hospital-networkdesign-ciscopacket
Đề tài này được sử dụng cho đồ án tốt nghiệp sử dụng trên môi trường Cisco Packet Tracer.

# Mô hình mạng đã được thiết kế
<img width="1998" height="1114" alt="Topology" src="https://github.com/user-attachments/assets/8212b02a-b9e6-4504-bc3f-f0ebed553754" />

# Yêu cầu đặt ra
- Thiết kế hệ thống mạng máy tính cho Bệnh viện Đa khoa Anh Quất xây dựng một mô hình mạng hoàn chỉnh phục vụ cho việc quản lý, trao đổi thông tin và vận hành các dịch vụ y tế tại bệnh viện. Hệ thống mạng được thiết kế theo mô hình phân tầng (Core – Distribution – Access), Sử dụng công nghệ VLAN, DHCP, NAT, VPN, cùng với các dịch vụ cần thiết như Mail Server, Web Server, DNS Server. Có bảo mật và tính sẵn sàng cao từ Firewall và ACL.

# Quy mô hệ thống
- Cơ sở 1
  + Gồm nhiều khoa/phòng (Cấp cứu, Tiếp đón, Nội, Ngoại, Sản, Nhi, Xét nghiệm, Hành chính, IT…)
  + Mỗi khoa sử dụng một VLAN riêng
  + Có hệ thống WiFi phủ sóng theo từng tầng
- Cơ sở 2
  + Gồm các phòng khám bệnh, xét nghiệm, hành chính, IT…
  + Mỗi phòng sử dụng VLAN riêng

# Dải địa chỉ mạng 
- Cơ sở 1: 172.16.0.0/24
- Cơ sở 2: 192.168.0.0/24
- DMZ Server: 99.0.0.0/28
- Kết nối WAN / ISP: 10.x.x.x và 11.x.x.x

# Hạn chế
- Hạn chế từ môi trường Cisco Packet Tracer chưa sử dụng được hết các chức năng của IPv6

# Hướng dẫn
- Cài đặt Cisco Packet Tracer, sau đó mở file [Toan bo he thong.pkt](./Toan%20bo%20he%20thong.pkt) 
Đây là file toàn bộ hệ thống được xây dựng, nếu muốn chạy đủ các chức năng nhưng đỡ rối mắt, hãy sử dụng file [Demo.pkt](./Demo.pkt).
Toàn bộ hệ thống mạng đã được cấu hình sẵn và hoạt động ổn định.
- Kiểm tra bằng cách:
  + Gửi gói tin giữa các máy tính
  + Sử dụng lệnh PING trong Cisco Packet Tracer

Nếu có vấn đề hoặc cần hỗ trợ, vui lòng liên hệ: ngvd.ngvanduc@gmail.com
