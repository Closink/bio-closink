<div align="center">

<!-- 1. АНИМИРОВАННЫЙ БАННЕР (HTML5 Canvas) -->
<canvas id="matrix-banner" width="800" height="200" style="border-radius:10px;margin-bottom:20px;"></canvas>
<script>
  const canvas = document.getElementById('matrix-banner');
  const ctx = canvas.getContext('2d');
  canvas.width = 800;
  canvas.height = 200;
  
  const katakana = 'アァカサタナハマヤャラワガザダバパイィキシチニヒミリヰギジヂビピウゥクスツヌフムユュルグズブヅプエェケセテネヘメレヱゲゼデベペオォコソトノホモヨョロヲゴゾドボポヴッン';
  const drops = Array(Math.floor(canvas.width/20)).fill(1);
  
  function draw() {
    ctx.fillStyle = 'rgba(0, 0, 0, 0.05)';
    ctx.fillRect(0, 0, canvas.width, canvas.height);
    ctx.fillStyle = '#0F0';
    ctx.font = '15px monospace';
    
    drops.forEach((y, i) => {
      const text = katakana[Math.floor(Math.random() * katakana.length)];
      ctx.fillText(text, i*20, y*20);
      drops[i] = y > canvas.height/20 || Math.random() > 0.95 ? 0 : y + 1;
    });
  }
  setInterval(draw, 50);
</script>

<!-- 2. ИНТЕРАКТИВНЫЕ КНОПКИ -->
<div class="buttons" style="display: flex; flex-wrap: wrap; gap: 10px; justify-content: center; margin: 20px 0;">
  <a href="https://t.me/+bNP53gq3IvI5MDcy" target="_blank" style="transition: all 0.3s;">
    <img src="https://img.shields.io/badge/💬_OSINT_Канал-26A5E4?style=for-the-badge&logo=telegram&logoColor=white&labelColor=000000" 
         onmouseover="this.style.transform='scale(1.1)';this.src='https://img.shields.io/badge/💬_OSINT_Канал-00FFFF?style=for-the-badge&logo=telegram&logoColor=black&labelColor=000000'" 
         onmouseout="this.style.transform='scale(1)';this.src='https://img.shields.io/badge/💬_OSINT_Канал-26A5E4?style=for-the-badge&logo=telegram&logoColor=white&labelColor=000000'"/>
  </a>
  <!-- Остальные кнопки с аналогичными эффектами -->
</div>

<!-- 3. 3D КАРТОЧКА (без геоданных) -->
<iframe src="https://my.spline.design/untitled-9a0b8b7e34640a1a24a4d5e5d8f1a1dc/" frameborder="0" width="100%" height="300"></iframe>

</div>

---

## **🚀 closink | CRXSS**
```python
class CyberResearcher:
    def __init__(self):
        self.name = "Closink or CR_XSS"
        self.skills = {
            'OSINT': ['Telegram Analysis', 'Blockchain Tracking', 'Image Geolocation'],
            'Tech': ['Python', 'SQL', 'TensorFlow'],
            'Creative': ['Data Art', 'Music Visualization']
        }
        self.current_project = " OSINT Framework"
    
    def __repr__(self):
        return f"{self.name} | {self.current_project}"

    def contact(self):
        return {
            "Telegram": "@CR_XSS",
            "Email": "closinknovivich@gmail.com",
            
        }

print(CyberResearcher())
