<svg width="800" height="240" viewBox="0 0 800 240" xmlns="http://www.w3.org/2000/svg">
<defs>
  <clipPath id="clip"><rect width="800" height="240" rx="14"/></clipPath>
  <pattern id="gr" width="32" height="32" patternUnits="userSpaceOnUse">
    <path d="M32 0H0V32" fill="none" stroke="#00d2ff" stroke-width="0.4" stroke-opacity="0.07"/>
  </pattern>
  <linearGradient id="ng" x1="40" y1="0" x2="440" y2="0" gradientUnits="userSpaceOnUse">
    <stop offset="0%" stop-color="#00d4ff"/>
    <stop offset="100%" stop-color="#00ffb3"/>
  </linearGradient>
</defs>

<g clip-path="url(#clip)">

  <!-- Background -->
  <rect width="800" height="240" fill="#060c1a"/>
  <!-- Grid overlay -->
  <rect width="800" height="240" fill="url(#gr)"/>

  <!-- Glow orb top-left -->
  <ellipse cx="-10" cy="-10" rx="310" ry="260" fill="#00b4ff" fill-opacity="0.10">
    <animate attributeName="fill-opacity" values="0.07;0.14;0.07" dur="4s" repeatCount="indefinite"/>
  </ellipse>

  <!-- Glow orb bottom-right -->
  <ellipse cx="820" cy="255" rx="270" ry="210" fill="#00ffb3" fill-opacity="0.07">
    <animate attributeName="fill-opacity" values="0.04;0.10;0.04" dur="5s" repeatCount="indefinite"/>
  </ellipse>

  <!-- ═══ META (top right) ═══ -->
  <g opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="0.2s" dur="0.7s" fill="freeze"/>
    <text font-family="'Courier New',Courier,monospace" font-size="9" fill="#00d4ff" fill-opacity="0.4"
          text-anchor="end" letter-spacing="1.5" x="762" y="34">v2.0 — 2025</text>
    <text font-family="'Courier New',Courier,monospace" font-size="9" fill="#00d4ff" fill-opacity="0.4"
          text-anchor="end" letter-spacing="1.5" x="762" y="50">SRI LANKA</text>
  </g>

  <!-- ═══ TAG LINE ═══ -->
  <g opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="0.5s" dur="0.7s" fill="freeze"/>
    <line x1="40" y1="44" x2="62" y2="44" stroke="#00d4ff" stroke-width="1"/>
    <text font-family="'Courier New',Courier,monospace" font-size="10" font-weight="700"
          fill="#00d4ff" letter-spacing="2.5" x="70" y="49">PORTFOLIO · OPEN TO WORK</text>
  </g>

  <!-- ═══ NAME: Abheetha ═══ -->
  <text font-family="Arial,'Helvetica Neue',Helvetica,sans-serif" font-size="46" font-weight="900"
        fill="#ffffff" x="40" y="107" opacity="0">
    Abheetha
    <animate attributeName="opacity" from="0" to="1" begin="0.8s" dur="0.6s" fill="freeze"/>
  </text>

  <!-- ═══ NAME: Dhananjaya (gradient) ═══ -->
  <text font-family="Arial,'Helvetica Neue',Helvetica,sans-serif" font-size="46" font-weight="900"
        fill="url(#ng)" x="40" y="155" opacity="0">
    Dhananjaya
    <animate attributeName="opacity" from="0" to="1" begin="1.0s" dur="0.6s" fill="freeze"/>
  </text>

  <!-- ═══ ROLE CYCLING TEXT ═══ -->
  <!-- Role 1: QA Engineer  (0s – 3s) -->
  <text font-family="'Courier New',Courier,monospace" font-size="13" fill="#7a9bb5" x="40" y="178" opacity="1">
    QA Engineer
    <animate attributeName="opacity"
      values="1;1;0;0"
      keyTimes="0;0.208;0.25;1"
      dur="12s" repeatCount="indefinite"/>
  </text>

  <!-- Role 2: UI/UX Designer  (3s – 6s) -->
  <text font-family="'Courier New',Courier,monospace" font-size="13" fill="#7a9bb5" x="40" y="178" opacity="0">
    UI/UX Designer
    <animate attributeName="opacity"
      values="0;0;1;1;0;0"
      keyTimes="0;0.25;0.292;0.458;0.5;1"
      dur="12s" repeatCount="indefinite"/>
  </text>

  <!-- Role 3: Data Administrator  (6s – 9s) -->
  <text font-family="'Courier New',Courier,monospace" font-size="13" fill="#7a9bb5" x="40" y="178" opacity="0">
    Data Administrator
    <animate attributeName="opacity"
      values="0;0;1;1;0;0"
      keyTimes="0;0.5;0.542;0.708;0.75;1"
      dur="12s" repeatCount="indefinite"/>
  </text>

  <!-- Role 4: Bug Hunter  (9s – 12s) -->
  <text font-family="'Courier New',Courier,monospace" font-size="13" fill="#7a9bb5" x="40" y="178" opacity="0">
    Bug Hunter
    <animate attributeName="opacity"
      values="0;0;1;1;0"
      keyTimes="0;0.75;0.792;0.958;1"
      dur="12s" repeatCount="indefinite"/>
  </text>

  <!-- ═══ PILL 1: QA Engineering (cyan) ═══ -->
  <g opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="1.4s" dur="0.6s" fill="freeze"/>
    <rect x="40" y="194" width="118" height="22" rx="11"
          fill="#00d4ff" fill-opacity="0.07" stroke="#00d4ff" stroke-width="0.8" stroke-opacity="0.4"/>
    <text font-family="'Courier New',Courier,monospace" font-size="9" font-weight="700"
          letter-spacing="1" fill="#00d4ff" text-anchor="middle" x="99" y="209">QA ENGINEERING</text>
  </g>

  <!-- ═══ PILL 2: UI/UX Design (green) ═══ -->
  <g opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="1.6s" dur="0.6s" fill="freeze"/>
    <rect x="166" y="194" width="106" height="22" rx="11"
          fill="#00ffb3" fill-opacity="0.07" stroke="#00ffb3" stroke-width="0.8" stroke-opacity="0.4"/>
    <text font-family="'Courier New',Courier,monospace" font-size="9" font-weight="700"
          letter-spacing="1" fill="#00ffb3" text-anchor="middle" x="219" y="209">UI/UX DESIGN</text>
  </g>

  <!-- ═══ PILL 3: Data Administration (purple) ═══ -->
  <g opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="1.8s" dur="0.6s" fill="freeze"/>
    <rect x="280" y="194" width="148" height="22" rx="11"
          fill="#a78bff" fill-opacity="0.07" stroke="#a78bff" stroke-width="0.8" stroke-opacity="0.4"/>
    <text font-family="'Courier New',Courier,monospace" font-size="9" font-weight="700"
          letter-spacing="1" fill="#a78bff" text-anchor="middle" x="354" y="209">DATA ADMINISTRATION</text>
  </g>

  <!-- ═══ PILL 4: Quality Assurance (orange) ═══ -->
  <g opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="2.0s" dur="0.6s" fill="freeze"/>
    <rect x="436" y="194" width="138" height="22" rx="11"
          fill="#ff8c6b" fill-opacity="0.07" stroke="#ff8c6b" stroke-width="0.8" stroke-opacity="0.4"/>
    <text font-family="'Courier New',Courier,monospace" font-size="9" font-weight="700"
          letter-spacing="1" fill="#ff8c6b" text-anchor="middle" x="505" y="209">QUALITY ASSURANCE</text>
  </g>

  <!-- ═══ ANIMATED DOTS ═══ -->
  <circle cx="748" cy="207" r="3.5" fill="#00d4ff" opacity="0.25">
    <animate attributeName="opacity" values="0.25;1;0.25" dur="2s" repeatCount="indefinite"/>
    <animate attributeName="r" values="3.5;4.5;3.5" dur="2s" repeatCount="indefinite"/>
  </circle>
  <circle cx="760" cy="207" r="3.5" fill="#00ffb3" opacity="0.25">
    <animate attributeName="opacity" values="0.25;1;0.25" dur="2s" begin="0.4s" repeatCount="indefinite"/>
    <animate attributeName="r" values="3.5;4.5;3.5" dur="2s" begin="0.4s" repeatCount="indefinite"/>
  </circle>
  <circle cx="772" cy="207" r="3.5" fill="#a78bff" opacity="0.25">
    <animate attributeName="opacity" values="0.25;1;0.25" dur="2s" begin="0.8s" repeatCount="indefinite"/>
    <animate attributeName="r" values="3.5;4.5;3.5" dur="2s" begin="0.8s" repeatCount="indefinite"/>
  </circle>

</g>
</svg>

---

## 🧑‍💻 About Me

<table>
<tr>
<td width="50%">

### 🔍 Quality Assurance
Experienced in software testing methodologies, bug tracking, and automation tools. I ensure every product meets the highest reliability standards before it reaches users.

</td>
<td width="50%">

### 🎨 UI/UX Design
Skilled in wireframing, prototyping, and crafting user-friendly interfaces with **Figma** and **Adobe XD** — turning ideas into intuitive digital experiences.

</td>
</tr>
<tr>
<td width="50%">

### 📊 Data Administration
Proficient in database management, data validation, and ensuring data integrity using both SQL and NoSQL databases to keep systems accurate and reliable.

</td>
<td width="50%">

### 🌱 Currently Learning
Expanding into **usability testing**, **accessibility design (WCAG)**, **MobileNetV2**, and **transfer learning** techniques to build smarter, more inclusive products.

</td>
</tr>
</table>

---

## 🛠️ Tech Stack & Tools

### 💻 Programming Languages

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![C](https://img.shields.io/badge/C-A8B9CC?style=for-the-badge&logo=c&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)

</div>

---

### 🌐 Frontend & Mobile

<div align="center">

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)
![Adobe XD](https://img.shields.io/badge/Adobe_XD-FF61F6?style=for-the-badge&logo=adobexd&logoColor=white)

</div>

---

### 🗄️ Databases

<div align="center">

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)
![Apache Hive](https://img.shields.io/badge/Apache_Hive-FDEE21?style=for-the-badge&logo=apachehive&logoColor=black)

</div>

---

### ☁️ Cloud & DevOps

<div align="center">

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=FF9900)
![Azure](https://img.shields.io/badge/Microsoft_Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

</div>

---

### 🤖 AI / ML & Data Science

<div align="center">

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![MobileNetV2](https://img.shields.io/badge/MobileNetV2-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Transfer Learning](https://img.shields.io/badge/Transfer_Learning-00897B?style=for-the-badge&logo=tensorflow&logoColor=white)

</div>

---

### 🧰 Frameworks & Tools

<div align="center">

![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white)
![Jira](https://img.shields.io/badge/Jira-0052CC?style=for-the-badge&logo=jira&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ_IDEA-000000?style=for-the-badge&logo=intellijidea&logoColor=white)

</div>

---

## 📊 GitHub Stats

<div align="center">

<img src="https://streak-stats.demolab.com/?user=abheethasma&theme=tokyonight&hide_border=true&background=0d1117&stroke=00d4ff&ring=00d4ff&fire=ff6b6b&currStreakLabel=00d4ff" width="700"/>

</div>

<div align="center">

[![Abheetha's Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=abheethasma&bg_color=0d1117&color=00d4ff&line=00d4ff&point=ffffff&area=true&hide_border=true)](https://github.com/ashutosh00710/github-readme-activity-graph)

</div>

---

## 🏆 GitHub Trophies

---

## 🎯 Career Goal

> *"Seeking an opportunity to apply my skills in quality assurance, UI/UX, and data administration to improve product performance and user satisfaction. Let's connect and collaborate on building high-quality, user-centric solutions!"* 🚀

---

## 🤝 Connect With Me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abheetha-dhananjaya-419957282/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/abheethadhananjaya)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abheethasma)

</div>

---

<div align="center">

<img src="https://komarev.com/ghpvc/?username=abheethasma&label=Profile+Views&color=00d4ff&style=for-the-badge" alt="profile views" />

</div>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00d4ff,50:0e4d7a,100:0d1117&height=120&section=footer" />

</div>
