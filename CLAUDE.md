# Portfolio – hướng dẫn cho Claude

## Skills thiết kế (đã cài trong `.claude/skills/`)
- **Gu thẩm mỹ & quy trình**: `frontend-design`, `design-brief`, `design-tokens`, `design-review`, `design-flow`, `information-architecture`, `brief-to-tasks`, `grill-me` (julianoczkowski/designer-skills)
- **Chuyển động**: `emil-design-eng` (emilkowalski/skills) – timing, easing, spring, reduced-motion
- **QA giao diện**: `impeccable` (pbakaus/impeccable), `web-design-guidelines` (vercel-labs/agent-skills)

Quy trình: brief/tokens -> dựng UI -> chuyển động -> rà soát bằng `design-review` / `impeccable` / `web-design-guidelines` (lệch pixel, thang 4px, dark mode, tương phản, a11y) trước khi báo xong.

## Tech stack (đã chốt)
Next.js + Tailwind CSS + shadcn/ui; Magic UI / Aceternity cho hiệu ứng; Framer Motion (motion) cho chuyển động. Repo chưa scaffold app.

## Thư viện component (không phải skill – cài khi dựng UI)
shadcn/ui (`npx shadcn@latest add <component>`), Magic UI, Aceternity UI. Ưu tiên lấy block có sẵn thay vì tự code từ đầu; chỉ dùng khi stack của repo là React + Tailwind.

## Tạo ảnh
Dùng Higgsfield MCP (`https://mcp.higgsfield.ai/mcp`) nếu connector đã bật trong session.

## Bảo mật
Skill chạy với quyền agent. `impeccable/scripts/` có script thực thi (live-browser...) – chỉ chạy khi cần và đã đọc qua.
