# Ansible Information

Đây là trang giới thiệu về Ansible cũng như các code mẫu của mình.
----

Ansible là một công cụ quản lý, triển khai và điều phối cấu hình CNTT mã nguồn mở. Nó nhằm mục đích cung cấp mức tăng năng suất lớn trước nhiều thách thức tự động hóa. Công cụ này rất đơn giản để sử dụng nhưng đủ mạnh để tự động hóa các môi trường ứng dụng CNTT nhiều tầng phức tạp.

1) Vậy tại sao chúng ta lại cần Ansible??
Trước đây, các quản trị viên hệ thống quản lý các máy chủ bằng tay, cài đặt phần mềm, thay đổi cấu hình và quản trị các dịch vụ trên các máy chủ riêng lẻ.

Khi các trung tâm dữ liệu phát triển và các ứng dụng được lưu trữ trở nên phức tạp hơn, các quản trị viên nhận ra rằng họ không thể mở rộng quy mô quản lý hệ thống thủ công của mình nhanh như các ứng dụng. Nó cũng cản trở tốc độ công việc của các nhà phát triển vì nhóm phát triển nhanh chóng và thường xuyên phát hành phần mềm, nhưng các hoạt động CNTT đang dành nhiều thời gian hơn cho việc cấu hình hệ thống. Đó là lý do tại sao các công cụ quản lý cấu hình và cung cấp máy chủ trở nên phát triển mạnh mẽ.

Hãy xem xét công việc quản trị một đội máy chủ thường xuyên tẻ nhạt. Chúng ta luôn cần cập nhật, đẩy các thay đổi, sao chép các tệp tin trên chúng, v.v. Những tác vụ này khiến mọi thứ trở nên rất phức tạp và tốn thời gian. Nhưng không cần quá lo lắng về điều đó vì chúng ta đã có giải pháp. Giải pháp đó chính là - Ansible. Nhưng trước khi hiểu nhiều hơn về Ansible, chúng ta hãy làm quen với một số thuật ngữ Ansible như:

Controller Machine: Nơi Ansible được cài đặt, chịu trách nhiệm chạy cấp phép trên các máy chủ mà bạn đang quản lý.
Inventory: Tệp khởi tạo chứa thông tin về các máy chủ (hosts) mà bạn đang quản lý.
Playbook: Điểm đầu vào để cung cấp cho Ansible, nơi tự động hóa được xác định thông qua các tác vụ sử dụng định dạng YAML.
Task: Một khối xác định một thủ tục sẽ được thực thi. Ví dụ: Cài đặt một package
Module: Một mô-đun thường tóm tắt một nhiệm vụ hệ thống, như xử lý các gói hoặc tạo và thay đổi tệp. Ansible có vô số mô-đun tích hợp, nhưng bạn cũng có thể tạo những mô-đun tùy chỉnh.
Role: Một cách được xác định trước để tổ chức playbook và các tệp khác nhằm tạo điều kiện chia sẻ và sử dụng lại các phần của cấp phép.
Play: Một cung cấp được thực hiện để thực thi các Task.
Facts: Các biến toàn cục chứa thông tin về hệ thống, như giao diện mạng hoặc hệ điều hành.
Handlers: Được sử dụng để kích hoạt các thay đổi trạng thái dịch vụ, chẳng hạn như khởi động lại hoặc dừng một dịch vụ.
Ansible là một công cụ hữu ích cho phép bạn tạo các nhóm máy, mô tả cách cấu hình các máy này hoặc những hành động nên thực hiện trên chúng. Ansible đưa ra tất cả các lệnh từ một vị trí trung tâm để thực hiện các tác vụ này.

Không có phần mềm máy khách nào khác được cài đặt trên các node (nút). Nó sử dụng SSH để kết nối với các node. Ansible chỉ cần được cài đặt trên máy điều khiển (máy mà bạn sẽ chạy lệnh), thậm chí có thể là máy tính xách tay của bạn. Nó là một giải pháp đơn giản cho một vấn đề phức tạp.

2) Ưu điểm của việc sử dụng Ansible
- Đơn giản hóa nghiệp vụ (Simple)
- Không cần tác nhân hỗ trợ (Agentless)
- Mạnh mẽ & Linh hoạt (Powerful & Flexible)
- Hiệu quả (Efficient)