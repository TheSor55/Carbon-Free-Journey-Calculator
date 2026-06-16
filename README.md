# 🌿 Carbon-Free Journey Calculator · V7.1

**เที่ยวไทย ไม่ทิ้งคาร์บอน** — คำนวณรอยเท้าคาร์บอนจากทริปท่องเที่ยวของคุณ

> ส่งประกวดโครงการ **"Carbon-Free Journey"**  
> จัดโดย องค์การบริหารจัดการก๊าซเรือนกระจก (อบก. · TGO)  
> `#เที่ยวไทยไม่ทิ้งคาร์บอน` `#CarbonFreeJourney`

---

## 🔗 Live Demo

**[thesor55.github.io/carbon-free-journey](https://thesor55.github.io/carbon-free-journey)**

---

## ✨ Features

### 🧮 การคำนวณ
- คำนวณ Carbon Footprint จาก **การเดินทาง + อาหาร + ที่พัก + กิจกรรม**
- รองรับน้ำมัน/พาหนะ 9 ประเภท: B7, B20, Diesel Premier, Gasohol E10, EV, มอเตอร์ไซค์, VIP Bus, รถไฟ
- สลับหน่วย **กม./ลิตร ↔ ลิตร/100กม.** พร้อม auto-convert real-time
- Dynamic fuel hint — อธิบายข้อดี/ข้อเสียน้ำมันแต่ละประเภทอัตโนมัติ

### 📊 ผลลัพธ์ V7.1
- **Low Carbon Score** (0–100) พร้อม Grade: คาร์บอนต่ำมาก / ต่ำ / ปานกลาง / สูง
- **Impact Snapshot** — ระบุ hotspot การปล่อยหลัก อัตโนมัติ
- **Smart Recommendation** — คำแนะนำ 4 ด้าน: รถไฟ, EV, ที่พัก, อาหาร
- **Scenario Comparison** — เปรียบเทียบ B20 vs EV vs Train+ พร้อมกัน
- **Breakdown Chart** — สัดส่วนการปล่อยแต่ละ category พร้อม progress bar
- **Compare Panel** — Dynamic เปรียบเทียบน้ำมันที่เลือก vs B7 baseline
- **Carbon Offset Options** — ต้นไม้ / Solar / รถไฟ / T-VER credit
- **Methodology Card** — แสดง EF source อ้างอิง: IPCC, TGO, EGAT, DEDE
- 💾 **Save as PNG** — บันทึกผลเป็นรูปภาพพร้อมชื่อทริป

### 🌍 Bilingual
- สลับ **TH / EN** ได้ทุกจุด — re-render ทุก section อัตโนมัติ
- รองรับ dynamic text ทั้ง Score, Impact, Recommendations, Offset

### 📱 Mobile-First
| อุปกรณ์ | การรองรับ |
|---|---|
| iPhone (iOS Safari) | Dynamic Island, Notch, Home Bar safe areas |
| Android (Chrome) | Theme color `#1a3a2a`, no tap highlight |
| iPad / Tablet | Responsive 2-column grid |
| Desktop | Max-width 860px centered |

---

## ⚡ Emission Factors (EF)

| พาหนะ / น้ำมัน | EF | หน่วย | อ้างอิง |
|---|---|---|---|
| ดีเซล B7 | 2.68 | kgCO₂/L | IPCC / DEDE |
| ดีเซล B20 | 2.33 | kgCO₂/L | biogenic carbon ~13% reduction |
| Diesel Premier | 2.68 | kgCO₂/L | = B7 (ต่างแค่ PM/SOx/NOx) |
| เบนซิน | 2.31 | kgCO₂/L | IPCC |
| Gasohol E10 | 2.14 | kgCO₂/L | ethanol blend ~7.5% reduction |
| รถไฟฟ้า EV | 0.50 | kgCO₂/kWh | EGAT Grid EF 2024 |
| มอเตอร์ไซค์ | 2.31 | kgCO₂/L | IPCC |
| VIP Bus | 0.028 | kgCO₂/pkm | inter-city coach average |
| รถไฟ (+บขส.) | 0.045 | kgCO₂/pkm | diesel rail Thailand |

> **หมายเหตุ:** รถไฟสายตะวันออกสิ้นสุดที่ระยอง (มาบตาพุด) — ต่อ บขส./รถตู้เพื่อไปจันทบุรี

---

## 🔢 Low Carbon Score Algorithm

```
score = clamp(0, 100,  100 − (emissionPerPerson × 1.8) + (reductionVsB7% × 20) )
```

| ช่วงคะแนน | ระดับ |
|---|---|
| 85–100 | คาร์บอนต่ำมาก 🌿 |
| 70–84 | คาร์บอนต่ำ 💚 |
| 50–69 | ระดับปานกลาง ⚠️ |
| 0–49 | คาร์บอนสูง 🔥 |

---

## 🚀 วิธีใช้งาน (Local)

```bash
# Clone repo
git clone https://github.com/thesor55/carbon-free-journey.git
cd carbon-free-journey

# เปิดใน browser (ไม่ต้อง install อะไร — Pure HTML/CSS/JS)
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

---

## 🌐 Deploy บน GitHub Pages

1. ไปที่ **Settings** ของ repo → **Pages**
2. Source: **Deploy from a branch** → Branch: **main** / Folder: **/ (root)**
3. กด **Save** → รอ ~1 นาที
4. เข้าที่ `https://thesor55.github.io/carbon-free-journey`

---

## 📁 โครงสร้างไฟล์

```
carbon-free-journey/
├── index.html   ← แอปหลัก (all-in-one: HTML + CSS + JS)
└── README.md    ← เอกสารนี้
```

> ไฟล์เดียว ไม่มี dependency ภายนอก (html2canvas โหลดจาก CDN อัตโนมัติ)

---

## 🎬 เกี่ยวกับทริปนี้

| รายละเอียด | ข้อมูล |
|---|---|
| เส้นทาง | ศรีราชา → น้ำตกเขาชะเมา → จันทบุรี → น้ำตกพริ้ว → ศรีราชา |
| พาหนะ | Isuzu MU-X 1.9 ดีเซล · เติม B20 · 13 กม./ลิตร |
| ผู้โดยสาร | ครอบครัว 4 คน |
| ระยะทาง | ~520 กม. (ไป-กลับ) |
| ที่พัก | โรงแรม 1 คืน · จันทบุรี |
| กิจกรรม | เดินน้ำตก · ไหว้เจ้าตาก · เก็บสแตมป์ลาบเซนต์อุทยาน |

---

## 📋 Changelog

| Version | รายละเอียด |
|---|---|
| **V7.1** | Low Carbon Score, Smart Recommendation, Scenario Grid, Impact Snapshot, Methodology Card, Bilingual TH/EN fix |
| **V7.0** | Compare panel dynamic, กม./ลิตร toggle, Dynamic fuel hint |
| **V6.x** | Save as PNG, End Credit, Mobile-first (safe areas) |
| **V5.x** | Carbon Offset options, T-VER, breakdown chart |
| **V1–4** | Initial calculator: transport / food / stay |

---

**Sorawit Suwannarong & Family** · [github.com/thesor55](https://github.com/thesor55)

*EF Reference: IPCC · DEDE Thailand · TGO · EGAT Grid Emission Factor 2024*
