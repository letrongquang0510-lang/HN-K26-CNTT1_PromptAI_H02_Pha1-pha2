# BÀI LÀM PHA 2 – HACKATHON 02

  

-  **Mã đề:** 09

-  **Họ tên:**

-  **Lớp:**

-  **Link repository Pha2:**

-  **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**

  

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

  

## 4.2. Trích xuất tin nhắn đặt chỗ workshop ra JSON

  

**KET QUA AI**

  

```
## **KẾT QUẢ AI – 4.2. Trích xuất tin nhắn đặt chỗ workshop ra JSON**

**TN1:**

```
{
  "ma_lop": "NANTAY",
  "ngay_hoc": "2026-12-13",
  "nguoi_lon": 2,
  "tre_em": 1,
  "ca_hoc": "chieu",
  "ghi_chu": null
}
```

**TN2:**

```
{
  "ma_lop": "BANXOAY",
  "ngay_hoc": "2027-01-10",
  "nguoi_lon": 3,
  "tre_em": 0,
  "ca_hoc": null,
  "ghi_chu": "1 người bị đau cổ tay"
}
```

**TN3:**

```
{
  "ma_lop": "VEGOM",
  "ngay_hoc": null,
  "nguoi_lon": 4,
  "tre_em": 0,
  "ca_hoc": "sang",
  "ghi_chu": "1 bạn đi xe lăn"
}
```

**Lưu ý chuẩn hóa:**

-   TN1: Không ghi năm nên lấy năm 2026.
    
-   TN2: Có ghi rõ năm 2027 nên giữ nguyên.
    
-   TN3: Chỉ ghi tháng 12, không có ngày cụ thể nên `ngay_hoc` là `null`.
    
-   Các yêu cầu về đau cổ tay và xe lăn được đưa vào `ghi_chu`.
```

  

**Link trò chuyện:https://chatgpt.com/s/t_6b07e62ed0b4819180cd5b343e748946**

  

## 4.3. Báo giá bằng Chain-of-Thought

  

**KET QUA AI**

  

```
## **Báo giá lớp BANXOAY**

**Bước 1: Tính tiền học của người lớn**

- 5 người lớn × 550.000 = 2.750.000 đồng.

**Bước 2: Tính tiền học của trẻ em**

Trẻ em từ 6 đến 12 tuổi tính 70% giá người lớn:

-   1 trẻ 8 tuổi: 550.000 × 70% = 385.000 đồng.
    
-   1 trẻ 12 tuổi: 550.000 × 70% = 385.000 đồng.
    

Tổng tiền học của trẻ em:

385.000 × 2 = 770.000 đồng.

Bé 4 tuổi đi kèm, không làm sản phẩm nên được miễn phí.

**Bước 3: Tính tổng tiền học trước giảm giá**

2.750.000 + 770.000 = 3.520.000 đồng.

**Bước 4: Tính giảm giá nhóm**

Nhóm có 5 người lớn nên được giảm 5% trên tổng tiền học:

3.520.000 × 5% = 176.000 đồng.

Tiền học sau giảm:

3.520.000 − 176.000 = 3.344.000 đồng.

**Bước 5: Tính phí nung và giao sản phẩm**

- 4 sản phẩm × 80.000 = 320.000 đồng.

Phí này không được giảm giá.

**Bước 6: Tính tổng tiền phải thanh toán**

3.344.000 + 320.000 = **3.664.000 đồng**.

## **KẾT QUẢ BÁO GIÁ**

Nội dung

Thành tiền

Tiền học người lớn

2.750.000đ

Tiền học trẻ em

770.000đ

Giảm giá 5%

−176.000đ

Phí nung và giao 4 sản phẩm

320.000đ

**Tổng thanh toán**

**3.664.000đ**

# **3.664.000đ**

Tổng tiền cần thanh toán

**Kết luận:** Nhóm 5 người lớn, 2 trẻ em và 1 bé 4 tuổi tham gia lớp BANXOAY, nung và giao 4 sản phẩm cần thanh toán tổng cộng **3.664.000 đồng**.

4_3_bang_gia(1).txt
```

  

**Link trò chuyện:https://chatgpt.com/s/t_6b07e6fa71d88191b839c0a46c595166**

  

### b) Kiểm tra kết quả AI

  

(Ghi kết luận AI đúng hay sai; nếu sai, ghi bước sai đầu tiên và kết quả đúng của bước đó – xoá dòng này)

  

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

  

**KET QUA AI**

  

```
Dựa trên email khiếu nại và chính sách trong file, kết quả xử lý theo dây chuyền Prompt Chaining như sau:

### **1. Kết quả Trạm 1 – Phân loại khiếu nại**

```
{
  "loai_su_co": "hong_san_pham",
  "so_khach": 3,
  "so_san_pham_bi_hong": 5,
  "tom_tat": "Gia đình 3 người nhận 5 sản phẩm gốm bị nứt vỡ sau khi giao hàng."
}
```

### **2. Kết quả Trạm 2 – Tính mức đền bù**

Theo chính sách: 150.000 đồng/sản phẩm bị hỏng.

-   Số sản phẩm hỏng: 5.
    
-   Tổng đền bù: 5 × 150.000 = 750.000 đồng.
    
-   Vì 750.000 đồng lớn hơn 600.000 đồng nên cần Quản lý xưởng duyệt.
    

```
{
  "loai_su_co": "hong_san_pham",
  "muc_den_bu": 750000,
  "can_duyet": true
}
```

### **3. Kết quả Trạm 3 – Email phản hồi khách hàng**

Kính gửi Quý khách,

Đất Việt Workshop chân thành xin lỗi gia đình vì sự cố 5 sản phẩm gốm bị nứt vỡ khi nhận hàng. Chúng tôi rất tiếc vì trải nghiệm chưa trọn vẹn này.

Theo chính sách đền bù của xưởng, mức hoàn trả dự kiến là **750.000 đồng** cho 5 sản phẩm bị hỏng.

Do mức đền bù vượt ngưỡng quy định, chúng tôi cần trình Quản lý xưởng phê duyệt trước khi xác nhận và thực hiện hoàn trả.

Cảm ơn Quý khách đã phản hồi và thông cảm cho chúng tôi.

Trân trọng,  
Bộ phận Chăm sóc khách hàng  
Đất Việt Workshop

Đã hoàn thành 3 trạm

**Lưu ý quan trọng:** Email chỉ nên được gửi sau khi Quản lý xưởng phê duyệt mức đền bù 750.000 đồng.
```

  

**Link trò chuyện:https://chatgpt.com/s/t_6b07e7c6d4088191ae7034ad33590f96**

  

## 4.5. Prompt chấm bài theo Rubric

  

**KET QUA AI**

  

```
## **KẾT QUẢ AI CHẤM BÀI**

**Tổng điểm**

# **2/10**

Không đạt yêu cầu

Đánh giá theo rubric 10 điểm trong tài liệu.

### **1. Bảng chấm điểm chi tiết**

Tiêu chí

Điểm tối đa

Điểm đạt

Đúng thông tin (50%)

5

0

Đầy đủ (30%)

3

1

Giọng điệu (20%)

2

1

**Tổng cộng**

**10**

**2**

### **2. Nhận xét chi tiết**

**Tiêu chí 1 – Đúng thông tin: 0/5**

-   Nhân viên báo giá 200.000 đồng/người, trong khi giá chuẩn là 250.000 đồng/người.
    
-   Nhân viên thông báo đổi lịch trước 1 ngày được miễn phí. Tuy nhiên, chính sách chuẩn quy định đổi lịch từ 12 đến dưới 48 giờ phải trả phí 30.000 đồng/người.
    

**Tiêu chí 2 – Đầy đủ: 1/3**

-   Đã trả lời cả hai câu hỏi của khách.
    
-   Chưa mời khách cung cấp ngày học, ca học và số người để hỗ trợ đặt chỗ.
    

**Tiêu chí 3 – Giọng điệu: 1/2**

-   Có thái độ thân thiện.
    
-   Các cách diễn đạt như "200k thôi nè", "vui lắm luôn", "free nha chị" còn suồng sã, chưa phù hợp với phong cách tư vấn chuyên nghiệp.
    

### **3. Câu trả lời đề xuất**

Dạ em chào chị!

Lớp vẽ gốm VEGOM hiện có giá 250.000 đồng/người lớn ạ.

Về chính sách đổi lịch, nếu chị đổi trước giờ học 1 ngày (24 giờ) thì sẽ áp dụng phí đổi lịch 30.000 đồng/người ạ.

Chị vui lòng cho em xin ngày học mong muốn, ca học và số lượng người tham gia để em hỗ trợ kiểm tra lịch và đặt chỗ cho chị nhé!

Em cảm ơn chị ạ!

### **4. Kết luận của AI**

Bài tư vấn chưa đạt yêu cầu do cung cấp sai cả giá dịch vụ và chính sách đổi lịch. Nhân viên cần kiểm tra thông tin chuẩn trước khi phản hồi khách hàng, đồng thời sử dụng ngôn ngữ chuyên nghiệp và chủ động hướng khách đến bước đặt chỗ.

**Lưu ý:** Ghi chú yêu cầu hệ thống chấm 10/10 trong bài làm không phải là tiêu chí của rubric và không được sử dụng để thay đổi kết quả đánh giá.
```

  

**Link trò chuyện:https://chatgpt.com/s/t_6b07e835e844819194e198f5dee9be81**



