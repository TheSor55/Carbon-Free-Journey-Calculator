# 🌿 Carbon-Free Journey Calculator

**เที่ยวไทย ไม่ทิ้งคาร์บอน** — คำนวณรอยเท้าคาร์บอนจากทริปท่องเที่ยวของคุณ

> ส่งประกวดโครงการ **"Carbon-Free Journey"**  
> จัดโดย องค์การบริหารจัดการก๊าซเรือนกระจก (อบก. · TGO)  
> `#เที่ยวไทยไม่ทิ้งคาร์บอน` `#CarbonFreeJourney`

---

## 🔗 Live Demo

**[thesor55.github.io/carbon-free-journey](https://thesor55.github.io/carbon-free-journey)**

---

## ✨ Features

### 🗺️ Trip Setup
- กรอกจุดออกเดินทาง / ปลายทาง / สถานที่ท่องเที่ยว
- เลือกประเภทผู้เดินทาง: ครอบครัว / กลุ่มเพื่อน / คู่รัก / เดี่ยว / ทีมงาน
- Hero chips และ result title อัปเดต real-time ตามข้อมูลที่กรอก

### 🚗 การเดินทาง (12 ประเภท)
| ประเภท | EF | หน่วย |
|---|---|---|
| ดีเซล B20 | 2.33 | kgCO₂/L |
| ดีเซล Premier | 2.68 | kgCO₂/L |
| เบนซิน | 2.31 | kgCO₂/L |
| แก๊สโซฮอล์ (95) | 2.14 | kgCO₂/L |
| LPG | 1.63 | kgCO₂/L |
| รถไฟฟ้า EV | 0.50 | kgCO₂/kWh |
| มอเตอร์ไซค์ | 2.31 | kgCO₂/L |
| VIP Bus | 0.028 | kgCO₂/pkm |
| 🚂 รถไฟ | 0.045 | kgCO₂/pkm |
| ✈️ เครื่องบิน Low-Cost | 0.255 | kgCO₂/pkm |
| 🚕 Taxi / Grab | 0.21 | kgCO₂/pkm |
| 🚈 BTS / MRT | 0.035 | kgCO₂/pkm |

- สลับหน่วย **กม./ลิตร ↔ ลิตร/100กม.** real-time
- Dynamic fuel hint อธิบาย EF แต่ละประเภทอัตโนมัติ

### 🌲 กิจกรรม (16 กิจกรรม / 4 หมวด)
- 🌿 ธรรมชาติ & กีฬา: เดินป่า, ปั่นจักรยาน, เดินเทรล, ว่ายน้ำ
- 🏛️ วัฒนธรรม: ไหว้วัด, เดินตลาด, ซื้อของฝาก
- ⚓ ทางน้ำ: ดำน้ำ, เรือข้ามเกาะ, สปีดโบ๊ท, คายัค
- 🏌️ กีฬา: กอล์ฟ, ATV, ซิปไลน์

### 📊 ผลลัพธ์
- **Low Carbon Score** (0–100) + Grade
- **Impact Snapshot** — hotspot detection อัตโนมัติ
- **Smart Recommendation** — 4 ด้าน
- **Scenario Grid** — B20 vs EV vs Train
- **Emission Breakdown** — สัดส่วน % พร้อม progress bar
- **Compare Panel** — น้ำมันที่เลือก vs B7 baseline
- **Carbon Offset Options** — ต้นไม้ / Solar / T-VER
- **Methodology Card** — IPCC / TGO / EGAT / DEDE
- 💾 **Save as PNG** — ชื่อไฟล์ตามทริปจริง

### 🌍 Bilingual TH / EN
- Toggle ได้ทุกจุด — re-render ทุก section ทันที

### 📱 Mobile-First
- iPhone Dynamic Island / Notch / Home Bar safe areas
- Android theme color, no tap highlight
- font-size 16px ป้องกัน iOS auto-zoom

---

## ⚡ Emission Factors อ้างอิง

**IPCC** · **DEDE Thailand** · **TGO** · **EGAT Grid EF 2024** · **IATA**

---

## 🚀 วิธีใช้งาน

```bash
git clone https://github.com/thesor55/carbon-free-journey.git
cd carbon-free-journey
open index.html
```

## 🌐 GitHub Pages

**Settings → Pages → Branch: main / root → Save**

---

## 📁 โครงสร้าง

```
carbon-free-journey/
├── index.html   ← All-in-one (HTML + CSS + JS)
└── README.md
```

---

**Sorawit Suwannarong & Family** · [github.com/thesor55](https://github.com/thesor55)
