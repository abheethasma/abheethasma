<img width="1440" height="532" alt="image" src="https://github.com/user-attachments/assets/4bc1e734-c704-4313-87de-86599cf27e31" /><div align="center">

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Abheetha Dhananjaya — Header</title>
  <link href="https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Sora:wght@300;600;800&display=swap" rel="stylesheet"/>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: #03070f;
      display: flex;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      padding: 24px;
    }

    .hdr-root {
      background: #060c1a;
      border-radius: 16px;
      overflow: hidden;
      position: relative;
      min-height: 240px;
      width: 100%;
      max-width: 700px;
      font-family: 'Sora', sans-serif;
    }

    /* Animated grid background */
    .hdr-grid {
      position: absolute; inset: 0;
      background-image:
        linear-gradient(rgba(0,210,255,0.04) 1px, transparent 1px),
        linear-gradient(90deg, rgba(0,210,255,0.04) 1px, transparent 1px);
      background-size: 32px 32px;
      animation: gridShift 12s linear infinite;
    }
    @keyframes gridShift {
      from { background-position: 0 0; }
      to   { background-position: 32px 32px; }
    }

    /* Glow orbs */
    .hdr-glow {
      position: absolute;
      width: 340px; height: 340px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(0,180,255,0.13) 0%, transparent 70%);
      top: -80px; left: -60px;
      animation: pulse 4s ease-in-out infinite alternate;
      pointer-events: none;
    }
    .hdr-glow2 {
      position: absolute;
      width: 260px; height: 260px;
      border-radius: 50%;
      background: radial-gradient(circle, rgba(0,255,180,0.08) 0%, transparent 70%);
      bottom: -60px; right: -30px;
      animation: pulse 5s ease-in-out infinite alternate-reverse;
      pointer-events: none;
    }
    @keyframes pulse {
      from { opacity: 0.6; transform: scale(1); }
      to   { opacity: 1;   transform: scale(1.12); }
    }

    /* Main content area */
    .hdr-content {
      position: relative; z-index: 2;
      padding: 36px 40px 32px;
    }

    /* Top tag line */
    .hdr-tag {
      font-family: 'Space Mono', monospace;
      font-size: 11px;
      color: #00d4ff;
      letter-spacing: 0.18em;
      text-transform: uppercase;
      margin-bottom: 10px;
      opacity: 0;
      animation: fadeUp 0.5s ease forwards 0.3s;
      display: flex; align-items: center; gap: 8px;
    }
    .hdr-tag::before {
      content: '';
      display: inline-block; width: 24px; height: 1px;
      background: #00d4ff;
    }

    /* Name */
    .hdr-name {
      font-size: 42px;
      font-weight: 800;
      color: #ffffff;
      line-height: 1.1;
      margin: 0 0 6px;
      letter-spacing: -0.02em;
      opacity: 0;
      animation: fadeUp 0.6s ease forwards 0.55s;
    }
    .hdr-name span {
      background: linear-gradient(90deg, #00d4ff, #00ffb3);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      background-clip: text;
    }

    /* Typing roles */
    .hdr-roles {
      font-size: 15px;
      color: #7a9bb5;
      height: 24px;
      margin-bottom: 28px;
      font-family: 'Space Mono', monospace;
      opacity: 0;
      animation: fadeUp 0.6s ease forwards 0.8s;
    }
    .hdr-roles .cursor {
      color: #00d4ff;
      animation: blink 1s step-end infinite;
    }
    @keyframes blink { 50% { opacity: 0; } }

    /* Skill pills */
    .hdr-pills {
      display: flex; flex-wrap: wrap; gap: 8px;
      opacity: 0;
      animation: fadeUp 0.6s ease forwards 1.1s;
    }
    .hdr-pill {
      font-size: 11px;
      font-family: 'Space Mono', monospace;
      letter-spacing: 0.06em;
      padding: 5px 12px;
      border-radius: 999px;
      border: 1px solid;
      transition: all 0.2s;
      cursor: default;
    }
    .hdr-pill:hover {
      transform: translateY(-2px);
      box-shadow: 0 4px 16px rgba(0,212,255,0.2);
    }
    .p1 { color: #00d4ff; border-color: rgba(0,212,255,0.35);   background: rgba(0,212,255,0.07); }
    .p2 { color: #00ffb3; border-color: rgba(0,255,179,0.35);   background: rgba(0,255,179,0.07); }
    .p3 { color: #a78bff; border-color: rgba(167,139,255,0.35); background: rgba(167,139,255,0.07); }
    .p4 { color: #ff8c6b; border-color: rgba(255,140,107,0.35); background: rgba(255,140,107,0.07); }

    /* Corner meta info */
    .hdr-corner {
      position: absolute;
      top: 20px; right: 24px; z-index: 2;
      font-family: 'Space Mono', monospace;
      font-size: 10px;
      color: rgba(0,212,255,0.35);
      letter-spacing: 0.1em;
      opacity: 0;
      animation: fadeIn 1s ease forwards 1.4s;
    }
    .hdr-corner div { text-align: right; line-height: 1.8; }

    /* Animated dots */
    .hdr-dots {
      position: absolute;
      bottom: 18px; right: 24px; z-index: 2;
      display: flex; gap: 6px;
      opacity: 0;
      animation: fadeIn 1s ease forwards 1.6s;
    }
    .dot { width: 7px; height: 7px; border-radius: 50%; }
    .d1 { background: #00d4ff; animation: dotPulse 2s ease-in-out infinite; }
    .d2 { background: #00ffb3; animation: dotPulse 2s ease-in-out infinite 0.4s; }
    .d3 { background: #a78bff; animation: dotPulse 2s ease-in-out infinite 0.8s; }
    @keyframes dotPulse {
      0%,100% { opacity: 0.3; transform: scale(1); }
      50%     { opacity: 1;   transform: scale(1.3); }
    }

    /* Shared keyframes */
    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(12px); }
      to   { opacity: 1; transform: translateY(0); }
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to   { opacity: 1; }
    }

    /* Responsive */
    @media (max-width: 500px) {
      .hdr-name { font-size: 28px; }
      .hdr-content { padding: 28px 24px 24px; }
      .hdr-corner { display: none; }
    }
  </style>
</head>
<body>

  <div class="hdr-root">
    <div class="hdr-grid"></div>
    <div class="hdr-glow"></div>
    <div class="hdr-glow2"></div>

    <div class="hdr-corner">
      <div>v2.0 — 2025</div>
      <div>SRI LANKA 🇱🇰</div>
    </div>

    <div class="hdr-content">
      <div class="hdr-tag">Portfolio · Open to work</div>
      <div class="hdr-name">Abheetha<br><span>Dhananjaya</span></div>
      <div class="hdr-roles" id="roles"><span id="typed"></span><span class="cursor">|</span></div>
      <div class="hdr-pills">
        <span class="hdr-pill p1">QA Engineering</span>
        <span class="hdr-pill p2">UI/UX Design</span>
        <span class="hdr-pill p3">Data Administration</span>
        <span class="hdr-pill p4">Quality Assurance</span>
      </div>
    </div>

    <div class="hdr-dots">
      <div class="dot d1"></div>
      <div class="dot d2"></div>
      <div class="dot d3"></div>
    </div>
  </div>

  <script>
    const roles = ['QA Engineer', 'UI/UX Designer', 'Data Administrator', 'Bug Hunter 🐞'];
    let ri = 0, ci = 0, deleting = false;
    const el = document.getElementById('typed');

    function type() {
      const word = roles[ri];
      if (!deleting) {
        el.textContent = word.slice(0, ++ci);
        if (ci === word.length) {
          deleting = true;
          setTimeout(type, 1600);
          return;
        }
      } else {
        el.textContent = word.slice(0, --ci);
        if (ci === 0) {
          deleting = false;
          ri = (ri + 1) % roles.length;
        }
      }
      setTimeout(type, deleting ? 55 : 80);
    }

    setTimeout(type, 1400);
  </script>

</body>
</html>

<div align="center">

<!-- Typing SVG -->
[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&pause=1000&color=00D4FF&center=true&vCenter=true&random=false&width=620&lines=🔍+Quality+Assurance+Engineer;🎨+UI%2FUX+Designer+%26+Prototyper;📊+Data+Administrator+%26+Analyst;🚀+Open-Source+Contributor;⚡+Always+Learning%2C+Always+Building)](https://git.io/typing-svg)

</div>

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
