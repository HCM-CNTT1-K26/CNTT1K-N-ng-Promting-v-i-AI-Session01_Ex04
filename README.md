# CNTT1K-N-ng-Promting-v-i-AI-Session01_Ex04
## Phần 1: Phân tích so sánh mô hình AI

Bảng dưới đây tóm tắt các thế mạnh vượt trội của 3 mô hình hàng đầu hiện nay dựa trên các yêu cầu kỹ thuật thực tế:

| Tiêu chí so sánh | OpenAI GPT-4o | Anthropic Claude 3.5 Sonnet | Google Gemini 1.5 Pro |
| --- | --- | --- | --- |
| **Thế mạnh cốt lõi** | Tốc độ xử lý nhanh, tích hợp hệ sinh thái công cụ đa dạng và khả năng tương tác thời gian thực xuất sắc. | Khả năng lập luận logic cực sâu, văn phong tự nhiên, tinh tế và lập trình/xử lý văn bản thông minh (Artifacts). | Cửa sổ ngữ cảnh siêu lớn (Super Large Context Window) và khả năng xử lý đa phương thức nguyên bản (Native Multimodal). |
| **Xử lý Dữ liệu & Code (Code Interpreter)** | **Xuất sắc:** Môi trường Sandbox mạnh mẽ, xử lý mượt mà các tập dữ liệu lớn bằng Python, vẽ biểu đồ trực quan chính xác. | **Tốt:** Lập trình tốt nhưng tối ưu hơn cho việc phân tích cú pháp, logic mã nguồn và cấu trúc tài liệu văn bản. | **Tốt:** Hỗ trợ thực thi mã (Code Execution) nhưng thế mạnh thực sự nằm ở việc nạp toàn bộ tập dữ liệu khổng lồ vào bộ nhớ ngữ cảnh. |
| **Văn phong & Lập luận Pháp lý** | Khá tốt, rõ ràng nhưng đôi khi mang văn phong kỹ thuật, ít uyển chuyển trong văn bản hành chính dài. | **Dẫn đầu:** Văn phong mượt mà, chuẩn mực hành chính, lập luận pháp lý sắc bén, chặt chẽ và ít bị lặp ý. | Khá tốt, tuy nhiên thường được ưa chuộng hơn trong các tác vụ tổng hợp thông tin từ kho tài liệu khổng lồ. |
| **Ngữ cảnh & Đa phương thức (Video/Audio)** | Ngữ cảnh trung bình (khoảng 128k tokens), xử lý tốt hình ảnh và âm thanh tương tác trực tiếp. | Ngữ cảnh trung bình-lớn (khoảng 200k tokens), phân tích tài liệu văn bản dài hiệu quả. | **Vô địch:** Ngữ cảnh siêu lớn từ 1M đến 2M+ tokens, xử lý trực tiếp video dài hàng giờ, âm thanh hoặc kho tài liệu hàng ngàn trang cùng lúc. |

---

## Phần 2: Ghép nối & Giải trình hạ tầng cho MartX

Dựa trên đặc thù bài toán nghiệp vụ của từng phòng ban, phương án phân bổ tối ưu được thiết lập như sau:

### 1. Kế toán & Phân tích

* **Mô hình lựa chọn:** **OpenAI GPT-4o**
* **Giải trình kỹ thuật ngắn gọn:**
Phòng Kế toán cần xử lý tập dữ liệu file Excel khổng lồ (1,5 triệu dòng) và vẽ biểu đồ. **GPT-4o** sở hữu tính năng *Advanced Data Analysis (Code Interpreter)* mạnh mẽ, cho phép tự động viết và thực thi mã Python trực tiếp trong môi trường sandbox để lọc dữ liệu, tính toán thống kê và trực quan hóa dữ liệu lớn một cách nhanh chóng, chính xác mà không bị tràn bộ nhớ.

### 2. Pháp chế & Văn thư

* **Mô hình lựa chọn:** **Claude 3.5 Sonnet**
* **Giải trình kỹ thuật ngắn gọn:**
Việc soạn thảo hợp đồng đại lý dài 80 trang đòi hỏi sự chuẩn xác cao độ về câu chữ, tính logic pháp lý chặt chẽ và văn phong hành chính tinh tế. **Claude 3.5 Sonnet** hiện là mô hình dẫn đầu về khả năng tạo văn bản tự nhiên, sắc sảo, hiểu sâu sắc các ràng buộc pháp lý và duy trì tính nhất quán xuyên suốt các văn bản dài.

### 3. An ninh & Giám sát

* **Mô hình lựa chọn:** **Gemini 1.5 Pro**
* **Giải trình kỹ thuật ngắn gọn:**
Yêu cầu tải lên video camera quầy thu ngân dài tới 1.5 tiếng để phân tích hành vi, thái độ đòi hỏi mô hình có khả năng xử lý video nguyên bản (Native Multimodal) kết hợp cửa sổ ngữ cảnh cực lớn (*Super Large Context Window*). **Gemini 1.5 Pro** với dung lượng ngữ cảnh lên tới 2 triệu tokens có thể nạp trọn vẹn tệp video dài vào bộ nhớ để truy vấn, phân tích chi tiết từng mốc thời gian mà không bị cắt nhỏ dữ liệu.
