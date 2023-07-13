---
layout: post
title: Lịch sử điện toán đám mây & Trải nghiệm của mình
subtitle: Từ localhost đến serverless
cover-img: 
thumbnail-img: /assets/img/my-raspberrypi-4.png
share-img: /assets/img/my-raspberrypi-4.png
tags: [máy-chủ,serverless, devops, dedicate-server]
comments: true
---
> Internet ra đời được 30 năm và thế giới đã hoàn toàn thay đổi: kết nối con người, kết nối vạn vật, thay đổi cách chúng ta giao tiếp, học tập và giải trí. Tốc độ truy cập và lượng thông tin trên internet tăng theo cấp số nhân. Theo đó, công nghệ lưu trữ và truyền tải dữ liệu của các máy chủ cũng đã có những bước chuyển mình. 
>

## Lịch sử từ sách giáo khoa

- 1970 - 2000: Máy chủ là các `máy tính vật lý` đồ sộ về mặt vật lý, với giá thành rất đắt mà các công ty lớn mới mua được. Đến những năm 90 khi world wide web được phát minh và máy tính cá nhân đi vào cuộc sống khiến internet ngày càng phổ biến hơn. Nếu bạn muốn xây dựng 1 máy chủ, bạn sẽ mua (hoặc thuê) một máy tính lớn, mạnh mẽ để thực hiện. Việc này khá đắt tiền. Bạn mua máy chủ, cài đặt mọi thứ lên đó và chạy, chúng ta vẫn gọi chúng là kiến trúc monothic. Nếu bạn cài hai phần mềm xung khắc lẫn nhau, nhiều khả năng bạn phải mua thêm 1 máy chủ vật lý mới.

<figure>
<img src="/assets/img/my-raspberrypi-4.png" alt="team-work" style="border: 2px solid  gray;">
<figcaption>Server của mình trên Raspberrypi 4, 8GB RAM và 1Tb SSD.
</figcaption>
</figure>

- Những năm 200x, `công nghệ ảo hóa` xuất hiện. Với công nghệ này, 1 server có thể cài được nhiều máy ảo khác nhau tương đối phân tách nhau về mặt vật lý. Mỗi máy ảo có thể cài các hệ điều hành khác nhau. Dễ dàng thay đổi phần cứng (RAM, CPU ...) giữa các máy. Giá thành một "server" theo đó đã giảm đi rất nhiều. Xây dựng một ứng dụng có thể chỉ còn mất vài giờ.

<figure>
<img src="/assets/img/may-ao-virtual-box.png" alt="team-work" style="border: 2px solid  gray;">
<figcaption>Máy ảo Virtual Box, cài 1 server Jenkins, 1 server SonarquBe, 1 server CentOS để test.
</figcaption>
</figure>

- Những năm 201x, công nghệ `contaner` xuất hiện. Các container không cần phân tách dựa trên ảo hóa hệ điều hành nữa mà chúng phân tách lẫn nhau dưa trên `Cgroup` và `Namespace` trên máy chủ. Việc xây dựng ứng dụng (hệ điều hành, ứng dụng và các gói phụ thuộc) có thể chỉ mất vài phút.
- Từ 2015 - nay: Hệ thống quản lý container tự động (với số lượng lớn bất kì) như `Kubernetes`, `Docker Swarm`, `Nomad` ... giúp xây dựng và quản lý hàng chục hay hàng trăm ứng dụng chỉ trong vài phút. 

<figure>
<img src="/assets/img/docker-container.png" alt="team-work" style="border: 2px solid  gray;">
<figcaption>Thật tuyệt khi có thể vừa đọc sách vừa dùng câu lệnh để trải nghiệm hầu hết các ứng dụng chỉ trong vài phút nhờ container.
</figcaption>
</figure>

- Hiện nay Công nghệ `Serverless` đang ngày càng phổ biến và là xu hướng mới trong ngành công nghệ. Với mục tiêu giảm bớt thời gian làm việc (setup, quản lý, vận hành) các máy chủ, tăng thời gian xây dựng ứng dụng và tự động triển khai lên đám mây. Công nghệ **Serverless** được kì vọng là tương lai của điện toán đám mây. 

## Trải nghiệm từ bản thân

Mình, thật may mắn, đã được trải nghiệm gần như đầy đủ các công nghệ lưu trữ như trên. Và nhận thấy được khá nhiều bài học từ đó.

- Năm 2008, bên trung tâm Pháp Ngữ (Hay TT liên kết ĐH Pháp), Trường ĐH Bách Khoa Hà Nội có tổ chức một lớp giới thiệu và hướng dẫn cài đặt `HDH Ubuntu`. Lúc đó phong trào phần mềm mã nguồn mở đang lên khá cao. Mình còn nhớ được hướng dẫn cài đặt Ubuntu lên máy tính, được tặng 1 đĩa cài đặt. Mình hồi hộp mang về cài lên máy tính cá nhân như hệ điều hành thứ 2. Loay hoay 1 hồi, mình nhanh chóng xóa hết dữ liệu trên ổ D, vì format nhầm. :). Mình vẫn luôn giữ Ubunt như HDH thứ 2 trên máy tính nhiều năm sau đó. 
- Đến năm 2014, khi ra kinh doanh riêng, mình tìm hiểu các phần mềm bán hàng mã nguồn mở, đầu tiên mình sử dụng `Dolibarr` sau đó quyết định dùng `Odoo`. Cả hai phần mềm này đều yêu cầu cài đặt Dependency khá nhiều và các hướng dẫn đều sử dụng câu lệnh từ `Ternimal`. Mình quyết định chuyển hẳn sang sử dụng Ubuntu như hệ điều hành chính kể từ đó và dùng luôn đến tận bây giờ. :D
- `Cload Computing` đang là xu hướng chính hiện nay, khi chi phí lên mây đã rẻ đi đáng kể và các công ty phục vụ khách hàng quốc tế nhận thấy việc sử dụng hạ tầng khổng lồ từ các nhà cung cấp như AWS, GCP, Microsoft Azure có thể giúp họ nâng cao trải nghiệm cho khách hàng (giảm thời gian chờ, dễ mở rộng, lưu trữ, vận hành). Ở cấp độ cá nhân, mình vẫn sử dụng máy chủ vật lý ảo (`Dedicate Server`) để phục vụ công việc, chưa có cơ hội phục vụ khách hàng quốc tế nên chưa lên mây với AWS.

## Tạm kết
Cho dù xu thế Cloud Computing là phổ biến và ngày càng phổ biến. Các công nghệ khác (Máy chủ vật lý, Máy Ảo) vẫn có nhiều ứng dụng và đặc biệt tiết kiệm với những người hiểu biết công nghệ. 

Hi vọng mình sẽ có cơ hội tham gia các dự án để ứng dụng sức mạnh của đám mây và `serverless`

