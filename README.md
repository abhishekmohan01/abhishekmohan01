<div align="center">

<!DOCTYPE html>
<html>
<head>
<style>
* { margin: 0; padding: 0; box-sizing: border-box; }
body { 
  background: #0a0a0a; 
  color: white; 
  font-family: 'Fira Code', monospace; 
  overflow-x: hidden;
  position: relative;
}
#particles { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; }
.particle { 
  position: absolute; 
  width: 3px; height: 3px; 
  background: radial-gradient(circle, #667eea, transparent); 
  border-radius: 50%; 
  animation: float 8s infinite linear; 
}
@keyframes float { 
  0% { transform: translateY(100vh) scale(0) rotate(0deg); opacity: 1; }
  50% { opacity: 0.8; }
  100% { transform: translateY(-100px) scale(1) rotate(360deg); opacity: 0; }
}
.glow-text { 
  background: linear-gradient(45deg, #667eea, #764ba2, #f093fb, #f093fb 60%, #764ba2); 
  background-size: 300% 300%;
  -webkit-background-clip: text; 
  background-clip: text; 
  -webkit-text-fill-color: transparent;
  animation: gradientShift 4s ease infinite, glow 2s ease-in-out infinite alternate;
}
@keyframes gradientShift { 0%,100% { background-position: 0% 50%; } 50% { background-position: 100% 50%; } }
@keyframes glow { 0% { filter: drop-shadow(0 0 5px #667eea); } 100% { filter: drop-shadow(0 0 20px #f093fb); } }
.neon-line { height: 2px; background: linear-gradient(90deg, transparent, #667eea, #f093fb, transparent); animation: lineGlow 3s ease-in-out infinite; margin: 20px 0; }
@keyframes lineGlow { 0%,100% { width: 0; } 50% { width: 100%; } }
.glass-card { 
  background: rgba(255,255,255,0.08); 
  backdrop-filter: blur(20px); 
  border: 1px solid rgba(255,255,255,0.2); 
  border-radius: 24px; 
  padding: 30px; 
  transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  position: relative; overflow: hidden;
}
.glass-card::before { 
  content: ''; position: absolute; top: 0; left: -100%; width: 100%; height: 100%; 
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
  transition: left 0.6s;
}
.glass-card:hover::before { left: 100%; }
.glass-card:hover { 
  transform: translateY(-12px) scale(1.02); 
  box-shadow: 0 32px 64px rgba(102, 126, 234, 0.3);
  border-color: #667eea;
}
.orbit-container { 
  position: relative; height: 250px; 
  display: flex; align-items: center; justify-content: center;
}
.orbit { 
  position: absolute; 
  border: 2px solid rgba(102, 126, 234, 0.3); 
  border-radius: 50%;
  animation: rotate 20s linear infinite;
}
.orbit:nth-child(1) { width: 200px; height: 200px; animation-duration: 20s; }
.orbit:nth-child(2) { width: 280px; height: 280px; animation-duration: 25s; animation-direction: reverse; }
.orbit:nth-child(3) { width: 360px; height: 360px; animation-duration: 30s; }
@keyframes rotate { from { transform: rotate(0deg); } to { transform: rotate(360deg); } }
.skill-icon { 
  position: absolute; 
  font-size: 36px; 
  filter: drop-shadow(0 0 12px currentColor);
  animation: pulse 2s ease-in-out infinite;
}
@keyframes pulse { 0%,100% { transform: scale(1); } 50% { transform: scale(1.1); } }
</style>
</head>

<!-- 🌌 Particle Galaxy Background -->
<div id="particles"></div>

<!-- 🎬 Hero Section -->
<div style="padding: 60px 20px 20px;">
  <div style="text-align: center;">
    <h1 class="glow-text" style="font-size: clamp(2.5em, 8vw, 4.5em); margin-bottom: 12px; font-weight: 800;">
      Abhishek Mohan
    </h1>
    <div class="neon-line" style="max-width: 600px; margin: 0 auto 20px;"></div>
    <div class="glow-text" style="font-size: 1.4em; margin-bottom: 8px;">
      Multi-Domain Tech Engineer
    </div>
    <p style="opacity: 0.9; font-size: 1.1em; margin-bottom: 20px;">
      <span style="background: linear-gradient(45deg, #667eea, #f093fb); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
        Varanasi, India
      </span> | 
      BTech CSE @ LPU | Web + Android + ML + Data + Systems
    </p>
    
    <!-- ⌨️ Typing Animation -->
    <img src="https://readme-typing-svg.herokuapp.com/?lines=Full-Stack%20Web%20Dev%20%7C%20Android%20Apps%20%7C%20ML%20Fundamentals%20%7C%20Data%20Analytics%20%7C%20Cybersecurity%20Basics%20%7C%20Systems%20Engineer&font=Fira%20Code&size=26&pause=1500&center=true&vCenter=true&width=900&color=%23667eea" alt="Typing SVG" />
  </div>
</div>

<!-- 📈 GitHub Stats Galaxy -->
<div style="max-width: 1200px; margin: 0 auto; padding: 0 20px;">
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(420px, 1fr)); gap: 24px; margin: 40px 0;">
    <div class="glass-card">
      <img src="https://github-readme-stats.vercel.app/api?username=abhi-mohan&show_icons=true&theme=dark&hide_border=true&bg_color=0a0a0a&title_color=667eea&icon_color=f093fb&text_color=e1e1e1&hide=contribs,issues" width="100%"/>
    </div>
    <div class="glass-card">
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=abhi-mohan&layout=compact&theme=dark&hide_border=true&bg_color=0a0a0a&title_color=667eea&text_color=e1e1e1&hide=style,html,css" width="100%"/>
    </div>
  </div>
  <div class="glass-card" style="margin-top: 20px;">
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=abhi-mohan&theme=dark&hide_border=true&background=0a0a0a&stroke=667eea&ring=f093fb&currStreakNum=f093fb&currStreakLabel=764ba2&sideNums=667eea&sideLabels=f093fb&dates=f093fb" width="100%"/>
  </div>
</div>

<!-- 🚀 Featured Projects Showcase -->
<div style="max-width: 1200px; margin: 60px auto; padding: 0 20px;">
  <h2 class="glow-text" style="font-size: 2.8em; text-align: center; margin-bottom: 50px;">
    🚀 Featured Projects
  </h2>
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(380px, 1fr)); gap: 28px;">
    
    <div class="glass-card">
      <div style="font-size: 3em; text-align: center; margin-bottom: 20px;">🌤️</div>
      <h3 style="font-size: 1.6em; margin-bottom: 12px; color: #667eea;">
        PRODIGYWD05 Weather Dashboard
      </h3>
      <p style="margin-bottom: 20px; opacity: 0.9;">
        Advanced real-time weather app with dynamic UI, smooth animations, and responsive design
      </p>
      <div style="display: flex; gap: 10px; flex-wrap: wrap;">
        <span style="background: rgba(102,126,234,0.2); color: #667eea; padding: 6px 12px; border-radius: 20px; font-size: 0.85em;">HTML/CSS/JS</span>
        <span style="background: rgba(102,126,234,0.2); color: #667eea; padding: 6px 12px; border-radius: 20px; font-size: 0.85em;">Responsive</span>
        <span style="background: rgba(102,126,234,0.2); color: #667eea; padding: 6px 12px; border-radius: 20px; font-size: 0.85em;">Real-time</span>
      </div>
      [![View Repo](https://img.shields.io/badge/GitHub-View_Repo-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abhi-mohan/PRODIGYWD05--Weather-Web--)
    </div>

    <div class="glass-card">
      <div style="font-size: 3em; text-align: center; margin-bottom: 20px;">⏱️</div>
      <h3 style="font-size: 1.6em; margin-bottom: 12px; color: #f093fb;">
        PRODIGYWD02 Advanced Stopwatch
      </h3>
      <p style="margin-bottom: 20px; opacity: 0.9;">
        Feature-rich stopwatch with lap recording, session saving, and buttery-smooth animations
      </p>
      <div style="display: flex; gap: 10px; flex-wrap: wrap;">
        <span style="background: rgba(240,147,251,0.2); color: #f093fb; padding: 6px 12px; border-radius: 20px; font-size: 0.85em;">JavaScript</span>
        <span style="background: rgba(240,147,251,0.2); color: #f093fb; padding: 6px 12px; border-radius: 20px; font-size: 0.85em;">Animations</span>
        <span style="background: rgba(240,147,251,0.2); color: #f093fb; padding: 6px 12px; border-radius: 20px; font-size: 0.85em;">LocalStorage</span>
      </div>
      [![View Repo](https://img.shields.io/badge/GitHub-View_Repo-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abhi-mohan/PRODIGYWD02--Stopwatch--)
    </div>

    <div class="glass-card">
      <div style="font-size: 3em; text-align: center; margin-bottom: 20px;">🎮</div>
      <h3 style="font-size: 1.6em; margin-bottom: 12px; color: #764ba2;">
        PRODIGYWD03 Tic-Tac-Toe Pro
      </h3>
      <p style="margin-bottom: 20px; opacity: 0.9;">
        Interactive game engine with custom themes, multiple modes, and competitive gameplay
      </p>
      <div style="display: flex; gap: 10px; flex-wrap: wrap;">
        <span style="background: rgba(118,75,162,0.2); color: #764ba2; padding: 6px 12px; border-radius: 20px; font-size: 0.85em;">Game Logic</span>
        <span style="background: rgba(118,75,162,0.2); color: #764ba2; padding: 6px 12px; border-radius: 20px; font-size: 0.85em;">Themes</span>
        <span style="background: rgba(118,75,162,0.2); color: #764ba2; padding: 6px 12px; border-radius: 20px; font-size: 0.85em;">Multiplayer</span>
      </div>
      [![View Repo](https://img.shields.io/badge/GitHub-View_Repo-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/abhi-mohan/PRODIGYWD03--Tic-Tac-Toe--)
    </div>
  </div>
</div>

<!-- 🛠️ Orbiting Tech Stack -->
<div style="max-width: 800px; margin: 80px auto; padding: 0 20px;">
  <h2 class="glow-text" style="font-size: 2.6em; text-align: center; margin-bottom: 60px;">
    🛠️ Tech Arsenal
  </h2>
  <div class="orbit-container">
    <div class="orbit"></div>
    <div class="orbit"></div>
    <div class="orbit"></div>
    <img src="https://skillicons.dev/icons?i=html,css,js" style="top: 50%; left: 50%; transform: translate(-50%,-50%); position: absolute; width: 80px; color: #667eea;" class="skill-icon" data-color="#667eea"/>
    <img src="https://skillicons.dev/icons?i=git" style="top: 20%; left: 80%; position: absolute; width: 60px; color: #f093fb;" class="skill-icon" data-color="#f093fb"/>
    <img src="https://skillicons.dev/icons?i=excel" style="bottom: 30%; right: 20%; position: absolute; width: 55px; color: #764ba2;" class="skill-icon" data-color="#764ba2"/>
    <img src="https://skillicons.dev/icons?i=powerbi" style="top: 70%; right: 10%; position: absolute; width: 65px; color: #667eea;" class="skill-icon" data-color="#667eea"/>
    <img src="https://skillicons.dev/icons?i=tableau" style="bottom: 10%; left: 20%; position: absolute; width: 60px; color: #f093fb;" class="skill-icon" data-color="#f093fb"/>
  </div>
</div>

<!-- 🏆 Certifications & Connect -->
<div style="max-width: 1000px; margin: 60px auto; padding: 0 20px;">
  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px;">
    
    <div class="glass-card">
      <h3 style="font-size: 1.5em; margin-bottom: 20px; color: #667eea;">🏆 Certifications</h3>
      <div style="display: flex; flex-direction: column; gap: 12px;">
        <span style="display: flex; align-items: center; gap: 12px;">
          <div style="width: 12px; height: 12px; background: #667eea; border-radius: 50%;"></div>
          Responsive Web Design (freeCodeCamp)
        </span>
        <span style="display: flex; align-items: center; gap: 12px;">
          <div style="width: 12px; height: 12px; background: #f093fb; border-radius: 50%;"></div>
          Power BI (Microsoft)
        </span>
        <span style="display: flex; align-items: center; gap: 12px;">
          <div style="width: 12px; height: 12px; background: #764ba2; border-radius: 50%;"></div>
          Hardware/OS/Networking (IBM)
        </span>
      </div>
    </div>

    <div class="glass-card">
      <h3 style="font-size: 1.5em; margin-bottom: 25px; color: #f093fb;">📞 Let's Connect</h3>
      <div style="display: flex; flex-direction: column; gap: 16px;">
        [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/abhishek---mohan/)
        [![Email](https://img.shields.io/badge/Email-abhishek5489@outlook.com-black?style=for-the-badge&logo=microsoft-outlook&logoColor=white)](mailto:abhishek5489@outlook.com)
        [![Phone](https://img.shields.io/badge/Phone-8004638881-green?style=for-the-badge&logo=phone&logoColor=white)](tel:+918004638881)
      </div>
    </div>
  </div>
</div>

<!-- 💫 Philosophy -->
<div style="margin: 80px 20px; padding: 40px; background: rgba(255,255,255,0.02); border-radius: 28px; border: 1px solid rgba(102,126,234,0.3); text-align: center; backdrop-filter: blur(20px);">
  <div class="glow-text" style="font-size: 1.4em; font-style: italic; opacity: 0.95;">
    "Strong engineers understand systems end-to-end, not just frameworks. Cross-domain knowledge is critical in modern tech."
  </div>
</div>

<script>
// 🌌 Advanced Particle System
function createParticles() {
  const particles = document.getElementById('particles');
  for(let i = 0; i < 80; i++) {
    const particle = document.createElement('div');
    particle.className = 'particle';
    particle.style.left = Math.random() * 100 + '%';
    particle.style.animationDelay = Math.random() * 8 + 's';
    particle.style.animationDuration = (Math.random() * 4 + 6) + 's';
    particles.appendChild(particle);
  }
}
createParticles();

// 🎨 Dynamic Skill Colors
document.querySelectorAll('.skill-icon').forEach((icon, i) => {
  const colors = ['#667eea', '#f093fb', '#764ba2'];
  icon.style.color = colors[i % colors.length];
});
</script>

</html>

</div>
