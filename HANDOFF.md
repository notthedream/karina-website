> Codex: อ่านไฟล์นี้และ `git log` ก่อนเริ่มงานทุกครั้ง แล้วสรุปสถานะให้พี่น็อตก่อนทำต่อ
> หมายเหตุ: ไฟล์นี้สรุปจาก repo บน GitHub (ยังไม่ได้รวมแชต Codex เก่าบน Mac mini เพราะเครื่องออฟไลน์ตอนทำ) ห้าม commit ไฟล์ลับ/คีย์

# HANDOFF — Karina Website
- เว็บการตลาดภาษาอังกฤษของ Karina Media Player ใน `public/` deploy อัตโนมัติด้วย GitHub Pages (.github/workflows/pages.yml) เมื่อ push main
- ล่าสุด: เพิ่มข้อมูลดาวน์โหลด Karina 7.0.0 preview (release karina-v7.0.0-preview, macOS 15+, ยังไม่ notarize)
## Next steps
1. เช็กลิงก์ดาวน์โหลดและหน้าเว็บบน Pages ว่าทำงาน
2. อัปเดตเนื้อหาให้ตรงกับฟีเจอร์ใน best-media-player ทุกครั้งที่ออกเวอร์ชัน
3. SEO พื้นฐาน (meta, og image, sitemap)

## จากแชตเก่า (Codex บน Mac mini, อ่านเมื่อ 23 ต.ค.)
- แชต: เดียวกับ best-media-player โฟลเดอร์งานคือ /Volumes/Macintosh SSD DATA/ChatGPT/Codex/2026-10-21/karina-website (clean, push ครบ)
- เสร็จแล้ว: เว็บขึ้นแล้วที่ https://notthedream.github.io/karina-website/ และ release karina-v7.0.0-preview (zip ~26.3 MB) ตรวจแล้วไม่มีรหัสผ่าน คีย์ หรือไฟล์ส่วนตัวหลุด
- repo นี้เป็น public ห้ามใส่ไฟล์ส่วนตัว วิดีโอ หรือซับส่วนตัว
- พี่น็อตเคยถามเรื่อง host กับโดเมน: ตอนนี้ใช้ GitHub Pages ฟรี ยังไม่มีโดเมนของตัวเอง (ถ้าจะซื้อโดเมน: รอถามพี่น็อต)
- Next: ถ้าจะทำ signed release ต้องมี Developer ID (เสียเงิน)
