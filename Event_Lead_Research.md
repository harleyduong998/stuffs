## 3. Business Use Cases

### 3.1 Order Events — Use Cases


| Event                      | Mục tiêu kinh doanh           | Hành động chăm sóc                                   | Độ ưu tiên     | Giá trị kỳ vọng                      |
| -------------------------- | ----------------------------- | ---------------------------------------------------- | -------------- | ------------------------------------ |
| order.completed            | Tăng repeat rate, cross-sell  | Gọi cảm ơn trong 24h, gợi ý sản phẩm liên quan       | **Cao**        | +15-20% repeat order trong 30 ngày   |
| order.rejected_by_customer | Giảm tỷ lệ hủy, recovery      | Gọi trong vòng 2h, tìm hiểu lý do, đề xuất giải pháp | **Rất cao**    | Recovery 30-40% đơn bị từ chối       |
| order.delivery_failed      | Giảm hủy đơn do logistics     | Gọi ngay trong 1h, xác nhận lại thông tin giao hàng  | **Rất cao**    | Giảm 50% tỷ lệ hủy sau giao thất bại |
| order.high_value           | Tăng LTV khách VIP            | Chăm sóc VIP: gọi xác nhận, tặng quà, ưu tiên giao   | **Cao**        | +25% retention khách VIP             |
| order.repeat_product       | Tăng giá trị đơn trung bình   | Đề xuất gói mua sỉ, subscription                     | **Trung bình** | +10-15% AOV                          |
| order.dormant_customer     | Win-back, giảm churn          | Gọi hỏi thăm, gửi coupon win-back cá nhân hóa        | **Cao**        | Recovery 10-15% khách dormant        |
| order.first_purchase       | Onboarding, tạo thói quen mua | Welcome call, hướng dẫn, mời loyalty                 | **Cao**        | +30% probability mua lần 2           |


### 3.2 Loyalty Events — Use Cases


| Event                          | Mục tiêu kinh doanh                      | Hành động chăm sóc                         | Độ ưu tiên     | Giá trị kỳ vọng                        |
| ------------------------------ | ---------------------------------------- | ------------------------------------------ | -------------- | -------------------------------------- |
| loyalty.tier_upgraded          | Kích hoạt quyền lợi mới, tăng engagement | Gọi chúc mừng, giới thiệu ưu đãi hạng mới  | **Cao**        | +20% spending trong tháng đầu hạng mới |
| loyalty.points_expiring        | Kích hoạt sử dụng điểm, tạo giao dịch    | Nhắc trước 7 ngày và 3 ngày, gợi ý quà đổi | **Rất cao**    | Recovery 25-35% điểm sắp hết hạn       |
| loyalty.low_engagement         | Tái kích hoạt, giảm churn loyalty        | Gọi giới thiệu lại, gợi ý quà dễ đổi       | **Trung bình** | +15% reactivation rate                 |
| loyalty.tier_downgrade_warning | Giữ hạng, kích thích mua thêm            | Nhắc "chỉ cần mua thêm X để giữ hạng"      | **Cao**        | 40% khách sẽ mua thêm để giữ hạng      |


### 3.3 Coupon Events — Use Cases


| Event                    | Mục tiêu kinh doanh             | Hành động chăm sóc                               | Độ ưu tiên     | Giá trị kỳ vọng                |
| ------------------------ | ------------------------------- | ------------------------------------------------ | -------------- | ------------------------------ |
| coupon.viewed + not_used | Chuyển đổi intent → mua         | Nhắc sau 4-6h, gợi ý sản phẩm phù hợp với coupon | **Cao**        | +20% conversion coupon         |
| coupon.expiring_soon     | Tạo urgency, recovery coupon    | Gọi/nhắn "coupon sắp hết hạn trong 24h"          | **Rất cao**    | +30% redemption rate           |
| coupon.expired_unused    | Win-back, hiểu lý do không dùng | Gọi hỏi, cân nhắc gia hạn hoặc tạo coupon mới    | **Trung bình** | Recovery 10-15% qua coupon mới |
| coupon.almost_qualified  | Tăng AOV, push cross-sell       | Nhắc "mua thêm 50k để được giảm 100k"            | **Cao**        | +25% conversion, +15% AOV      |


### 3.4 Livechat Events — Use Cases


| Event                           | Mục tiêu kinh doanh      | Hành động chăm sóc                             | Độ ưu tiên   | Giá trị kỳ vọng                  |
| ------------------------------- | ------------------------ | ---------------------------------------------- | ------------ | -------------------------------- |
| livechat.inquiry_no_purchase    | Chuyển đổi lead          | Telesales gọi trong 30 phút, giải đáp thắc mắc | **Rất cao**  | +35% conversion từ chat → mua    |
| livechat.price_inquiry          | Close deal, upsell       | Gửi báo giá chính thức, gọi tư vấn             | **Rất cao**  | +40% close rate khi gọi trong 1h |
| livechat.negative_sentiment     | Giảm churn, bảo vệ brand | Escalate CSKH senior, gọi xin lỗi ngay         | **Khẩn cấp** | Giảm 60% negative review         |
| livechat.abandoned_conversation | Recovery lead            | Follow-up trong 2h qua kênh khác               | **Cao**      | Recovery 20-25%                  |


### 3.5 Product Interest Events — Use Cases


| Event                           | Mục tiêu kinh doanh             | Hành động chăm sóc                                  | Độ ưu tiên  | Giá trị kỳ vọng                  |
| ------------------------------- | ------------------------------- | --------------------------------------------------- | ----------- | -------------------------------- |
| product.added_to_cart_abandoned | Recovery abandoned cart         | Nhắc sau 1h, gửi incentive nhỏ nếu chưa mua sau 24h | **Rất cao** | +15-25% cart recovery            |
| product.viewed_multiple_times   | Chuyển đổi interest → mua       | Telesales tư vấn, gửi thông tin chi tiết            | **Cao**     | +20% conversion                  |
| product.high_value_viewed       | Tăng doanh thu sản phẩm premium | Tư vấn VIP, đề xuất trả góp, demo                   | **Cao**     | +10% conversion sản phẩm premium |
| product.campaign_interest       | Tối ưu hiệu quả campaign        | Ưu tiên telesales, gửi thông tin campaign chi tiết  | **Cao**     | +30% campaign conversion         |


---

## 4. UI Context Research

### 4.1 Order Event — Context UI

Khi telesales/CSKH mở một lead từ Order event, UI cần hiển thị:

**Block 1: Event Summary (Header)**

- Loại event (VD: "Đơn giao thất bại")
- Thời gian xảy ra
- Urgency indicator (badge màu: đỏ/cam/vàng)
- Trạng thái xử lý (chưa xử lý / đang xử lý / đã xử lý)

**Block 2: Current Order Detail**

- Mã đơn, trạng thái đơn
- Danh sách sản phẩm trong đơn (tên, số lượng, giá)
- Tổng giá trị đơn
  ---
- Phương thức thanh toán, trạng thái thanh toán
- Thông tin giao hàng (địa chỉ, đơn vị vận chuyển, trạng thái)
- Ghi chú đơn hàng (nếu có)

**Block 3: Customer Summary**

- Tên, SDT, email
- Segment / hạng thành viên
- Tổng số đơn đã mua, tổng giá trị vòng đời (LTV)
- Đơn gần nhất trước đó
- Điểm loyalty hiện tại
- Ghi chú nội bộ về khách

**Block 4: Order History**

- 5-10 đơn gần nhất (mã đơn, ngày, giá trị, trạng thái)
- Tỷ lệ đơn thành công vs thất bại
- Sản phẩm mua nhiều nhất
- Tần suất mua (trung bình bao lâu mua 1 lần)

**Block 5: Recommended Actions**

- Gợi ý script gọi điện theo loại event
- Sản phẩm cross-sell/upsell gợi ý (dựa trên lịch sử mua)
- Coupon có thể áp dụng cho khách
- CTA chính: "Gọi điện", "Gửi SMS", "Tạo ticket"

### 4.2 Loyalty Event — Context UI

**Block 1: Event Summary**

- Loại event loyalty (VD: "Điểm sắp hết hạn")
- Deadline (ngày hết hạn điểm / ngày xét hạng)
- Urgency indicator

**Block 2: Loyalty Status**

- Hạng hiện tại, tiến trình đến hạng tiếp theo (progress bar)
- Tổng điểm, điểm khả dụng, điểm sắp hết hạn
- Lịch sử nâng/hạ hạng
- Quyền lợi hiện tại theo hạng

**Block 3: Points Timeline**

- Timeline tích/tiêu điểm (dạng chart hoặc list)
- Điểm sắp hết hạn theo từng đợt (ngày hết hạn, số điểm)
- Lịch sử đổi quà

**Block 4: Customer Summary** (tương tự Order)

**Block 5: Recommended Actions**

- Gợi ý quà có thể đổi với số điểm hiện tại
- Sản phẩm giúp khách đạt ngưỡng nâng hạng
- Script tư vấn theo event
- CTA: "Gọi điện", "Gửi nhắc điểm", "Tạo coupon"

### 4.3 Coupon Event — Context UI

**Block 1: Event Summary**

- Loại event coupon (VD: "Coupon sắp hết hạn")
- Countdown (còn bao lâu hết hạn)
- Urgency indicator

**Block 2: Coupon Detail**

- Mã coupon, loại giảm giá (%, tiền, freeship)
- Điều kiện sử dụng (đơn tối thiểu, danh mục áp dụng)
- Ngày bắt đầu — ngày kết thúc
- Trạng thái: đã gán / đã xem / đã dùng / hết hạn

**Block 3: Coupon Lifecycle Timeline**

- Timeline: gán → gửi thông báo → khách xem → (chưa dùng / đã dùng)
- Các lần nhắc đã gửi
- Hành vi tương tác của khách với coupon (mở email, click link, v.v.)

**Block 4: Customer Summary** + lịch sử sử dụng coupon trước đó

**Block 5: Recommended Actions**

- Gợi ý sản phẩm phù hợp với điều kiện coupon
- Khả năng recovery (cao/trung bình/thấp) dựa trên hành vi
- Script gọi điện
- CTA: "Gọi nhắc coupon", "Gia hạn coupon", "Tạo coupon mới"

### 4.4 Livechat Event — Context UI

**Block 1: Event Summary**

- Loại event (VD: "Khách chat hỏi giá nhưng chưa mua")
- Sentiment score (nếu có AI phân tích)
- Thời gian cuộc chat, thời gian kết thúc

**Block 2: Conversation Summary**

- Nội dung tóm tắt cuộc chat (AI-generated hoặc excerpt)
- Sản phẩm được nhắc đến trong chat
- Câu hỏi chính của khách
- Sentiment highlights (câu tích cực / tiêu cực nổi bật)

**Block 3: Full Conversation** (collapsible)

- Toàn bộ nội dung chat, có thể scroll
- Highlight các đoạn quan trọng (giá, khiếu nại, yêu cầu)

**Block 4: Customer Summary** + lịch sử chat trước đó

**Block 5: Recommended Actions**

- Gợi ý phản hồi dựa trên nội dung chat
- Sản phẩm liên quan đến cuộc hội thoại
- Script theo loại sentiment
- CTA: "Gọi điện", "Gửi thông tin sản phẩm", "Tạo ticket hỗ trợ"

### 4.5 Product Interest Event — Context UI

**Block 1: Event Summary**

- Loại event (VD: "Xem sản phẩm 5 lần trong 3 ngày")
- Intent score (tính toán từ tần suất + thời gian xem)
- Sản phẩm chính đang quan tâm

**Block 2: Product Detail**

- Tên, hình ảnh, giá, trạng thái tồn kho
- Mô tả ngắn, category
- Rating, số lượng đã bán
- Các chương trình khuyến mãi đang áp dụng

**Block 3: Browsing Behavior**

- Timeline xem sản phẩm (ngày giờ, thiết bị, thời gian xem)
- Các sản phẩm khác đã xem trong cùng session
- Giỏ hàng hiện tại (nếu có)
- So sánh sản phẩm (nếu khách đã so sánh)

**Block 4: Customer Summary** + lịch sử mua sản phẩm cùng danh mục

**Block 5: Recommended Actions**

- Sản phẩm tương tự hoặc bổ sung
- Coupon có thể áp dụng cho sản phẩm này
- Script tư vấn theo mức giá và hành vi
- CTA: "Gọi tư vấn", "Gửi thông tin sản phẩm", "Tạo coupon cá nhân"

---

