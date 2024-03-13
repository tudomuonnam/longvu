---
layout: post
title: Lợi nhuận logarith và lợi nhuận trung bình đơn giản
subtitle: Cách sử dụng, khi nào sử dụng 
cover-img: 
thumbnail-img: /assets/img/image.jpg
share-img: /assets/image.jpg
tags: [log return,simple return, finance]
comments: true
---

> Lợi nhuận logrith (ln(Pt - P(t-1)) và lợi nhuận trung bình đơn giản (1/2(Pt - P(t-1)) thường được dùng rộng rãi trong phân tích. Nhưng sự giống và khác nhau của 2 loại lợi nhuận này, khi nào sử dụng loại nào? Dưới đây là trích đoạn của một paper có dẫn nguồn ở dưới. Dịch bằng gg translate. Tài liệu dùng để lưu trữ.
 

**1/. Một vài nhận xét về hai phương pháp**

i) Lợi nhuận logarit có thể được hiểu là lợi nhuận gộp liên tục. Điều này có nghĩa là, đối với các quá trình không ngẫu nhiên, chẳng hạn như lợi nhuận của chứng khoán có lãi suất cố định không rủi ro được giữ đến ngày đáo hạn, khi sử dụng lợi nhuận logarit, tần suất gộp không quan trọng và lợi nhuận trên các tài sản có thể dễ dàng được so sánh hơn.

ii) Sử dụng lợi nhuận gộp liên tục (logarit) là thuận lợi khi xem xét lợi tức nhiều kỳ vì lợi tức gộp liên tục nhiều kỳ chỉ đơn giản là tổng của các lợi nhuận gộp liên tục một kỳ. Lợi nhuận gộp liên tục có tính cộng theo thời gian và dễ dàng rút ra các đặc tính chuỗi thời gian của các quy trình cộng hơn so với các quy trình nhân (xem Campbell et al, 1997, trang 11). Trong bối cảnh này, một số nghiên cứu đã chỉ ra rằng việc sử dụng lợi nhuận đơn giản để ước tính lợi nhuận trên
thời gian dài hơn có thể không đạt yêu cầu (xem Roll, 1983 và Dissanaike, 1993).

iii) Việc sử dụng lợi nhuận logarit ngăn giá chứng khoán trở nên âm trong các mô hình lợi nhuận chứng khoán (xem Jorion, 2001, trang 100).

iv) Nếu giá chứng khoán tuân theo chuyển động hình học Brownian (một mô hình biến động giá chứng khoán rất phổ biến được sử dụng, chẳng hạn như trong mô hình định giá quyền chọn Black-Scholes) thì lợi nhuận logarit của chứng khoán thường được phân phối.

v) Để dự báo lợi nhuận tích lũy trong tương lai, việc gộp liên tục lợi nhuận logarit dự kiến sẽ đưa ra hướng dẫn tốt hơn về lợi nhuận tích lũy trung bình trong tương lai (lợi nhuận mà các nhà đầu tư có thể nhận ra) so với lợi nhuận đơn giản kỳ vọng gộp (Hughson và cộng sự, 2006).

vi) Lợi nhuận logarit xấp xỉ bằng lợi nhuận đơn giản. Kiểm tra công thức kết nối logarit và trả về đơn giản RLt = ln(1+ RSt) cho thấy miễn là RSt không quá lớn (Rozeff và Kinney, 1976, p380, đề xuất RSt ≤ 0,15) thì lợi nhuận logarit và trả về đơn giản rất giống nhau về kích cỡ. Mặc dù điều này là đúng nhưng điều quan trọng là không được suy luận sai từ đó rằng giá trị trung bình của một tập hợp lợi nhuận được đo bằng lợi nhuận logarit nhất thiết phải rất giống với giá trị trung bình của cùng một tập hợp lợi nhuận được đo bằng lợi nhuận đơn giản. Lý thuyết đằng sau kết quả này được trình bày trong phần tiếp theo và Phụ lục V

**2\. Lưu ý khi dùng lợi nhuận logrith**

Có một số đặc tính không mong muốn liên quan đến lợi nhuận logarit:

i) Lợi nhuận logarit không đưa ra thước đo trực tiếp về sự thay đổi tài sản của nhà đầu tư trong một khoảng thời gian cụ thể. Theo định nghĩa, thước đo thích hợp để sử dụng cho mục đích này là lợi nhuận đơn giản trong khoảng thời gian đó. Đối với các hệ thống không ngẫu nhiên, đây là một khó khăn không đáng kể vì có sự tương ứng một-một giữa lợi nhuận logarit và lợi nhuận đơn giản P5. Tình huống trở nên rắc rối hơn nhiều đối với các hệ thống ngẫu nhiên như được thảo luận ở iii\) dưới đây.

ii) Sự khác biệt giữa lợi nhuận logarit trung bình của một chứng khoán trong một khoảng thời gian nhất định và lợi nhuận đơn giản trung bình trong cùng khoảng thời gian phụ thuộc vào phương sai của lợi nhuận cũng như lợi nhuận đơn giản trung bình kỳ vọng của chúng. Bằng chứng chính thức về tính chất này được trình bày trong Phụ lục A. Ngoài ra, phương sai của lợi nhuận hầu như không phụ thuộc vào việc sử dụng lợi nhuận logarit hay lợi nhuận đơn giản và bằng chứng về điều này cũng được đưa ra trong Phụ lục A. Mối quan hệ giữa phương sai và lợi nhuận được nêu rõ Tuy nhiên, trong đoạn này, cho phép suy ra phương pháp gần đúng để chuyển đổi giữa các giá trị được tính bằng cách sử dụng kết quả trả về logarit và những giá trị được tính bằng cách sử dụng trả về đơn giản và phương pháp dẫn xuất này được nêu trong Phụ lục A. Công thức cho phương pháp gần đúng này là:

xl = x s +  0.5*`lamda` ^2  (1)

xl = trung bình lợi nhuận logarith

xs = trung bình lợi nhuận đơn giản

`lamda`^2: phương sai mẫu của lợi nhuận đơn giản

iii) Cho rằng lợi nhuận logarit trung bình có liên quan đến cả giá trị trung bình và phương sai của lợi nhuận đơn giản, không thể có mối quan hệ 1-1 giữa lợi nhuận logarit trung bình và lợi nhuận đơn giản trung bình cho các hệ thống ngẫu nhiên. Lợi nhuận logarit trung bình cụ thể có thể là kết quả của nhiều sự kết hợp giữa giá trị trung bình và phương sai của lợi nhuận đơn giản. Phụ lục B minh họa tính chất này. *Ý nghĩa quan trọng của điều này là giá trị trung bình của lợi nhuận logarit của một phân phối cụ thể không thể được sử dụng để suy ra giá trị trung bình của lợi nhuận đơn giản của phân phối đó*. 

Các đặc tính của lợi nhuận logarit được trình bày từ i) đến iii) ở trên làm nảy sinh sự phức tạp về mặt khái niệm trong đó lý thuyết tài chính coi rủi ro6 và lợi nhuận là những khái niệm chỉ được liên kết với nhau do thực tế là trong một thị trường cạnh tranh, các nhà đầu tư chấp nhận một mức độ rủi ro cụ thể. được khen thưởng bằng một mức lợi nhuận thích hợp. Quan điểm này không gây khó khăn gì khi xem xét lợi nhuận đơn giản vì không có mối liên hệ toán học trực tiếp và tự động giữa rủi ro và lợi nhuận. Tuy nhiên, lợi nhuận logarit kỳ vọng của một chuỗi lợi nhuận phụ thuộc vào phương sai của chuỗi. Do đó, ở một mức độ nào đó, sự tạo tác toán học này của phương pháp được sử dụng để tính lợi nhuận logarit đã che khuất mối quan hệ giữa rủi ro và lợi nhuận. Phụ lục C đưa ra một ví dụ trong đó, trong một khoảng thời gian cụ thể, lợi nhuận đơn giản dự kiến cao hơn lợi nhuận logarit dự kiến do chênh lệch lợi nhuận cao.

**3 \. Kết luận**

Bài viết này chứng minh rằng việc so sánh các phương tiện được tính bằng logarit và lợi nhuận đơn giản trong tính toán tài chính đặt ra một số vấn đề đáng lo ngại. **Bằng chứng lý thuyết đã chứng minh rằng giá trị trung bình của một tập hợp lợi nhuận được tính bằng lợi nhuận logarit nhỏ hơn giá trị trung bình được tính bằng lợi nhuận đơn giản với một lượng liên quan đến phương sai của tập hợp lợi nhuận, trong đó phương sai tương đối bất biến cho dù nó được đo bằng logarit hay lợi nhuận đơn giản**. 

*Điều này ngụ ý rằng không có mối quan hệ một đối một giữa logarit trung bình và lợi nhuận đơn giản trung bình nên rất khó để đưa ra kết luận về tài sản cuối cùng kỳ vọng từ các nghiên cứu được thực hiện bằng cách sử dụng lợi nhuận logarit*. 

Ngoài ra, các phép tính về mối quan hệ giữa rủi ro và lợi nhuận được tính bằng lợi nhuận logarit sẽ khác một cách có hệ thống so với các phép tính được tính bằng lợi nhuận đơn giản. Thật vậy, khi sử dụng lợi nhuận logarit, ceteris paribus, phương sai cao hơn sẽ tự động làm giảm lợi nhuận kỳ vọng như một vấn đề của đại số cơ bản. Do đó, mối quan hệ giữa rủi ro và lợi nhuận trong bất kỳ tình huống tài chính nào đều phụ thuộc vào cách đo lường lợi nhuận. Các ví dụ thực nghiệm rút ra từ một số lĩnh vực thực hành học thuật xác nhận lý thuyết của chúng tôi. Họ cũng chỉ ra rằng tác động này có thể quan trọng trong các nghiên cứu thực tế với sự khác biệt đáng kể về mức độ lợi nhuận được tính toán có thể dễ dàng nhận thấy và cũng có những trường hợp mà ý nghĩa thống kê của kết quả thay đổi. Nói chung, đối với bất kỳ nghiên cứu thực nghiệm nào mà ý nghĩa thống kê thay đổi khá ít thì thước đo lợi nhuận có thể sẽ thay đổi ý nghĩa. *Tác động của việc thay đổi thước đo lợi nhuận có thể khá ấn tượng khi có liên quan đến dữ liệu trong ngày*. Rõ ràng lợi nhuận đang được xem xét trong bất kỳ bài tập nghiên cứu nào có thể được định nghĩa là lợi nhuận logarit hoặc lợi nhuận đơn giản và mỗi trong số này sẽ đưa ra một khuôn khổ logic nhất quán nội bộ để giải quyết vấn đề. *Tuy nhiên, trong bối cảnh điều tra về tài sản cuối cùng của các nhà đầu tư, có vẻ như rõ ràng rằng lãi suất đơn giản là thước đo thích hợp nhất để sử dụng*. 

Dựa trên những điều đã nói ở trên, có thể phù hợp trong các nghiên cứu về lợi nhuận để xem xét kỹ hơn liệu lợi nhuận trung bình được tính toán đơn giản hay lợi nhuận logarit. Tính toán lợi nhuận bằng cách sử dụng một trong hai hoặc cả hai phương pháp nói chung là một nhiệm vụ tầm thường đối với nghiên cứu trong tương lai trên các hệ thống máy tính hiện đại. Tuy nhiên, có rất nhiều tài liệu trong đó chỉ có một loại lợi nhuận được báo cáo và trong một số trường hợp, việc xem lại các kết luận mà không cần tham gia vào việc mở lại các tính toán cũ có thể là điều mong muốn và thuận tiện. Theo đó, chúng tôi đưa ra một phương pháp gần đúng để điều chỉnh phương tiện được tính toán bằng cách sử dụng lợi nhuận logarit để có thể rút ra kết luận có ý nghĩa về sự giàu có cuối cùng từ các nghiên cứu sử dụng những lợi nhuận này.
_Tóm lại, mặc dù mỗi phương pháp tính toán lợi nhuận đều có ưu điểm nhưng các phương pháp này có thể cho kết quả khác nhau một cách đáng ngạc nhiên. Cần phải nhận thức được điều này để không đưa ra những kết luận không phù hợp từ các nghiên cứu thực nghiệm_.

**4\. Số liệu**

|               | SP500<br>(1950 - 2009) | SP500<br>(1980 - 2009) | Dow Johns (1897-2009)<br>Daily return |
|---------------|:----------------------:|------------------------|---------------------------------------|
| Log Return    | 2.985700 <br>(2.62534) | 2.485555<br>(1.672631) | 0.00018<br>(0.00012)                  |
| Simple Return | 3.434317<br>(2.926564) | 2.958536<br>(2.018502) | 0.00024<br>(0.00012)                  |
|               |                        |                        |                                       |

***Tham khảo***

1. [On the use Log return in finance](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=1549328)