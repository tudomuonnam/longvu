---
layout: post
title: Quản lý linh hoạt (Agile)
subtitle: Vận hành dự án nhan hơn, đơn giản hơn, dễ thay đổi và sửa lỗi hơn
#cover-img: /assets/img/MVP-2048x1365.jpg
thumbnail-img: /assets/img/MVP-2048x1365.jpg
share-img: /assets/img/MVP-2048x1365.jpg
tags: [project-management, google-certificate, agile, scrum, scrum-master]
comments: true
---

> Quản lý linh hoạt (`Agile`) là phần mình tò mò muốn học nhất. Vì đây là khái niệm mới đối với bản thân mình. `Agile` có liên quan trực tiếp đến vị trí công việc mà mình quan tâm là `DevOps`.  
> 
> Khóa học cho mình thấy sự thay đổi góc nhìn lớn trong vận hành và phát triển team. Team phát triển từ bị động sang chủ động. Từ việc chỉ bắt đầu hoạt động từ giai đoạn 3 trong quản lý dự án, nay họ tự quản lý, phân chia và học hỏi, tự lên kế hoạch và nhận yêu cầu, hỗ trợ từ Stakeholder như Product Owner và Scrum Master.
>
> Quản lý linh hoạt là nhanh chóng đưa ra sản phẩm với những yêu cầu chính, để khách hàng kiểm thử. Khi khách hàng thấy sản phẩm, dịnh vụ chính yếu đó giải quyết được vấn đề  của họ rồi, mới phát triển thêm các tính năng phụ khác. Đây là khái niệm MVP (`Minimum Viable Product`) mà các startup hay nhắc tới. 
>
> Quản lý linh hoạt cũng giảm thiểu giấy tờ. Thay vì một danh sách các tài liệu, team xoay quanh `Product Backlogs Items` để phát triển các tính năng
>

> Quản lý linh hoạt thích hợp với các team nhỏ, muốn đi nhanh. Với các dự án mà khi khởi tạo, các yêu cầu là chưa rõ ràng và team có thể vừa làm vừa nhận thêm yêu cầu từ khách để hoàn thiện dần.
>
> Tuy nhiên quản lý linh hoạt cũng yêu cầu team phải chủ động hơn rất nhiều trong công việc.
> 
<figure>
<img src="/assets/img/MVP-2048x1365.jpg" alt="minimum-viable-product" style="border: 2px solid  gray;">
<figcaption>Suy nghĩ đúng về Sản phẩm với tính năng tối thiểu (MVP) <a href="https://inflectiv.co/2022/03/31/mvp-minimum-viable-product/">Nguồn ảnh</a></figcaption>
</figure>

## Quản lý dự án cổ điển (Từ cổ điển - 1990s)

Trước khi quản lý linh hoạt ra đời, quản lý dự án đã có một thời kì phát triển hàng trăm năm. Xã hội càng hiện đại, đòi hỏi phải xây dựng những dự án lớn, dài hàng năm, tiêu tốn nhiều tài nguyên, con người. Quản lý dự án dần ứng dụng khoa học, kĩ thuật để có được bộ công cụ quản lý tốt nhất với đầy đủ các bước đi để hoàn thành.
5 giai đoạn trong quản trị dự án:
- Khởi tạo dự án
- Lên kế hoạch
- Thực thi, theo dõi, điều chỉnh
- Đóng kế hoạch

Mỗi bước trong kế hoạch đều có những form tài liệu chuẩn để thực hiện, triển khai. Như
- Giai đoạn khởi tạo: Project Charter
- Giai đoạn lên kế hoạch: Bản chia nhỏ công việc (Work break down struct), Xác định các điểm trọng yếu cần hoàn thành (Critical Path method) ...
- Giai đoạn Thực thi: Các phương pháp giao tiếp, giải quyết xung đột, Tiêu chuẩn chất lượng, QA, QC
- Đóng dự án: Họp tổng kết (Retrospective), Báo cáo đóng dự án, Báo cáo ảnh hưởng của dự án ..

Quản trị dự án cổ điển sử dụng phương pháp thác nước: Mọi yêu cầu, suy tính đều được đặt lên bàn để bàn luận từ đầu, từ giai đoạn khởi tạo dự án đấy ạ. Khi chốt vấn đề rồi sẽ khó để thay đổi lại vì vấn đề này lại liên quan đến vấn đề kia, sửa một phần sẽ làm rối các phần còn lại. Do vậy quản trị dự án cổ điển sẽ rất khó chịu khi phát hiện có sai sót hoặc cần thay đổi giữa chừng. 

Một nhược điểm khác của quản trị dự án cổ điển là sử dụng rất nhiều tài liệu. Có thể gây rối cho người mới và không thể theo kịp, quản lý kịp, cập nhật kịp các vấn đề phát sinh

## Quản lý linh hoạt (1990s - nay)

 Với sự ra đời của máy tính cá nhân đã khiến các dòng đời của các dự án nhanh hơn, yêu cầu sản phẩm được đưa ra thị trường càng sớm càng tốt để khách hàng trải nghiệm. Yêu cầu sản phẩm có thể được chỉnh sửa nhanh và ngay khi khách hàng phản hồi. Tư duy của thị trường, của nhóm phát triển thay đổi đòi hỏi tư duy, công cụ quản lý thay đổi theo. 
 
 Tuyên ngôn của `quản lý linh hoạt` là:
 - Ưu tiên **Cá nhân và tương tác** hơn quy trình và công cụ
 - Ưu tiên **phần mềm** hơn là các bộ tài liệu
 - Ưu tiên **hợp tác với khách hàng** hơn là đàm phán hợp đồng
 - Ưu tiên **ứng phó với sự thay đổi** hơn là làm theo kế hoạch

Cần lưu ý là không phải tất cả các dự án đều nên sử dụng `quản lý linh hoạt`. Tùy theo dự án, con người, yêu cầu của các bên mà sử dụng phương pháp quản lý cổ điển hay tinh gọn cho hiệu quả. Nhiều dự án có thể kết hợp cả 2 phương pháp.

## Scum - quản lý linh hoạt áp dụng trong dự án phần mềm

Scum áp dụng tinh thần của quản lý linh hoạt, áp dụng (chủ yếu) trong các dự án phần mềm. Scum làm chi tiết hợn quản lý tinh gọn trong môi trường cụ thể.

### Ba giá trị cốt lõi của Scum là: 
 - **Tính minh bạch**. Kết quả công việc hiển thị rõ ràng cho các bên liên quan
 - **Tính kiểm tra**: Liên tục kiểm tra quá trình phát triển để phát hiện ra lỗi sai càng sớm càng tốt.
 - **Tính thích ứng**. Team luôn tình cách thay đổi sản phẩm, quy trình để sai sót. Đón nhận sự thay đổi như một phần phát triển của dự án.

### Team làm việc theo Scum gồm:

- Scrum Master: Người hướng dẫn team áp dụng phương pháp Scum để hoàn thành dự án. Khác với `Project Manager`, `Scrum Master` thiên về hướng dẫn hơn là quản lý team. Nói một cách đơn giản hơn: Team là người có vai trò dẫn dắt, quyết định thay vì ở vị trí bị động như cách quản lý truyền thống (với Project Manager)
   
- Product Owner: Có trách nhiệm tối đa hóa giá trị của sản phẩm đầu ra bằng cách đóng vai khách hàng và nói lên mong muốn khách hàng về sản phẩm. Trách nhiệm của Product Owner:
  - Tạo ra mục tiêu của sản phẩm (goals)
  - Tạo ra Danh sách tính năng của sản phẩm (Product backlog items) 

- Team phát triển. Chị trách nhiệm xây dựng sản phẩm. Họ tự:
  - Lập kế hoạch cho từng giai đoạn phát triển (`Sprints`), hoàn thành việc xây dựng tính năng sản phẩm (`Product backlogs items`)
  - Tự quản lý chất lượng bằng bản định nghĩa hoàn thành
  - Tự thay đổi kế hoạch hằng ngày để hoàn thành mục tiêu của từng giai đoạn
  - Chịu trách nhiệm về công việc của mình

### Các hoạt động của team gồm:

- Các giai đoạn phát triển (Sprints). 
- `Sprint`: Mỗi giai đoạn phát triển được chia thành các khoảng thời gian gọi là(`Sprint`) nhằm thực hiện một nhiệm vụ cụ thể (`Product goals`). Sprints thường kéo dài 1 tháng hoặc ít hơn
  
- `Sprint planning`: Lên kế hoạch giải quyết các `Product backlogs items` trong Sprint tiếp theo. Hoàn thành chúng như thế nào? Tại sao lại lựa chọn những items đó để thực hiện (trước). Các cuộc họp Sprint Planning diễn ra trước mỗi Sprint.
  
- `Daily scrum`: Xem xét những việc đã làm và sẽ làm trong ngày để hoàn thành mục tiêu. Thường là meeting 15 phút hàng ngày

- `Sprint Review`: Họp cuối mỗi Sprint, kiểm tra lại việc hoàn thành mục tiêu. Nhận phản hồi từ Product Owner, Stakeholder về công việc đã làm trong Sprint

- `Retrospective`: Buổi tổng kết trong team về các vấn đề cần rút ra, học được từ Sprint vừa qua. 

## Công cụ được sử dụng trong Scum
Với giá trị cốt lõi là tính minh bạch, công cụ trong Scum hướng tới sự trực quan, đơn giản để những người có liên quan đều có thể hiểu và nắm được tiến độ công việc.
- `Kanban`: Bảng chia công việc thành các mục: Lên kế hoạch, đang thực hiện, đã thực hiện xong... Nhằm theo dõi tiến độ hoàn thành. Công việc được gắn tới từng thành viên để tiện theo dõi. Tránh nhân viên bị gắn quá nhiều công việc (quá tải)
- `Extreme Programming`(XP): Nhằm mục tiêu cải thiện chất lượng sản phẩm và tăng năng lực phản ứng với sự thay đổi của khách hàng. Các hoạt động của XP gồm: Thiết kế, Coding, Testing và Listening. 
Cách làm mới với XP: 
  - `Pair Programming`: Hai người làm cùng 1 task, cùng thời gian. 
  - `Continous Intergration/ Continous Delivery`
  - Tránh thiết kế toàn bộ hệ thống trước. Thiết kế vừa đủ để hoàn thành mục tiêu trước rồi cải thiện sau đó
  - Luôn viết test, không phải tài liệu. Test nhằm 2 mục đích: Nói với team bạn built gì và so sánh cái bạn buid với cái dự định built 
  - Ứng dụng `Lean manufacturing principles` 

## DevOps

Là sự kết hợp của Phát triển sản phẩm (Developlent) và Hoạt động (Operation). Hai hoạt động này, trước đây tách rời nhau hoàn toàn. Sản phẩm trong giai đoạn phát triển sẽ chưa được triển khai, mãi đến khi được đóng gói hoàn chỉnh rồi mới được chuyển giao cho khách hàng để hoạt động.

Áp dụng tinh thần của `Agile` cụ thể hóa qua `Scum` về việc rút ngắn quá trình chuyển giao sản phẩm, đưa khách hàng vào quá trình phát triển. Liên tục đưa ra sản phẩm để nhận phản hồi. DevOps được sinh ra để hiện thực hóa quá trình này.

DevOps đẩy nhanh quá trình phát triển phần mềm nhờ thực thi hai công việc chính

1. Continous Intergration
2. Continous Deployment
3. Infrastructure as Code

Mình sẽ có những bài viết thiên về kĩ thuật của DevOps trong thời gian tới 

## Tạm kết

Quản lý dự án linh hoạt được nói nhiều nhưng có lẽ vẫn chưa quá phổ biến trên thực tế ở Việt Nam. Mình có hỏi công ty cũ về vị trí DevOps nhưng trong công ty không có vị trí này và Quản trị dự án vẫn làm như cách đây 14 năm mình ở đó. Quản lý linh hoạt có lẽ được sử dụng nhiều hơn bởi các startup và các công ty làm việc hoặc outsource từ nước ngoài. 

Tuy nhiên, theo quan điểm của mình, đây là xu hướng không thể tránh được. Và vị trí DevOps khá mới với rất nhiều yêu cầu về kiến thức (cả phần Dev và Ops) có thể sẽ `hot` trong thời gian tới. Có điều các công ty hiện nay vừa yêu cầu kiến thức cao, vừa yêu cầu kinh nghiệm nhiều. Khá khó để đạt được cả 2 trong giai đoạn này.


## Nguồn tham khảo:
1. [https://www.coursera.org/learn/agile-project-management](https://www.coursera.org/learn/agile-project-management)
2. [https://management.org/history-of-project-management](https://management.org/history-of-project-management)
3. [https://agilemanifesto.org/](https://agilemanifesto.org/)
4. [https://hocvienagile.com/devops-la-gi-ky-nang-can-thiet-devops-engineer/](https://hocvienagile.com/devops-la-gi-ky-nang-can-thiet-devops-engineer/)