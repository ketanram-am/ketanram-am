<!-- ============================================================
     KETAN'S GITHUB README  —  ketanram-am
     ============================================================ -->
<svg width="600" height="300" viewBox="0 0 600 300" fill="none" xmlns="http://www.w3.org/2000/svg">
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Courier+Prime:wght@700&amp;display=swap');
    
    .bg { fill: #0d1117; rx: 16; }
    .text-header { font: 700 24px 'Courier Prime', monospace; fill: #e6edf3; letter-spacing: 4px; }
    .text-sub { font: 700 12px 'Courier Prime', monospace; fill: #58a6ff; letter-spacing: 2px; }
    
    /* Monitor Glow */
    .monitor-glow { fill: #58a6ff; opacity: 0.1; filter: blur(10px); animation: pulse 3s infinite; }
    @keyframes pulse { 0%, 100% { opacity: 0.05; } 50% { opacity: 0.15; } }

    /* Typing Animation */
    .code-line { fill: #3fb950; height: 4px; animation: type 4s steps(10) infinite; }
    @keyframes type { 0% { width: 0; } 50% { width: 100px; } 100% { width: 0; } }
    
    /* Steam Rising */
    .steam { fill: #58a6ff; opacity: 0; animation: steamRise 2s infinite; }
    @keyframes steamRise {
      0% { transform: translateY(0); opacity: 0; }
      50% { opacity: 0.4; }
      100% { transform: translateY(-15px); opacity: 0; }
    }

    /* Floating Particles */
    .particle { font: 10px monospace; fill: #d2a8ff; animation: float 5s infinite; }
    @keyframes float {
      0% { transform: translateY(0); opacity: 0; }
      20% { opacity: 0.6; }
      100% { transform: translateY(-60px); opacity: 0; }
    }
  </style>

  <!-- Background -->
  <rect width="600" height="300" class="bg" />

  <!-- Stars -->
  <circle cx="50" cy="40" r="1" fill="white" />
  <circle cx="550" cy="30" r="1.5" fill="white" />
  <circle cx="400" cy="60" r="1" fill="white" />
  <circle cx="100" cy="80" r="1" fill="white" />

  <!-- Header -->
  <text x="50%" y="50" text-anchor="middle" class="text-header">KETAN RAM</text>
  <text x="50%" y="75" text-anchor="middle" class="text-sub">[ FULLSTACK · AI · ML ]</text>

  <!-- Desk & Chair -->
  <rect x="200" y="240" width="200" height="8" fill="#1c2128" rx="2" /> <!-- Desk -->
  <rect x="210" y="248" width="6" height="30" fill="#1c2128" /> <!-- Leg L -->
  <rect x="384" y="248" width="6" height="30" fill="#1c2128" /> <!-- Leg R -->
  
  <rect x="275" y="210" width="50" height="50" fill="#21262d" rx="4" /> <!-- Chair Back -->

  <!-- Monitor Setup -->
  <circle cx="300" cy="160" r="60" class="monitor-glow" />
  <rect x="240" y="130" width="120" height="80" fill="#1f2b3e" stroke="#30363d" stroke-width="4" rx="4" />
  <rect x="250" y="140" width="100" height="60" fill="#0d1929" />
  
  <!-- Animated Code in Monitor -->
  <rect x="255" y="150" class="code-line" width="60" fill="#58a6ff" />
  <rect x="255" y="160" class="code-line" width="80" style="animation-delay: 0.5s" />
  <rect x="255" y="170" class="code-line" width="40" style="animation-delay: 1s" fill="#f78166" />

  <!-- Mug with Steam -->
  <rect x="360" y="225" width="15" height="15" fill="#21262d" rx="2" />
  <rect x="363" y="210" width="2" height="8" class="steam" />
  <rect x="370" y="210" width="2" height="8" class="steam" style="animation-delay: 0.7s" />

  <!-- Floating Syntax Particles -->
  <text x="210" y="200" class="particle" style="animation-delay: 0s;">{ }</text>
  <text x="380" y="180" class="particle" style="animation-delay: 1.5s; fill: #3fb950;">&lt;/&gt;</text>
  <text x="230" y="130" class="particle" style="animation-delay: 3s; fill: #ffa657;">fn()</text>

  <!-- Status Bar -->
  <rect x="150" y="270" width="300" height="20" fill="#161b22" rx="10" stroke="#21262d" />
  <circle cx="165" cy="280" r="4" fill="#3fb950">
    <animate attributeName="opacity" values="1;0.2;1" dur="1.5s" repeatCount="indefinite" />
  </circle>
  <text x="175" y="284" font-family="monospace" font-size="10" fill="#3fb950">CODING NOW...</text>
</svg>


<div align="center">

<!-- PIXEL ART: Man coding at desk (SVG) -->
<svg xmlns="http://www.w3.org/2000/svg" width="320" height="200" viewBox="0 0 320 200" style="image-rendering:pixelated">
  <!-- Dark room background -->
  <rect width="320" height="200" fill="#0d1117"/>
  <!-- Monitor glow -->
  <rect x="90" y="55" width="140" height="90" fill="#1a2233" rx="4"/>
  <rect x="95" y="60" width="130" height="80" fill="#0e1629"/>
  <!-- Code lines on screen -->
  <rect x="100" y="68" width="60" height="4" fill="#58a6ff" rx="1"/>
  <rect x="105" y="76" width="40" height="4" fill="#3fb950" rx="1"/>
  <rect x="105" y="84" width="50" height="4" fill="#f78166" rx="1"/>
  <rect x="105" y="92" width="35" height="4" fill="#d2a8ff" rx="1"/>
  <rect x="105" y="100" width="55" height="4" fill="#58a6ff" rx="1"/>
  <rect x="105" y="108" width="30" height="4" fill="#3fb950" rx="1"/>
  <!-- Cursor blink -->
  <rect x="137" y="108" width="3" height="4" fill="#e6edf3" rx="0.5">
    <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>
  </rect>
  <!-- Monitor stand -->
  <rect x="152" y="145" width="16" height="8" fill="#30363d"/>
  <rect x="140" y="153" width="40" height="4" fill="#30363d" rx="1"/>
  <!-- Desk -->
  <rect x="60" y="157" width="200" height="8" fill="#1c2128" rx="2"/>
  <rect x="70" y="165" width="6" height="30" fill="#1c2128"/>
  <rect x="244" y="165" width="6" height="30" fill="#1c2128"/>
  <!-- Keyboard -->
  <rect x="110" y="158" width="50" height="6" fill="#21262d" rx="1"/>
  <rect x="113" y="160" width="6" height="2" fill="#30363d" rx="0.5"/>
  <rect x="121" y="160" width="6" height="2" fill="#30363d" rx="0.5"/>
  <rect x="129" y="160" width="6" height="2" fill="#30363d" rx="0.5"/>
  <rect x="137" y="160" width="6" height="2" fill="#30363d" rx="0.5"/>
  <rect x="145" y="160" width="6" height="2" fill="#30363d" rx="0.5"/>
  <!-- Coffee mug -->
  <rect x="205" y="148" width="14" height="14" fill="#21262d" rx="2"/>
  <rect x="219" y="152" width="4" height="6" fill="none" stroke="#30363d" stroke-width="1.5"/>
  <rect x="207" y="150" width="10" height="3" fill="#3fb950" opacity="0.7" rx="1"/>
  <!-- Steam -->
  <path d="M210 148 Q211 144 210 140" stroke="#58a6ff" stroke-width="1" fill="none" opacity="0.5">
    <animate attributeName="opacity" values="0.5;0;0.5" dur="2s" repeatCount="indefinite"/>
  </path>
  <path d="M214 147 Q215 143 214 139" stroke="#58a6ff" stroke-width="1" fill="none" opacity="0.3">
    <animate attributeName="opacity" values="0.3;0;0.3" dur="2s" begin="0.5s" repeatCount="indefinite"/>
  </path>
  <!-- Person body -->
  <rect x="175" y="115" width="22" height="30" fill="#1f6feb" rx="3"/>
  <!-- Arms -->
  <rect x="163" y="118" width="12" height="8" fill="#1f6feb" rx="2"/>
  <rect x="197" y="118" width="12" height="8" fill="#1f6feb" rx="2"/>
  <!-- Hands -->
  <rect x="158" y="122" width="8" height="6" fill="#f0d9b5" rx="2"/>
  <rect x="205" y="122" width="8" height="6" fill="#f0d9b5" rx="2"/>
  <!-- Neck -->
  <rect x="182" y="108" width="8" height="8" fill="#f0d9b5" rx="1"/>
  <!-- Head -->
  <rect x="176" y="90" width="20" height="20" fill="#f0d9b5" rx="4"/>
  <!-- Hair -->
  <rect x="176" y="88" width="20" height="8" fill="#1a1008" rx="3"/>
  <rect x="176" y="90" width="4" height="6" fill="#1a1008"/>
  <!-- Eyes -->
  <rect x="180" y="96" width="3" height="3" fill="#1a1008" rx="1"/>
  <rect x="189" y="96" width="3" height="3" fill="#1a1008" rx="1"/>
  <!-- Glasses -->
  <rect x="178" y="95" width="7" height="5" fill="none" stroke="#58a6ff" stroke-width="1" rx="1"/>
  <rect x="187" y="95" width="7" height="5" fill="none" stroke="#58a6ff" stroke-width="1" rx="1"/>
  <rect x="185" y="97" width="2" height="1" fill="#58a6ff"/>
  <!-- Legs / chair -->
  <rect x="175" y="145" width="22" height="12" fill="#0d1117"/>
  <!-- Chair -->
  <rect x="168" y="143" width="36" height="6" fill="#21262d" rx="2"/>
  <rect x="168" y="149" width="4" height="20" fill="#21262d" rx="1"/>
  <rect x="200" y="149" width="4" height="20" fill="#21262d" rx="1"/>
  <!-- Bookshelf (right side) -->
  <rect x="262" y="90" width="40" height="65" fill="#1c2128" rx="2"/>
  <rect x="264" y="100" width="36" height="8" fill="#f78166" rx="1"/>
  <rect x="264" y="110" width="36" height="8" fill="#3fb950" rx="1"/>
  <rect x="264" y="120" width="36" height="8" fill="#58a6ff" rx="1"/>
  <rect x="264" y="130" width="36" height="8" fill="#d2a8ff" rx="1"/>
  <rect x="264" y="140" width="36" height="8" fill="#ffa657" rx="1"/>
  <!-- Plant (left side) -->
  <rect x="22" y="140" width="12" height="18" fill="#30363d" rx="1"/>
  <ellipse cx="28" cy="135" rx="14" ry="12" fill="#196127"/>
  <ellipse cx="20" cy="128" rx="8" ry="7" fill="#2ea043"/>
  <ellipse cx="36" cy="128" rx="8" ry="7" fill="#2ea043"/>
  <ellipse cx="28" cy="122" rx="7" ry="8" fill="#3fb950"/>
  <!-- Stars / particles -->
  <circle cx="45" cy="30" r="1" fill="#e6edf3" opacity="0.8"/>
  <circle cx="280" cy="20" r="1.5" fill="#58a6ff" opacity="0.6"/>
  <circle cx="15" cy="60" r="1" fill="#d2a8ff" opacity="0.7"/>
  <circle cx="300" cy="70" r="1" fill="#3fb950" opacity="0.5"/>
  <circle cx="250" cy="40" r="1" fill="#ffa657" opacity="0.6"/>
  <circle cx="70" cy="25" r="1.5" fill="#e6edf3" opacity="0.4"/>
</svg>

<!-- Animated typing headline -->
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=28&pause=1000&color=58A6FF&center=true&vCenter=true&width=600&lines=Hey+there!+I'm+Ketan+%F0%9F%91%BE;Fullstack+%7C+AI+%7C+ML+Developer;Building+Cool+Things+Every+Day;Always+Curious%2C+Always+Learning!" alt="Typing SVG" />

<br/>

<!-- Visitor badge + Profile views -->
[![](https://visitcount.itsvg.in/api?id=ketanram-am&icon=5&color=6)](https://visitcount.itsvg.in)
&nbsp;
![GitHub followers](https://img.shields.io/github/followers/ketanram-am?style=social)
&nbsp;
![Profile Views](https://komarev.com/ghpvc/?username=ketanram-am&color=58a6ff&style=flat-square&label=Profile+Views)

</div>

---

## 🧑‍💻 About Me

```javascript
const ketan = {
  name        : "Ketan Ram Amara",
  role        : "Fullstack + AI/ML Developer",
  location    : "India 🇮🇳",
  email       : "ketanramamara123@gmail.com",
  passion     : "Building projects that solve real problems",
  currentFocus: ["Making projects smarter", "Clean architecture", "AI integration"],
  funFact     : "I debug with chocolate ☕ and curiosity 🔍"
};
```

---

## 🚀 Tech Stack

### 💬 Languages
![Java](https://img.shields.io/badge/Java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/JavaScript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![C](https://img.shields.io/badge/C-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)

### ⚙️ Frameworks & Libraries
![React](https://img.shields.io/badge/React-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)
![Next JS](https://img.shields.io/badge/Next.js-black?style=for-the-badge&logo=next.js&logoColor=white)
![NodeJS](https://img.shields.io/badge/Node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Remix](https://img.shields.io/badge/Remix-%23000.svg?style=for-the-badge&logo=remix&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/Scikit--Learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)

### 🗄️ Databases & Cloud
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-%23000000.svg?style=for-the-badge&logo=netlify&logoColor=#00C7B7)

### 🛠️ Tools & Platforms
![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)
![NPM](https://img.shields.io/badge/NPM-%23CB3837.svg?style=for-the-badge&logo=npm&logoColor=white)
![Adobe Photoshop](https://img.shields.io/badge/Photoshop-%2331A8FF.svg?style=for-the-badge&logo=adobe%20photoshop&logoColor=white)

---

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=ketanram-am&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&show_icons=true&rank_icon=github" width="49%" alt="GitHub Stats"/>
<img src="https://nirzak-streak-stats.vercel.app/?user=ketanram-am&theme=tokyonight&hide_border=true" width="49%" alt="Streak Stats"/>

<br/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ketanram-am&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&layout=compact&langs_count=10" width="50%" alt="Top Languages"/>

</div>

---

## 🏆 GitHub Trophies

<div align="center">

![Trophies](https://github-profile-trophy.vercel.app/?username=ketanram-am&theme=tokyonight&no-frame=true&no-bg=true&margin-w=4&column=7)

</div>

---

## 📈 Contribution Graph

<div align="center">

![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=ketanram-am&theme=tokyo-night&hide_border=true&area=true)

</div>

---

## 🌐 Connect With Me

<div align="center">

[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ketanramamara123@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ketanram-am)

</div>

---

<div align="center">

```
   ██╗  ██╗███████╗████████╗ █████╗ ███╗   ██╗
   ██║ ██╔╝██╔════╝╚══██╔══╝██╔══██╗████╗  ██║
   █████╔╝ █████╗     ██║   ███████║██╔██╗ ██║
   ██╔═██╗ ██╔══╝     ██║   ██╔══██║██║╚██╗██║
   ██║  ██╗███████╗   ██║   ██║  ██║██║ ╚████║
   ╚═╝  ╚═╝╚══════╝   ╚═╝   ╚═╝  ╚═╝╚═╝  ╚═══╝
```

*"First, solve the problem. Then, write the code."*

⭐ **If you like my work, consider starring my repos!**

</div>
