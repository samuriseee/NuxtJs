# NuxtJs
I) Khái niệm cơ bản về Server Side Rendering và Client Side Rendering a.k.a SPA 
   1) Server Side Rendering: 
      Khái niệm: 
            - Bất cứ khi nào Client truy cập vào website thì browser sẽ gửi request lên server 
            - Web server sẽ đáp lại request và render ra HTML, load Js, và sau đó mới bắt đầu load các framework (React,Vue,Angular,...)
            - Sau các giai đoạn thì web có thể viewable
                 
      Ưu điểm: 
            + Thân thiện với SEO, bot của Google có thể cào được các content có trong website => điểm của SEO sẽ cao hơn 
            + Bảo mật của Website sẽ cao hơn, người dùng khó có thể truy cập được dữ liệu API chúng ta dưới dạng .json
            + Chạy được khi trình duyện disable JavaScript.
      
      Nhược điểm:
            - Khi mà user route qua trang khác, browser sẽ gửi lại request lên server để render ra trang đích,
            - Khi load lại những chỗ không cần thiết/không thay đổi, làm tăng tốc độ load của website
            - Có nhiều luồng truy cập vào thì sẽ làm nghẽn cổ chai
            - Giảm trải nghiệm của người dùng khá là nhiều
     
   2) Client Side Rendering a.k.a SPA: 
      Khái niệm: 
            - Khác với Server Side phải render HTML ra từ server thì Client Side ra sẽ render ra từ browser
            - Website có thể viewable từ ngay lúc này, sau đó browser mới bắt đầu load Js, framework

      Ưu điểm: 
            + Khi route qua trang khác, chỉ load những component cần thiết/có thay đổi
            + Tốc độ load sẽ nhanh hơn
            + Làm tăng trải nghiệm người dùng
            + Hạn chế truy cập tới Server
            + Tạo công ăn việc làm cho Frontend
         
      Nhược điểm: 
            - Vì phải để browser render nên phải mất 1 ít thời gian khi truy cập vào URL của website thì mới render ra content được 
            - Bot của Google lại đọc ngay ở khúc nhập URL của trang web nên là sẽ không đọc được content
            - Vậy nên SPA không hề thân thiện với SEO 
            - Phải fetch API liên tục nên trang web dễ bị tuồn data ra ngoài
            - Trình duyệt mà không bật JavaScript là toang.
      
      
