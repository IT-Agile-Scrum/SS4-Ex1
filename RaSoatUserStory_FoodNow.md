# Bài Tập: Rà Soát User Story và Sắp Xếp Product Backlog (FoodNow)

## Bước 1. Tìm lỗi theo tiêu chí INVEST

| Mã | Kết quả và lý do |
| :--- | :--- |
| **US1** | **Đạt:** Vai trò rõ, một việc, có lợi ích, thử được bằng cách chọn loại món rồi xem kết quả. |
| **US2** | **Sai chữ T (Testable - Không thể kiểm thử):** Các từ mô tả như "đẹp" và "dễ dùng" mang tính chủ quan, cảm tính. Nhóm sẽ không có tiêu chí nghiệm thu rõ ràng để đo lường xem thế nào là đạt yêu cầu và khi nào thì được tính là "xong". |
| **US3** | **Sai chữ V (Valuable - Thiếu giá trị thực tiễn cho khách hàng):** Việc dùng React chỉ là giải pháp công nghệ nội bộ. Dù Backlog có chứa việc kỹ thuật, việc này cần chỉ ra được giá trị hoặc tác động cuối cùng mang lại cho sản phẩm/người dùng (ví dụ: để ứng dụng tải nhanh hơn 20%, giúp khách không bị bực mình khi chờ). |
| **US4** | **Sai chữ S (Small - Quá lớn):** Story này quá ôm đồm, chứa khối lượng công việc của cả một hệ thống lớn (nhiều bộ lọc thời gian, bộ lọc khu vực, xuất Excel, và cả hệ thống tự động gửi email). Khối lượng này không thể hoàn thành gọn gàng trong một Sprint. |

## Bước 2. Sửa lỗi

**a) Viết lại US2 (đưa ra tiêu chí đo được):**
- **US2 mới:** "Là một khách hàng, tôi muốn quy trình từ lúc chọn món đến lúc hoàn tất thanh toán chỉ gói gọn trong tối đa 3 thao tác chạm (click), để việc đặt món diễn ra nhanh chóng và thuận tiện." 
*(Tiêu chí "tối đa 3 thao tác chạm" hoàn toàn có thể đo lường và nghiệm thu thực tế).*

**b) Tách US4 và đặt vào cấu trúc 3 cấp:**
- **Epic:** Quản trị và Phân tích Dữ liệu Kinh doanh.
  - **Feature:** Báo cáo doanh thu cơ bản.
    - **User Story 4.1:** Là một admin, tôi muốn xem biểu đồ doanh thu tổng hợp theo ngày và tuần, để đánh giá nhanh tình hình kinh doanh hiện tại.
    - **User Story 4.2:** Là một admin, tôi muốn có nút "Xuất Excel" trên màn hình báo cáo doanh thu, để tải dữ liệu về máy lưu trữ và tổng hợp gửi cho ban giám đốc.

## Bước 3. Xếp lại Backlog

**a) Xếp thứ tự ưu tiên trong Product Backlog (từ cao xuống thấp):**
1. **US1:** Lọc nhà hàng theo loại món *(Ưu tiên cao nhất vì đây là tính năng cốt lõi giúp khách nhanh chóng tìm được đồ ăn, trực tiếp tạo ra đơn hàng).*
2. **US2 (đã sửa):** Rút gọn quy trình đặt món xuống 3 chạm *(Giúp cải thiện trải nghiệm và tăng tỷ lệ chuyển đổi đơn hàng, tạo doanh thu thực tế).*
3. **US 4.1:** Xem báo cáo doanh thu theo ngày/tuần *(Nhu cầu theo dõi quản trị cơ bản, quan trọng đối với việc vận hành hệ thống).*
4. **US 4.2:** Xuất Excel báo cáo *(Tính năng tiện ích bổ sung, admin tạm thời có thể tự xem số liệu trên màn hình để báo cáo nên có mức ưu tiên thấp nhất).*

**b) Ứng dụng DEEP cho Story đứng đầu (US1):**
- **Mức độ chi tiết:** Theo chữ **D (Detailed appropriately)**, US1 đang ở đầu Backlog nên cần được làm rõ với mức độ chi tiết cao nhất. Nó phải được trang bị đầy đủ các Acceptance Criteria (Tiêu chí nghiệm thu) cụ thể để định nghĩa sự hoàn thành (Ví dụ: danh sách các loại món, hành vi khi ấn bỏ lọc, v.v.).
- **Việc cần làm trong buổi Refinement:** Trước khi đưa vào Sprint, Product Owner và Development Team phải cùng nhau thảo luận để làm rõ mọi thắc mắc về US1, bổ sung đủ tiêu chí nghiệm thu, làm rõ rủi ro kỹ thuật, và tiến hành **ước lượng (Estimate - chữ E trong DEEP)** khối lượng công việc (ví dụ bằng Story Point) để team biết chắc chắn có thể làm xong trong Sprint hay không.
