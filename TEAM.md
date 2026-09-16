# TEAM — Day04, K4-L3B

## Thông tin bài nộp

- Tên nhóm: Nguyễn Hoàng Tuyền Team
- Người đại diện / MSSV: Nguyễn Hoàng Tuyền / 2A202602439
- Tên repo: `K4-L3-DAY04-NguyenHoangTuyen-2A202602439-PromptEngineeringToolCalling`
- URL repo, nhánh nộp, commit chốt: `https://github.com/Tuyen2k47/K4-L3-DAY04-NguyenHoangTuyen-2A202602439-PromptEngineeringToolCalling`
- Deadline áp dụng: 23:59 ngày học (UTC+07:00)

## Thành viên

| Họ và tên | MSSV | GitHub | Vai trò và công việc | File/commit/PR |
|---|---|---|---|---|
| Nguyễn Hoàng Tuyền | 2A202602439 | Tuyen2k47 | Trưởng nhóm, Prompt Engineering, Setup Ollama & OpenRouter, Viết Report | `artifacts/system_prompt.md`, `artifacts/REPORT.md` |

## Nhận xét chung

- Kết quả và bằng chứng: Đạt case_accuracy 1.00 (30/30 base cases pass) ở phiên bản v3; tool_routing_accuracy = 1.0. Tự viết 10 case nhóm trong `data/eval_group.json` đạt 10/10.
- Thay đổi hiệu quả nhất: Bổ sung các quy tắc phân tách rõ ràng giữa tra cứu và xác nhận tạo ticket (`clarify` yes_no), ép buộc map đúng `environment` và `category` trong prompt.
- Giới hạn còn lại: Cần điều chỉnh rate limit delay phù hợp khi gọi các API công cộng miễn phí.
- Cách phân công và tích hợp: Xây dựng môi trường ảo, tự động hóa chạy eval và tổng hợp kết quả chi tiết vào version log.

## INDIVIDUAL

### Nguyễn Hoàng Tuyền — 2A202602439

- Phần việc và file/commit/PR: Toàn bộ quá trình phân tích v0, tối ưu `system_prompt.md`, viết 10 case test nhóm `data/eval_group.json`, cấu hình Ollama local và hoàn thiện báo cáo `artifacts/REPORT.md`.
- Quyết định, khó khăn và cách xử lý: Xử lý sự cố Rate Limit API (429) bằng cách thiết lập Ollama local `llama3.1` trên ổ E và tích hợp cơ chế Smart Fallback trong script đánh giá.
- Điều đã học: Hiểu sâu sắc về cơ chế Function Calling / Tool Calling của LLM, quy trình Prompt Engineering theo vòng lặp v0-v3 có đối chứng qua metric.
- AI/công cụ đã dùng và cách kiểm tra: Sử dụng Antigravity AI assistant, OpenRouter, Ollama local llama3.1, kiểm thử tự động với `run_eval.py`.
- Thời điểm đã tự nộp URL repo chung trên VLearn: Đã hoàn tất và sẵn sàng nộp.
