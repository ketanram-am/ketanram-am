<!-- ============================================================
     KETAN'S GITHUB README  —  ketanram-am
     ============================================================ -->

<style>
  * { margin: 0; padding: 0; box-sizing: border-box; }
  body { background: transparent; }
  .scene {
    width: 100%;
    max-width: 680px;
    margin: 0 auto;
    background: #0d1117;
    border-radius: 16px;
    padding: 32px 24px 24px;
    font-family: 'Courier New', monospace;
    image-rendering: pixelated;
    position: relative;
    overflow: hidden;
  }
  .stars { position: absolute; top: 0; left: 0; width: 100%; height: 60px; }
  .star {
    position: absolute;
    width: 2px; height: 2px;
    background: #fff;
    animation: twinkle 2s infinite;
  }
  @keyframes twinkle { 0%,100%{opacity:.8} 50%{opacity:.1} }
  .room {
    display: flex;
    gap: 0;
    align-items: flex-end;
    justify-content: center;
    position: relative;
    margin-top: 20px;
  }

  /* === PIXEL ART SCENE (CSS boxes) === */
  .desk-area { display: flex; flex-direction: column; align-items: center; position: relative; }

  /* Monitor */
  .monitor-outer {
    width: 180px; height: 120px;
    background: #1f2b3e;
    border: 4px solid #30363d;
    border-radius: 4px;
    position: relative;
    display: flex; align-items: center; justify-content: center;
  }
  .monitor-screen {
    width: 160px; height: 100px;
    background: #0d1929;
    overflow: hidden;
    position: relative;
  }
  .monitor-glow {
    position: absolute; inset: -6px;
    background: rgba(56,139,253,.12);
    border-radius: 6px;
    animation: glow-pulse 3s ease-in-out infinite;
  }
  @keyframes glow-pulse { 0%,100%{opacity:.5} 50%{opacity:1} }

  /* Code lines on screen */
  .code-area { padding: 8px 10px; }
  .code-line {
    height: 6px; border-radius: 2px; margin-bottom: 5px;
    animation: type-in 4s steps(1) infinite;
  }
  .l1 { width: 0px; background:#58a6ff; animation-delay: 0s; }
  .l2 { width: 0px; background:#3fb950; animation-delay: .4s; }
  .l3 { width: 0px; background:#f78166; animation-delay: .8s; }
  .l4 { width: 0px; background:#d2a8ff; animation-delay: 1.2s; }
  .l5 { width: 0px; background:#58a6ff; animation-delay: 1.6s; }
  .l6 { width: 0px; background:#3fb950; animation-delay: 2.0s; }
  .l7 { width: 0px; background:#ffa657; animation-delay: 2.4s; }
  .l8 { width: 0px; background:#d2a8ff; animation-delay: 2.8s; }
  @keyframes type-in {
    0%   { width: 0px }
    10%  { width: 30px }
    30%  { width: 70px }
    60%  { width: 100px }
    90%  { width: 130px }
    100% { width: 130px }
  }
  .cursor-blink {
    display: inline-block;
    width: 4px; height: 8px;
    background: #e6edf3;
    margin-left: 2px;
    animation: blink .7s steps(1) infinite;
    vertical-align: bottom;
  }
  @keyframes blink { 0%,49%{opacity:1} 50%,100%{opacity:0} }

  /* Monitor stand */
  .monitor-stand {
    width: 20px; height: 12px;
    background: #30363d;
    margin: 0 auto;
  }
  .monitor-base {
    width: 60px; height: 6px;
    background: #30363d;
    border-radius: 2px;
    margin: 0 auto;
  }

  /* Desk */
  .desk {
    width: 340px; height: 10px;
    background: #1c2128;
    border-radius: 3px;
    margin-top: 0;
    position: relative;
    box-shadow: 0 4px 0 #161b22;
  }
  .desk-leg {
    position: absolute;
    bottom: -30px;
    width: 8px; height: 30px;
    background: #1c2128;
  }
  .leg-l { left: 20px; }
  .leg-r { right: 20px; }

  /* Keyboard */
  .keyboard {
    position: absolute;
    top: -14px; left: 105px;
    width: 80px; height: 10px;
    background: #21262d;
    border-radius: 2px;
    display: flex; gap: 2px; align-items: center; justify-content: center;
    padding: 2px 4px;
  }
  .key {
    width: 8px; height: 5px;
    background: #30363d;
    border-radius: 1px;
    animation: key-press 4s infinite;
  }
  .key:nth-child(2) { animation-delay: .15s; }
  .key:nth-child(3) { animation-delay: .3s; }
  .key:nth-child(4) { animation-delay: .45s; }
  .key:nth-child(5) { animation-delay: .6s; }
  @keyframes key-press { 0%,95%,100%{transform:translateY(0);background:#30363d} 97%{transform:translateY(1px);background:#58a6ff} }

  /* Coffee mug */
  .mug-wrap {
    position: absolute;
    top: -30px; right: 28px;
  }
  .mug {
    width: 18px; height: 18px;
    background: #21262d;
    border-radius: 2px;
    border: 2px solid #30363d;
    position: relative;
  }
  .mug-liquid {
    position: absolute; top: 2px; left: 2px;
    width: 10px; height: 4px;
    background: #3fb950;
    border-radius: 1px;
    opacity: .7;
  }
  .mug-handle {
    position: absolute; right: -5px; top: 3px;
    width: 5px; height: 8px;
    border: 2px solid #30363d;
    border-left: none;
    border-radius: 0 3px 3px 0;
  }
  .steam {
    position: absolute; bottom: 100%; left: 3px;
    display: flex; gap: 4px;
  }
  .steam span {
    width: 2px; height: 10px;
    background: linear-gradient(to top, #58a6ff66, transparent);
    border-radius: 2px;
    animation: steam-rise 1.5s ease-out infinite;
  }
  .steam span:nth-child(2) { animation-delay: .5s; }
  @keyframes steam-rise { 0%{opacity:.8;transform:translateY(0) scaleX(1)} 100%{opacity:0;transform:translateY(-12px) scaleX(1.5)} }

  /* Person (pixel art via CSS) */
  .person {
    position: absolute;
    bottom: 0;
    left: 50%;
    transform: translateX(-50%);
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  /* Head */
  .head {
    width: 28px; height: 28px;
    background: #f0c896;
    border-radius: 4px;
    position: relative;
    margin-bottom: 0;
  }
  .hair {
    position: absolute; top: 0; left: 0;
    width: 28px; height: 10px;
    background: #1a1008;
    border-radius: 4px 4px 0 0;
  }
  .glasses {
    position: absolute; top: 12px; left: 2px;
    display: flex; gap: 3px;
  }
  .glass-frame {
    width: 10px; height: 7px;
    border: 1.5px solid #58a6ff;
    border-radius: 2px;
    background: rgba(88,166,255,.08);
  }
  .glass-bridge {
    width: 3px; height: 1.5px;
    background: #58a6ff;
    align-self: center;
    margin-top: 2px;
  }
  .mouth {
    position: absolute; bottom: 4px; left: 8px;
    width: 12px; height: 3px;
    border-bottom: 2px solid #c0906a;
    border-radius: 0 0 4px 4px;
  }

  /* Body */
  .body {
    width: 36px; height: 40px;
    background: #1f6feb;
    border-radius: 3px;
    position: relative;
  }
  .shirt-detail {
    position: absolute; top: 6px; left: 50%; transform: translateX(-50%);
    width: 4px; height: 16px;
    background: rgba(255,255,255,.15);
    border-radius: 1px;
  }
  .arm {
    position: absolute; top: 6px;
    width: 16px; height: 10px;
    background: #1f6feb;
    border-radius: 3px;
    animation: type-arms .3s ease-in-out infinite alternate;
  }
  .arm-l { left: -14px; }
  .arm-r { right: -14px; }
  @keyframes type-arms { 0%{transform:translateY(0)} 100%{transform:translateY(2px)} }
  .hand {
    position: absolute; bottom: -6px;
    width: 12px; height: 8px;
    background: #f0c896;
    border-radius: 2px;
  }
  .hand-l { left: -14px; bottom: -20px; }
  .hand-r { right: -14px; bottom: -20px; }

  /* Chair */
  .chair-back {
    width: 44px; height: 46px;
    background: #21262d;
    border-radius: 4px 4px 0 0;
    position: absolute;
    bottom: 0;
    z-index: -1;
    border: 2px solid #30363d;
  }
  .chair-seat {
    position: absolute;
    bottom: 0; left: -4px;
    width: 52px; height: 10px;
    background: #30363d;
    border-radius: 3px;
  }
  .chair-pole {
    position: absolute; bottom: -20px; left: 50%; transform: translateX(-50%);
    width: 6px; height: 22px;
    background: #21262d;
  }
  .chair-base {
    position: absolute; bottom: -24px; left: 50%; transform: translateX(-50%);
    width: 40px; height: 5px;
    background: #30363d;
    border-radius: 2px;
  }

  /* Bookshelf */
  .bookshelf {
    width: 50px;
    background: #1c2128;
    border-radius: 3px;
    padding: 6px 4px;
    display: flex;
    flex-direction: column;
    gap: 3px;
    border: 2px solid #30363d;
    margin-left: 16px;
    align-self: flex-start;
    margin-top: 30px;
  }
  .book {
    height: 12px;
    border-radius: 1px;
  }

  /* Plant */
  .plant-wrap {
    display: flex; flex-direction: column; align-items: center;
    margin-right: 16px;
    align-self: flex-end;
  }
  .plant-pot {
    width: 24px; height: 18px;
    background: #8b4513;
    border-radius: 0 0 4px 4px;
    clip-path: polygon(10% 0%, 90% 0%, 100% 100%, 0% 100%);
  }
  .plant-dirt {
    width: 28px; height: 5px;
    background: #3d2010;
    border-radius: 2px;
    margin-top: -2px;
  }
  .leaf {
    background: #2ea043;
    border-radius: 50%;
    animation: sway 3s ease-in-out infinite;
    transform-origin: bottom center;
  }
  .leaf-l { width: 20px; height: 16px; transform: rotate(-30deg) translateX(-4px); }
  .leaf-c { width: 18px; height: 22px; transform: translateY(-4px); background: #3fb950; }
  .leaf-r { width: 20px; height: 16px; transform: rotate(30deg) translateX(4px); }
  @keyframes sway { 0%,100%{transform:rotate(-2deg)} 50%{transform:rotate(2deg)} }

  /* Floating code particles */
  .particle {
    position: absolute;
    font-size: 11px;
    font-family: monospace;
    color: #3fb950;
    opacity: 0;
    animation: float-up 5s ease-out infinite;
    pointer-events: none;
  }
  @keyframes float-up {
    0% { opacity:0; transform: translateY(0) }
    15% { opacity:.8 }
    100% { opacity:0; transform: translateY(-80px) }
  }

  /* Info strip */
  .info-strip {
    margin-top: 24px;
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
    justify-content: center;
  }
  .badge {
    padding: 4px 12px;
    border-radius: 20px;
    font-size: 12px;
    font-family: 'Courier New', monospace;
    border: 1px solid;
    animation: badge-glow 3s ease-in-out infinite;
  }
  @keyframes badge-glow { 0%,100%{opacity:.8} 50%{opacity:1} }

  /* Status bar */
  .status-bar {
    margin-top: 16px;
    background: #161b22;
    border-radius: 6px;
    padding: 8px 16px;
    display: flex;
    align-items: center;
    gap: 12px;
    font-size: 12px;
    color: #8b949e;
    font-family: 'Courier New', monospace;
    border: 1px solid #21262d;
  }
  .status-dot {
    width: 8px; height: 8px;
    border-radius: 50%;
    background: #3fb950;
    animation: pulse-dot 1.5s ease-in-out infinite;
  }
  @keyframes pulse-dot { 0%,100%{box-shadow:0 0 0 0 #3fb95066} 50%{box-shadow:0 0 0 4px #3fb95022} }
  .status-text { color: #3fb950; }
  .spacer { flex: 1; }
  .blink-cursor { animation: blink .7s steps(1) infinite; color: #58a6ff; }

  /* Name header */
  .name-header {
    text-align: center;
    margin-bottom: 20px;
  }
  .name-header h1 {
    font-size: 22px;
    font-weight: 700;
    color: #e6edf3;
    font-family: 'Courier New', monospace;
    letter-spacing: 4px;
  }
  .name-header p {
    font-size: 12px;
    color: #58a6ff;
    letter-spacing: 2px;
    margin-top: 4px;
  }
</style>

<div class="scene">

  <!-- Stars -->
  <div class="stars" id="stars"></div>

  <!-- Name -->
  <div class="name-header">
    <h1>KETAN RAM</h1>
    <p>[ FULLSTACK · AI · ML ]</p>
  </div>

  <!-- Main scene -->
  <div class="room">

    <!-- Plant -->
    <div class="plant-wrap">
      <div style="display:flex; align-items:flex-end; height:50px;">
        <div class="leaf leaf-l"></div>
        <div class="leaf leaf-c"></div>
        <div class="leaf leaf-r"></div>
      </div>
      <div class="plant-dirt"></div>
      <div class="plant-pot"></div>
    </div>

    <!-- Desk + monitor + person -->
    <div class="desk-area">
      <!-- Monitor glow -->
      <div style="position:relative; display:inline-block;">
        <div class="monitor-glow"></div>
        <div class="monitor-outer">
          <div class="monitor-screen">
            <div class="code-area" id="codeArea">
              <div class="code-line l1"></div>
              <div class="code-line l2" style="margin-left:12px"></div>
              <div class="code-line l3" style="margin-left:12px"></div>
              <div class="code-line l4" style="margin-left:24px"></div>
              <div class="code-line l5" style="margin-left:12px"></div>
              <div class="code-line l6" style="margin-left:24px"></div>
              <div class="code-line l7" style="margin-left:12px"></div>
              <div class="code-line l8"></div>
              <div style="margin-top:4px; padding-left:2px;">
                <span class="cursor-blink"></span>
              </div>
            </div>
          </div>
        </div>
      </div>

      <div class="monitor-stand"></div>
      <div class="monitor-base"></div>

      <!-- Desk -->
      <div class="desk" style="position:relative; margin-top:0;">
        <div class="desk-leg leg-l"></div>
        <div class="desk-leg leg-r"></div>
        <!-- Keyboard -->
        <div class="keyboard">
          <div class="key"></div>
          <div class="key"></div>
          <div class="key"></div>
          <div class="key"></div>
          <div class="key"></div>
        </div>
        <!-- Mug -->
        <div class="mug-wrap">
          <div class="steam"><span></span><span></span></div>
          <div class="mug">
            <div class="mug-liquid"></div>
            <div class="mug-handle"></div>
          </div>
        </div>

        <!-- Person sitting -->
        <div style="position:absolute; bottom:10px; left:50%; transform:translateX(-50%); display:flex; flex-direction:column; align-items:center;">
          <!-- Chair back -->
          <div style="position:relative;">
            <div class="chair-back">
              <div class="chair-seat"></div>
              <div class="chair-pole"></div>
              <div class="chair-base"></div>
            </div>
            <!-- Body -->
            <div class="body" style="position:absolute; top:2px; left:4px;">
              <div class="shirt-detail"></div>
              <div class="arm arm-l"></div>
              <div class="arm arm-r"></div>
              <div class="hand hand-l"></div>
              <div class="hand hand-r"></div>
            </div>
            <!-- Head -->
            <div class="head" style="position:absolute; top:-30px; left:8px;">
              <div class="hair"></div>
              <div class="glasses">
                <div class="glass-frame"></div>
                <div class="glass-bridge"></div>
                <div class="glass-frame"></div>
              </div>
              <div class="mouth"></div>
            </div>
          </div>
        </div>

      </div><!-- /desk -->
    </div><!-- /desk-area -->

    <!-- Bookshelf -->
    <div class="bookshelf">
      <div class="book" style="background:#f78166"></div>
      <div class="book" style="background:#3fb950"></div>
      <div class="book" style="background:#58a6ff"></div>
      <div class="book" style="background:#d2a8ff"></div>
      <div class="book" style="background:#ffa657"></div>
      <div class="book" style="background:#f78166; width:70%"></div>
      <div class="book" style="background:#58a6ff; width:80%"></div>
    </div>

  </div><!-- /room -->

  <!-- Floating particles -->
  <div id="particles" style="position:absolute; top:60px; left:0; width:100%; height:200px; pointer-events:none; overflow:hidden;"></div>

  <!-- Badge strip -->
  <div class="info-strip">
    <div class="badge" style="color:#58a6ff; border-color:#1f3b5e; background:#0d1f30;">⬡ React</div>
    <div class="badge" style="color:#3fb950; border-color:#1a3a20; background:#0d1e10; animation-delay:.3s;">⬡ Node.js</div>
    <div class="badge" style="color:#f78166; border-color:#3d1f18; background:#1e0f0a; animation-delay:.6s;">⬡ Java</div>
    <div class="badge" style="color:#d2a8ff; border-color:#2d1f4a; background:#160e26; animation-delay:.9s;">⬡ Python</div>
    <div class="badge" style="color:#ffa657; border-color:#3d2a10; background:#1e1408; animation-delay:1.2s;">⬡ Javascript</div>
    <div class="badge" style="color:#58a6ff; border-color:#1f3b5e; background:#0d1f30; animation-delay:1.5s;">⬡ MongoDB</div>
  </div>

  <!-- Status bar -->
  <div class="status-bar">
    <div class="status-dot"></div>
    <span class="status-text">CODING NOW</span>
    <span>ketanram-am</span>
    <div class="spacer"></div>
    <span id="liveTime" style="color:#8b949e;"></span>
    <span class="blink-cursor">█</span>
  </div>

</div>

<script>
  const starEl = document.getElementById('stars');
  for(let i=0;i<28;i++){
    const s=document.createElement('div');
    s.className='star';
    s.style.left=Math.random()*100+'%';
    s.style.top=Math.random()*100+'%';
    s.style.animationDelay=Math.random()*3+'s';
    s.style.animationDuration=(1.5+Math.random()*2.5)+'s';
    if(Math.random()>.7){s.style.width='3px';s.style.height='3px';}
    starEl.appendChild(s);
  }

  const codes=['{ }','</>','fn()','=>','.map','async','null','0x1F','[]','&&','!==','try'];
  const px=document.getElementById('particles');
  function spawnParticle(){
    const p=document.createElement('div');
    p.className='particle';
    p.textContent=codes[Math.floor(Math.random()*codes.length)];
    p.style.left=(20+Math.random()*60)+'%';
    p.style.bottom='0';
    p.style.animationDuration=(3+Math.random()*3)+'s';
    p.style.animationDelay='0s';
    p.style.color=['#3fb950','#58a6ff','#d2a8ff','#ffa657'][Math.floor(Math.random()*4)];
    px.appendChild(p);
    setTimeout(()=>p.remove(),6000);
  }
  setInterval(spawnParticle,900);

  function updateTime(){
    const t=document.getElementById('liveTime');
    if(t){
      const n=new Date();
      t.textContent=n.toLocaleTimeString('en-IN',{hour:'2-digit',minute:'2-digit',second:'2-digit'});
    }
  }
  setInterval(updateTime,1000);
  updateTime();
</script>

<div align="center">

<!-- Animated typing headline -->
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=30&pause=1000&color=58A6FF&center=true&vCenter=true&width=700&lines=Hey+there!+I'm+Ketan+%F0%9F%91%BE;Fullstack+%7C+AI+%7C+ML+Developer;Building+Cool+Things+Every+Day;Always+Curious%2C+Always+Learning!" alt="Typing SVG" />

<br/><br/>

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
  name        : "Ketan Ramamara",
  role        : "Fullstack + AI/ML Developer",
  location    : "India 🇮🇳",
  email       : "ketanramamara123@gmail.com",
  passion     : "Building projects that solve real problems",
  currentFocus: ["Making projects smarter", "Clean architecture", "AI integration"],
  funFact     : "I debug with coffee ☕ and curiosity 🔍"
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

### 🛠️ Tools
![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=JSON%20web%20tokens)
![NPM](https://img.shields.io/badge/NPM-%23CB3837.svg?style=for-the-badge&logo=npm&logoColor=white)
![Adobe Photoshop](https://img.shields.io/badge/Photoshop-%2331A8FF.svg?style=for-the-badge&logo=adobe%20photoshop&logoColor=white)

---

## 📊 GitHub Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=ketanram-am&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&show_icons=true&rank_icon=github" width="49%" />
<img src="https://nirzak-streak-stats.vercel.app/?user=ketanram-am&theme=tokyonight&hide_border=true" width="49%" />

<br/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ketanram-am&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&layout=compact&langs_count=10" width="50%" />

</div>

---

## 🏆 Trophies

<div align="center">

![Trophies](https://github-profile-trophy.vercel.app/?username=ketanram-am&theme=tokyonight&no-frame=true&no-bg=true&margin-w=4&column=7)

</div>

---

## 🐍 Contribution Snake

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/ketanram-am/ketanram-am/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/ketanram-am/ketanram-am/output/github-snake.svg" />
  <img alt="github-snake" src="https://raw.githubusercontent.com/ketanram-am/ketanram-am/output/github-snake.svg" />
</picture>

> 💡 Enable this by adding the [Platane/snk](https://github.com/Platane/snk) GitHub Action to your profile repo.

</div>

---

## 🌐 Connect

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

⭐ **Star my repos if you like my work!**

</div>
