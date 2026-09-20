# Team Follow-up Web App

เว็บแอปสำหรับติดตามงานกับทีม โดยเน้นงาน Daily / Weekly Follow-up

## Live site
Expected GitHub Pages URL after Pages is enabled:

https://pornchaipsj-ui.github.io/team-followup-app/

## Features
- Dashboard: Total Tasks, Due Today, Overdue, Blocked, Average Progress
- Task Follow-up Register
- Plan % vs Actual % และ Gap
- Status: Not Started / In Progress / Blocked / Done
- Area / Owner / System / Contractor
- Blocker / Reason
- Next Action / Recovery Plan
- Search & Filters
- Kanban Status Board
- Export CSV
- Backup / Restore JSON
- Responsive สำหรับมือถือและคอมพิวเตอร์

## Deployment
Repository นี้มี GitHub Actions workflow ที่ `.github/workflows/pages.yml`

หลังเปิด **Settings → Pages → Build and deployment → Source → GitHub Actions** แล้ว ทุกครั้งที่มีการ push เข้า `main` ระบบจะ deploy เว็บไซต์อัตโนมัติ

## Usage
เปิด `index.html` ผ่าน browser ได้โดยตรง หรือใช้ GitHub Pages URL ด้านบนเมื่อ deploy สำเร็จ

## Data storage
เวอร์ชัน MVP เก็บข้อมูลด้วย browser `localStorage` ดังนั้นข้อมูลของแต่ละ browser/device จะแยกจากกัน

สำหรับการใช้งานร่วมกันหลายคน ควรเชื่อมฐานข้อมูลกลางและระบบ authentication ในขั้นถัดไป
