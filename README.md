<defs>
  <radialGradient id="glow" cx="50%" cy="50%" r="50%">
    <stop offset="0%" stop-color="#ff1a1a" stop-opacity="0.55"/>
    <stop offset="60%" stop-color="#8a0000" stop-opacity="0.18"/>
    <stop offset="100%" stop-color="#000" stop-opacity="0"/>
  </radialGradient>
  <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
    <stop offset="0%" stop-color="#050505"/><stop offset="55%" stop-color="#0d0203"/><stop offset="100%" stop-color="#050505"/>
  </linearGradient>
  <linearGradient id="txt" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0%" stop-color="#ffffff"/><stop offset="50%" stop-color="#d9d9d9"/><stop offset="100%" stop-color="#ff2a2a"/>
  </linearGradient>
  <linearGradient id="scan" x1="0" y1="0" x2="1" y2="0">
    <stop offset="0%" stop-color="#ff1a1a" stop-opacity="0"/><stop offset="50%" stop-color="#ff1a1a" stop-opacity="0.9"/><stop offset="100%" stop-color="#ff1a1a" stop-opacity="0"/>
  </linearGradient>
  <clipPath id="circ"><circle cx="210" cy="210" r="150"/></clipPath>
  <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
    <path d="M40 0H0V40" fill="none" stroke="#ff1a1a" stroke-opacity="0.08" stroke-width="1"/>
  </pattern>
  <filter id="blur"><feGaussianBlur stdDeviation="6"/></filter>
</defs>

<rect width="1200" height="420" fill="url(#bg)"/>
<rect width="1200" height="420" fill="url(#grid)">
  <animateTransform attributeName="transform" type="translate" from="0 0" to="40 40" dur="6s" repeatCount="indefinite"/>
</rect>

<!-- crimson halo behind logo -->
<circle cx="210" cy="210" r="260" fill="url(#glow)">
  <animate attributeName="r" values="230;285;230" dur="4s" repeatCount="indefinite"/>
  <animate attributeName="opacity" values="0.7;1;0.7" dur="4s" repeatCount="indefinite"/>
</circle>

<!-- rotating gears (decor) -->
<g transform="translate(1060 90)" opacity="0.35">
  <circle r="70" fill="none" stroke="#ff1a1a" stroke-width="14" stroke-dasharray="14 11"/>
  <circle r="48" fill="none" stroke="#ff1a1a" stroke-width="2"/>
  <circle r="10" fill="#ff1a1a"/>
  <animateTransform attributeName="transform" type="rotate" from="0 0 0" to="360 0 0" dur="24s" repeatCount="indefinite" additive="sum"/>
</g>
<g transform="translate(1000 330)" opacity="0.3">
  <circle r="46" fill="none" stroke="#ff1a1a" stroke-width="10" stroke-dasharray="10 8"/>
  <circle r="30" fill="none" stroke="#ff1a1a" stroke-width="2"/>
  <circle r="7" fill="#ff1a1a"/>
  <animateTransform attributeName="transform" type="rotate" from="360 0 0" to="0 0 0" dur="16s" repeatCount="indefinite" additive="sum"/>
</g>


<circle cx="210" cy="210" r="152" fill="none" stroke="#ff1a1a" stroke-width="4">
  <animate attributeName="stroke-opacity" values="1;0.35;1" dur="2.6s" repeatCount="indefinite"/>
</circle>
<circle cx="210" cy="210" r="168" fill="none" stroke="#ff1a1a" stroke-width="1.5" stroke-dasharray="6 10" stroke-opacity="0.7">
  <animateTransform attributeName="transform" type="rotate" from="0 210 210" to="360 210 210" dur="18s" repeatCount="indefinite"/>
</circle>

<!-- text -->
<text x="420" y="150" font-family="Impact, 'Arial Black', 'Segoe UI', sans-serif" font-size="82" letter-spacing="6" fill="url(#txt)">DHIREN DHALL
  <animate attributeName="opacity" values="0;1" dur="1.6s" fill="freeze"/>
</text>
<text x="424" y="205" font-family="'Courier New', monospace" font-size="30" letter-spacing="14" fill="#ff1a1a" font-weight="bold">THE MECHA RONIN
  <animate attributeName="opacity" values="0;1" begin="0.6s" dur="1.6s" fill="freeze"/>
</text>
<rect x="424" y="228" width="520" height="3" fill="url(#scan)">
  <animate attributeName="width" values="40;520;40" dur="5s" repeatCount="indefinite"/>
</rect>
<text x="424" y="275" font-family="'Courier New', monospace" font-size="22" letter-spacing="5" fill="#e6e6e6">CODE • DESIGN • BUILD • AUTOMATE</text>
<text x="424" y="315" font-family="'Courier New', monospace" font-size="18" letter-spacing="4" fill="#9a9a9a">TURNING IDEAS INTO MACHINES</text>
<text x="424" y="352" font-family="'Courier New', monospace" font-size="15" letter-spacing="3" fill="#ff4d4d">MECHATRONICS  |  ROBOTICS  |  CAD/CAM  |  VIDEO EDITING</text>

<!-- drifting petals -->
<g fill="#ff1a1a">
  <circle r="3" cx="620" cy="-10" opacity="0.8"><animate attributeName="cy" values="-10;430" dur="7s" repeatCount="indefinite"/><animate attributeName="cx" values="620;560;640" dur="7s" repeatCount="indefinite"/></circle>
  <circle r="2" cx="760" cy="-10" opacity="0.6"><animate attributeName="cy" values="-10;430" dur="9s" begin="1s" repeatCount="indefinite"/><animate attributeName="cx" values="760;820;740" dur="9s" begin="1s" repeatCount="indefinite"/></circle>
  <circle r="3" cx="900" cy="-10" opacity="0.7"><animate attributeName="cy" values="-10;430" dur="8s" begin="2s" repeatCount="indefinite"/><animate attributeName="cx" values="900;860;930" dur="8s" begin="2s" repeatCount="indefinite"/></circle>
  <circle r="2" cx="500" cy="-10" opacity="0.5"><animate attributeName="cy" values="-10;430" dur="10s" begin="3s" repeatCount="indefinite"/><animate attributeName="cx" values="500;540;480" dur="10s" begin="3s" repeatCount="indefinite"/></circle>
  <circle r="2.5" cx="1100" cy="-10" opacity="0.6"><animate attributeName="cy" values="-10;430" dur="6s" begin="0.5s" repeatCount="indefinite"/><animate attributeName="cx" values="1100;1140;1080" dur="6s" begin="0.5s" repeatCount="indefinite"/></circle>
</g>

<!-- moving red scan line across whole banner -->
<rect x="-300" y="0" width="300" height="420" fill="url(#scan)" opacity="0.10">
  <animate attributeName="x" values="-300;1200" dur="7s" repeatCount="indefinite"/>
</rect>

<!-- bottom edge glow -->
<rect x="0" y="412" width="1200" height="8" fill="#ff1a1a">
  <animate attributeName="opacity" values="1;0.35;1" dur="3s" repeatCount="indefinite"/>
</rect>
<rect x="0" y="0" width="1200" height="4" fill="#ff1a1a" opacity="0.7"/>
</svg><div align="center">

<!-- ===== NAME ANIMATION ===== -->
<img src="https://readme-typing-svg.demolab.com?font=Orbitron&weight=900&size=44&duration=3500&pause=1200&color=E10600&center=true&vCenter=true&width=700&height=80&lines=DHIREN+DHALL;THE+MECHA+RONIN" alt="Dhiren Dhall" />

<!-- ===== USERNAME / TAGLINE / CONTACT ANIMATION ===== -->
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=18&duration=2800&pause=1000&color=C9C9C9&center=true&vCenter=true&width=700&height=40&lines=@TheMechaRonin;Code+%E2%80%A2+Design+%E2%80%A2+Build+%E2%80%A2+Automate;Turning+Ideas+into+Machines;%F0%9F%93%9E+8866079191;%E2%9C%89%EF%B8%8F+dhirendhall919@gmail.com" alt="Username, tagline and contact" />

<br/>

![Mechatronics](https://img.shields.io/badge/Mechatronics-E10600?style=for-the-badge&logo=arduino&logoColor=white)
![Robotics](https://img.shields.io/badge/Robotics-1a1a1a?style=for-the-badge&logo=raspberrypi&logoColor=E10600)
![CAD/CAM](https://img.shields.io/badge/CAD%2FCAM-E10600?style=for-the-badge&logo=solidworks&logoColor=white)
![Parul University](https://img.shields.io/badge/Parul_University-1a1a1a?style=for-the-badge&logoColor=white)
![Vadodara](https://img.shields.io/badge/Vadodara%2C_Gujarat-E10600?style=for-the-badge&logoColor=white)

</div>

---

## 🥷 whoami

```json
{
  "name": "Dhiren Dhall",
  "alias": "The Mecha Ronin",
  "role": "Mechatronics Student | CAD/CAM Designer | Robotics Builder",
  "education": "Diploma in Mechatronics, 1st Year — Parul University",
  "company": "Founder, MechaFusion Technologies",
  "location": "Vadodara, Gujarat, India",
  "focus": ["Mechanical Design", "Robotics", "Automation", "PCB Design"],
  "tagline": "Code • Design • Build • Automate",
  "brand": "Turning Ideas into Machines"
}
```

---

## ⚙️ About Me

- 🎓 Diploma **Mechatronics** student (1st year) at **Parul University**, Vadodara
- 🏭 Founder of **MechaFusion Technologies** *(website coming soon)*
- 📐 Designing in **SolidWorks, AutoCAD, Fusion 360 and Solid Edge** — from single parts to big assemblies
- 🤖 Building Arduino robots: line following, obstacle avoiding, Bluetooth-controlled cars
- 🔧 Hands-on with workshop work too: welding (Arc / MIG / TIG), lathe, grinding, basic milling
- 🧠 Code mostly written with **AI assistance** while I keep learning Arduino C++ and Python
- 🎬 Also do **video and photo editing**

---
## 🛠️ Tech Stack

### CAD / Design
![SolidWorks](https://img.shields.io/badge/SolidWorks-E10600?style=for-the-badge&logo=solidworks&logoColor=white)
![AutoCAD](https://img.shields.io/badge/AutoCAD-B00000?style=for-the-badge&logo=autodesk&logoColor=white)
![Fusion 360](https://img.shields.io/badge/Fusion_360-1a1a1a?style=for-the-badge&logo=autodesk&logoColor=E10600)
![Solid Edge](https://img.shields.io/badge/Solid_Edge-E10600?style=for-the-badge&logoColor=white)

### Electronics & Coding
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![C++](https://img.shields.io/badge/C++-1a1a1a?style=for-the-badge&logo=cplusplus&logoColor=E10600)
![Python](https://img.shields.io/badge/Python-B00000?style=for-the-badge&logo=python&logoColor=white)
![PCB Design](https://img.shields.io/badge/PCB_Design-E10600?style=for-the-badge&logoColor=white)

### Fabrication & Creative
![Welding](https://img.shields.io/badge/Welding-1a1a1a?style=for-the-badge&logoColor=E10600)
![Lathe](https://img.shields.io/badge/Lathe_%26_Grinding-E10600?style=for-the-badge&logoColor=white)
![Video Editing](https://img.shields.io/badge/Video_Editing-B00000?style=for-the-badge&logoColor=white)
![Photo Editing](https://img.shields.io/badge/Photo_Editing-1a1a1a?style=for-the-badge&logoColor=E10600)
![MS Office](https://img.shields.io/badge/MS_Office-E10600?style=for-the-badge&logo=microsoftoffice&logoColor=white)


---

## 🚀 Featured Projects

### 🤖 KOOKIE v1 — Friendly Service Robot (SolidWorks)

A robot I designed from scratch: a compact 4-wheel body with an **LED screen face** that shows animated eyes and a smile. The upper body hinges open for easy access, and the screen is held with locks.

<div align="center">
  <img src="kookie-iso.png" width="48%" alt="Kookie v1 isometric view" />
  <img src="kookie-exploded.png" width="48%" alt="Kookie v1 exploded assembly" />
</div>

| Part | Qty | Part | Qty |
|------|-----|------|-----|
| Wheels | 4 | Upper Body | 1 |
| Wheel Grip (tyre) | 4 | Screen | 1 |
| Bottom | 1 | Lock | 2 |
| Shaft | 2 | | |

**Key specs:** body 250 × 250 mm, wheel Ø90 mm tyre on Ø66 mm rim, full drawings with dimensions for every part.

---

### 🔧 Industrial Valve Design — Pipeline & Check Valves

Designed valve bodies and full assemblies in SolidWorks: **reducing check valve, feed check valve, screw-down valve** and more. Gray cast iron body, flange-based pipeline design, full section drawings with BOM.

<div align="center">
  <img src="valve-body.png" width="48%" alt="Valve body drawing" />
  <img src="valve-body-section.png" width="48%" alt="Valve body section view" />
</div>

---

### 🏎️ Arduino Smart Car (Line Following • Obstacle Avoiding • Bluetooth)

Arduino UNO based smart car with:
- 🛣️ Line following using IR sensors
- 🚧 Obstacle avoiding using ultrasonic sensor
- 📱 Bluetooth control from phone

---

### 🕳️ Pipeline Defect Detection Robot

A robot concept that goes **inside pipes** and finds out where the defects are, combining mechanical design, robotics and practical problem-solving.

---

### 📐 More CAD Work

<div align="center">
  <img src="y-pipe-manifold.png" width="32%" alt="Y pipe manifold" />
  <img src="sheet-metal-bin.png" width="32%" alt="Sheet metal bin" />
  <img src="shaft-drawing.png" width="32%" alt="Shaft drawing" />
</div>

> ⚙️ Gear machines, big assemblies, sheet-metal parts, shafts and more. 🚀 **More projects coming soon...**

---

## 🏢 MechaFusion Technologies

My own engineering venture, focused on **mechanical design, robotics and automation**.
🌐 Website: *coming soon*

---

<!--
## 📊 GitHub Stats  (remove this comment tag after you have a few repos)
<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=TheMechaRonin&show_icons=true&theme=radical&hide_border=true" width="48%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=TheMechaRonin&theme=radical&hide_border=true" width="48%" />
</div>
-->

## 🤝 Connect With Me

<div align="center">

[![Email](https://img.shields.io/badge/Email-dhirendhall919@gmail.com-E10600?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dhirendhall919@gmail.com)
![Phone](https://img.shields.io/badge/Phone-8866079191-1a1a1a?style=for-the-badge&logo=whatsapp&logoColor=E10600)
[![GitHub](https://img.shields.io/badge/GitHub-TheMechaRonin-1a1a1a?style=for-the-badge&logo=github&logoColor=white)](https://github.com/TheMechaRonin)

![Profile Views](https://komarev.com/ghpvc/?username=TheMechaRonin&label=PROFILE+VIEWS&color=E10600&style=for-the-badge)

<br/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=16&duration=4000&pause=1500&color=E10600&center=true&vCenter=true&width=500&height=30&lines=%22Code+%E2%80%A2+Design+%E2%80%A2+Build+%E2%80%A2+Automate%22" alt="Tagline" />

</div>

## 💼 Services — Work With Me

> Need a design, a video or a prototype? **I take real work.** Message me and let's build it.

<table>
<tr>
<td width="50%" valign="top">

### 🎬 Video & Photo Editing
- Reels / short videos
- YouTube-style video edits
- Event, college and promo videos
- Photo editing and posters

**Tools of the trade:** video & photo editing software, clean cuts, good pacing.

</td>
<td width="50%" valign="top">

### 📐 CAD / CAM Design
- 2D drafting in **AutoCAD**
- 3D part and assembly modeling in **SolidWorks**
- Engineering drawings with dimensions and BOM
- Pipeline, valve, gear and sheet-metal designs

**Software:** SolidWorks • AutoCAD • Fusion 360 • Solid Edge

</td>
</tr>
<tr>
<td colspan="2" align="center">

### 🔌 Also: PCB Design & Arduino-based prototype help

</td>
</tr>
</table>

<div align="center">

[![WhatsApp](https://img.shields.io/badge/WhatsApp_Me-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/918866079191)
[![Email](https://img.shields.io/badge/Email_Me-E10600?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dhirendhall919@gmail.com)
[![Call](https://img.shields.io/badge/Call_8866079191-1a1a1a?style=for-the-badge&logo=phone&logoColor=E10600)](tel:+918866079191)

</div>

<div align="center"><img src="divider.svg" width="100%" alt="" /></div>

<div align="center"><img src="divider.svg" width="100%" alt="" /></div>

## 🏆 Achievements

### 🥈 Robo Fight — 2nd Place
Took part in a robot fight competition and finished **runner-up (2nd place)**.

<div align="center">
  <img src="robo-fight.jpg" width="40%" alt="Robo Fight arena" />
  <br/><sub>The Robo Fight arena</sub>
</div>

### 🎓 Robotics Workshop — Completed
**LAKSHYA CONNECT – Robotics Workshop**, presented by **Lakshya 2047 – Center for Future Skills, Parul University** (1–3 September 2026). Completed the full workshop and received the **Certificate of Participation**.

<div align="center">
  <img src="certificate-robotics-workshop.jpg" width="40%" alt="Robotics Workshop certificate" />
</div>

<div align="center"><img src="divider.svg" width="100%" alt="" /></div>


<div align="center"><img src="divider.svg" width="100%" alt="" /></div>


## 🧭 My Journey So Far

| Milestone | What I did |
|-----------|------------|
| 🚗 **Arduino Smart Car** | Line following, obstacle avoiding and Bluetooth control |
| 🕳️ **Pipeline Robot** | Designed a robot concept to find defects inside pipes |
| 🥈 **Robo Fight** | Competed and finished **2nd place** |
| 🎓 **Robotics Workshop** | Completed Lakshya Connect workshop, Parul University (Sep 2026) |
| 🤖 **Kookie v1** | Designed a full robot in SolidWorks with drawings for every part |
| 🏢 **MechaFusion Technologies** | Started my own company *(website coming soon)* |

<div align="center"><img src="divider.svg" width="100%" alt="" /></div>

## 🚧 Currently Working On

- 📚 Getting better at **Arduino C++ and Python**
- 🧩 Learning more **Fusion 360** and **PCB design**
- 🌐 Building the **MechaFusion Technologies** website
- 🤖 Goal: take **Kookie** from CAD design to a working robot

<!--
## 📊 GitHub Stats  (remove this comment tag after you have a few repos)
<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=TheMechaRonin&show_icons=true&theme=radical&hide_border=true" width="48%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=TheMechaRonin&theme=radical&hide_border=true" width="48%" />
</div>
-->

<div align="center"><img src="divider.svg" width="100%" alt="" /></div>

## 🤝 Let's Connect

<div align="center">

**Want a video edited, a part designed or a robot built? Message me.**

[![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/918866079191)
[![Email](https://img.shields.io/badge/Email-dhirendhall919@gmail.com-E10600?style=for-the-badge&logo=gmail&logoColor=white)](mailto:dhirendhall919@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-TheMechaRonin-1a1a1a?style=for-the-badge&logo=github&logoColor=white)](https://github.com/TheMechaRonin)

![Profile Views](https://komarev.com/ghpvc/?username=TheMechaRonin&label=PROFILE+VIEWS&color=E10600&style=for-the-badge)

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=16&duration=4000&pause=1500&color=E10600&center=true&vCenter=true&width=520&height=30&lines=%22Code+%E2%80%A2+Design+%E2%80%A2+Build+%E2%80%A2+Automate%22" alt="Tagline" />

<img src="divider.svg" width="100%" alt="" />

</div>
