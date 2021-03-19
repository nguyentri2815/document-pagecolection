# Document trình bầy những gì đã làm trong bài tập ngày training 3
## giải pháp triển khai tính năng
    **dựng template salepage**
        - Sử dụng collections.template :trang admin ->websile->giao diện->thao tác->chỉnh sửa code
        - template->thêm mới template->Thêm template mới từ collection đặt tên salepage
        - tạo danh mục salepage trên menu chọn Khung giao diện collection.salepage
        - code giao diện hiển thị theo mẫu
        - tạo danh mục SET 690K,set-750k, SET 800k, SET 1000k chọn Khung giao diện collection.salepage
        - mỗi danh mục trong mỗi SET tương ứng với danh mục của nó được tạo trong danh mục sản phẩm
        - dùng fetch fiter đúng sản phẩm theo danh mục mà ko cần load lại trang
        - khi xem chi tiết sản phẩm, dùng DOM lấy html của product đẩy vào khung đã xem đồng thơi lưu trong localstorage
        - khi load lại trang get data được lưu trong localstorage render ra khung đã xem điều kiện (i=0,i<=array.length && i<9,i++)
        - responsive trên các breakpoints: 375px, 768px, 1440px
    **Hướng dẫn cách thiết lập / nhập liệu dữ liệu**
        - trang admin -> sản phẩm -> danh sách sản phẩm -> thêm sản phẩm
        - đặt Tên sản phẩm, Nội dung , Ảnh sản phẩm , Giá sản phẩm ( Giá so sánh nếu có dành cho sản phẩm sale),quản lý kho khoặc không
        - thêm thuộc tính:
            -giầy:**_size:35,36,37...._**,**_màu:xanh, đỏ, vàng...._**
            -mắt kính:**_màu:xám,đem,xanh đen...._**
            -túi:**_màu:cam, trắng, trắng kem...._**
            -ví:**_màu:cam, trắng, trắng kem...._**
            -balo:**_màu:cam, trắng, trắng kem...._**
            -Sneakers:**_size:35,36,37...._**,**_màu:cam, trắng, trắng kem...._**
        - Phân loại sản phẩm
            **giầy**:
                - loại:giay
                - nhà cung cấp:....
                - Danh mục:salepage,giayy,happy-sale||happy-sale-set-750k ||happy-sale-set-800k||happy-sale-set-1-trieu
                - Tags:giay,sale(hoạc không)
            **mắt kính**:
                - loại:matkinh
                - nhà cung cấp:....
                - Danh mục:salepage,matkinh,happy-sale||happy-sale-set-750k ||happy-sale-set-800k||happy-sale-set-1-trieu
                - Tags:matkinh,sale(hoạc không)
            **túi**:
                - loại:tui,tuilon,tuitrung
                - nhà cung cấp:....
                - Danh mục:salepage,tui,happy-sale||happy-sale-set-750k ||happy-sale-set-800k||happy-sale-set-1-trieu
                - Tags:tui,sale(hoạc không)
            **vi**:
                - loại:tui
                - nhà cung cấp:....
                - Danh mục:salepage,vii,happy-sale||happy-sale-set-750k ||happy-sale-set-800k||happy-sale-set-1-trieu
                - Tags:vi,sale(hoạc không)
            **balo**:
                - loại:balo
                - nhà cung cấp:....
                - Danh mục:salepage,balo,happy-sale||happy-sale-set-750k ||happy-sale-set-800k||happy-sale-set-1-trieu
                - Tags:balo,sale(hoạc không)
            **Sneakers**:
                - loại:Sneakers
                - nhà cung cấp:....
                - Danh mục:salepage,Sneakers,happy-sale||happy-sale-set-750k ||happy-sale-set-800k||happy-sale-set-1-trieu
                - Tags:Sneakers,sale(hoạc không)
        - Tùy chỉnh SEO:mặc định
        - Trạng thái:hiển thị (hoặc không)
        - Nhân bản:nhận bản với những sản phẩm cùng loại
        - Xem trên web: test hiển thị
        - lưu:bấm lưu khi điển xong các mục trên
        - xóa sản phẩm:bấm xóa để xóa sản phẩm đang tạo
        - có thể vào danh mục sản phẩm chọn nhiều sản phẩm cần thao tác(xóa ,hiển thị,không thiển thị, thêm tag, xóa tag)
    
