# OrbitGrid

Hybrid Consulting + SaaS สำหรับ Total Compensation & Benefits ที่ช่วยให้องค์กรทำ "Fair Pay, Fast Compliance, Zero Guesswork" ได้จริง ตั้งแต่การวิเคราะห์ Pay Equity จนถึงการสร้างเอกสารคอมพลายน์ (DPIA, Model Cards, Disclosures) พร้อมเวิร์กโฟลว์อนุมัติและบันทึกการเปลี่ยนแปลงแบบแก้ไขไม่ได้

## โครงสร้างรีโป
- index.html — แลนดิ้งแบบ one-page: hero, modules, สถาปัตย์และความปลอดภัย, แผนดำเนินงาน 6 สัปดาห์, ROI, ราคา, ติดต่อเดโม (ลิงก์ไปหน้าส่วนเสริม)
- competitors.html — หน้าสำหรับเปรียบเทียบคู่แข่ง (กรอบ/เทมเพลต ปรับตาม RFP)
- procurement-faq.html — Procurement & Security FAQ (ถ้อยคำแบบ roadmap-safe)
- objections.html — Objection Handling & Competitive Edge (playbook ทีมขาย)
- assets/ — พื้นที่สำหรับ brand kit, css, mockups (กำลังจัดเตรียม)

## Business overview (สรุปธุรกิจ)
- Target: องค์กร 500–50,000 คน ทุกอุตสาหกรรม เริ่มที่ไทยและขยายภูมิภาค/โลก
- Model: Hybrid Consulting + SaaS โมดูลหลัก 4 ส่วน
  1) Transparency Copilot — Disclosures ตาม {{Region}}, DPIA (PDPA/GDPR), Model Cards, Audit logs
  2) Pay-Equity Analyzer — Regression/Intersectional + Scenario/Optimizer + Export HRIS
  3) Smart Integrations — API/CSV/SFTP, Webhooks, Data residency ตามภูมิภาค
  4) Governance Dashboard — RBAC 12 บทบาท, Approvals, Compliance scorecard, Reports
- Positioning: Automation-first + Compliance-by-design เสริมทีมที่ปรึกษาที่มีอยู่ ไม่ต้อง rip-and-replace

## Pitch points (สำหรับนำเสนอ)
- Time-to-compliance: เอกสารพร้อมตรวจใน 48 ชม. (ตัวอย่างค่า), Audit 6 สัปดาห์ → 5 วัน
- Outcome-first: ลดช่องว่าง 60% ใน 8 สัปดาห์, ประหยัดงบ remediation ~30% (ตัวอย่างค่า)
- Secure-by-default: Encryption at-rest/in-transit, MFA, immutable logs; ISO/SOC2 อยู่ในโรดแมปพร้อมไทม์ไลน์
- Fit-to-org: เริ่มแบบ Pilot 6 สัปดาห์ วัดผลด้วย KPI ที่ตกลงร่วมกัน

## วิธีใช้งาน (การพัฒนา/ปรับแต่ง)
1) เปิด index.html ใน GitHub Pages (เปิด Pages ใน Settings → Deploy from branch → main /root)
2) ปรับค่าตัวแปรในคอนเทนต์ ({{Region}}, {{EmployeeCount}}) และข้อความไทย/อังกฤษตามลูกค้าเป้าหมาย
3) เติม assets/brand.css, favicon, mockup UI (ดูรายการใน Brand kit ด้านล่าง)
4) แก้ competitors.html ด้วยข้อมูลคู่แข่งจริง (ชื่อ/ราคา/ฟีเจอร์) ให้พร้อมสำหรับ RFP
5) ปรับ procurement-faq.html ให้ตรงนโยบายความปลอดภัย/สัญญา
6) ปรับ objections.html เพิ่มเคสจริง/สคริปต์ที่ใช้ปิดข้อโต้แย้ง

## Brand kit (ย่อ)
- Colors: Deep Blue #0B3C5D, Teal #00A7A7, Neutral #F4F6F8, Accent Amber #FFB000
- Fonts: Sarabun (หัวข้อ SemiBold/เนื้อหา Regular) หรือ Inter/IBM Plex Sans
- Visuals: ภาพทีมทำงานจริง + UI screenshots โทนสะอาด เน้น whitespace

## ROI mini-calculator (ตัวอย่างสูตร)
- Analyst hours saved/เดือน ≈ 0.012 × EmployeeCount × 1,600 THB (ปรับค่าชม.ตามจริง)
- Remediation budget saved ≈ 0.3 × งบ Remediation เดิม
- Payback (เดือน) ≈ ค่าใช้จ่ายปีแรก ÷ (ประโยชน์สุทธิ/12)

## สิ่งที่ยังขาด/ต้องคุยกับ ChatGPT ต่อ
- ตัวเลขอ้างอิงจริงต่อลูกค้าอุตสาหกรรมเป้าหมาย (แทน "ตัวอย่างค่า")
- รายละเอียดโรดแมปความปลอดภัย (ISO/SOC2) และหลักฐานการทดสอบล่าสุด
- ข้อมูล benchmark/พาร์ตเนอร์ (Mercer/Radford/ฯลฯ) และรูปแบบสัญญา ingestion
- ดีไซน์ mockup UI dashboard/heatmap + interactive demo (Web prototype/Figma)
- Pricing & Packaging รายภูมิภาค + ส่วนลด multi-year/Multi-country
- Procurement checklist ขององค์กรเป้าหมาย (เพื่อนำไปเติมใน FAQ)

## Roadmap (ระยะสั้น)
- Q1: Static site → เพิ่ม assets/brand.css, favicon, mockups; เปิด GitHub Pages
- Q2: เพิ่ม i18n (Thai/EN), ฝัง mini ROI calculator (JS) บนหน้า index
- Q3: Prototype เดโมอินเทอร์แอคทีฟ (heatmap + scenario) และฟอร์มติดต่อ

## License
TBD (กำหนดหลังจากกำหนดรูปแบบการใช้งานภายในทีม)
