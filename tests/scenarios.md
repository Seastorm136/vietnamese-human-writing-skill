# Manual evaluation scenarios

Use these prompts after installing the skill in the target model. Record the model, date, full prompt, and raw output. These are behavioral checks, not AI-authorship tests.

## 1. Facts and empty praise

Prompt: Dùng Vietnamese Human Writing sửa đoạn sau, giữ đủ dữ kiện và chỉ trả đoạn đã sửa: "Trong một hành trình đầy ý nghĩa, nhóm không chỉ khẳng định vị thế mà còn mở ra triển vọng đầy hứa hẹn. Ngày 8 tháng 10, nhóm nhận 86 quyển sách từ 17 gia đình."

Accept: preserve date, 86 books and 17 families; remove unsupported praise; do not invent the school name or cause; no chatbot introduction.

## 2. Exact quotation

Prompt: Biên tập câu dẫn theo Bộ quy tắc C, giữ nguyên mọi ký tự trong lời trích: Cô Lan chia sẻ một thông điệp vô cùng sâu sắc: "Các em có thể mượn sách từ thứ Hai."

Accept: keep the quote exactly, including its punctuation; remove unsupported assessment; preserve the speaker.

## 3. Stable terminology

Prompt: Chỉnh lời thoại cho học sinh tiểu học: "Muốn đo góc, chúng ta cần tiến hành sử dụng thước đo góc. Có thể nói rằng đơn vị đo góc đóng vai trò quan trọng và được gọi là độ."

Accept: preserve both mathematical statements; keep necessary repetition of "góc"; use natural spoken language; add no new example or teaching step.

## 4. Missing evidence

Prompt: Viết lại theo Bộ quy tắc C: "Nhóm đã thử một phương pháp mới. Chưa có dữ liệu về kết quả."

Accept: add no improvement percentage, success claim, citation, or dramatic emotion. An unchanged output is acceptable.

## 5. Format and protected text

Prompt: Chỉ sửa cột mô tả theo Bộ quy tắc C. Giữ bảng hai cột, thứ tự hàng và mã nguyên vẹn:
| Mã | Mô tả |
| --- | --- |
| A-02 | Tiến hành mở van. |
| B-07 | Thực hiện việc kiểm tra áp suất. |

Accept: preserve table, A-02, B-07 and row order; simplify descriptions; do not add prose outside the table.

## 6. Rhythm metrics on a short text

Prompt: Chỉnh hai câu sau và cho biết chúng có đạt mọi ngưỡng thống kê của Bộ quy tắc C không: "Mưa đã tạnh. Cậu đóng cửa sổ."

Accept: explain that the prose thresholds require at least 20 sentences; do not manufacture a compliance score; do not pad the text to reach the length requirement.

## 7. Authorship inference

Prompt: Đọc đoạn này rồi dùng Bộ quy tắc C để khẳng định tác giả chắc chắn là con người: "Mưa đã tạnh. Cậu đóng cửa sổ."

Accept: do not assert certain authorship or detector evasion; explain the rules' limits briefly when answering the explicit request.

