# 🎨 Quick Customization Snippets

Copy & paste these snippets to quickly customize your profile!

---

## 🔤 Change Your Name

### In SVG Files (Both Dark & Light)
Find this block and replace `AYUSH RAI` with your name:

```xml
<tspan x="60" dy="0">  ╔═══════════════╗</tspan>
<tspan x="60" dy="20">  ║  AYUSH RAI    ║</tspan>
<tspan x="60" dy="20">  ║  Developer    ║</tspan>
<tspan x="60" dy="20">  ║  Builder      ║</tspan>
<tspan x="60" dy="20">  ║  Engineer     ║</tspan>
<tspan x="60" dy="20">  ╚═══════════════╝</tspan>
```

**Adjust box width if name is longer:**
Change `width="70"` in the rectangles to fit your name

---

## 💼 Job Titles Configuration

### All 3 Rotating Titles (12-second cycle)

```xml
<!-- TITLE 1: Shows 0-3 seconds -->
<text x="510" y="135" font-family="'Segoe UI', Arial, sans-serif" font-size="24" font-weight="600" fill="url(#titleGradient)">
  <tspan id="title1" opacity="1">
    🚀 Full Stack Developer
    <animate attributeName="opacity" values="1;1;1;0;0" dur="12s" repeatCount="indefinite"/>
  </tspan>
</text>

<!-- TITLE 2: Shows 3-9 seconds -->
<text x="510" y="135" font-family="'Segoe UI', Arial, sans-serif" font-size="24" font-weight="600" fill="url(#titleGradient)">
  <tspan opacity="0">
    💡 Open Source Enthusiast
    <animate attributeName="opacity" values="0;0;1;1;0" dur="12s" repeatCount="indefinite"/>
  </tspan>
</text>

<!-- TITLE 3: Shows 9-12 seconds -->
<text x="510" y="135" font-family="'Segoe UI', Arial, sans-serif" font-size="24" font-weight="600" fill="url(#titleGradient)">
  <tspan opacity="0">
    ⚡ Problem Solver
    <animate attributeName="opacity" values="0;0;0;0;1" dur="12s" repeatCount="indefinite"/>
  </tspan>
</text>
```

### Quick Examples to Replace:
```
🚀 Full Stack Developer
💡 Software Engineer  
⚡ DevOps Engineer
🤖 ML Engineer
📱 Mobile Developer
🎮 Game Developer
🎨 UI/UX Designer
💼 Technical Lead
🔐 Security Engineer
☁️ Cloud Architect
```

---

## 📊 Tech Stack Badges

### Popular Tech Badges with Colors

```markdown
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8936?style=for-the-badge&logo=java&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=for-the-badge&logo=vue.js&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-13AA52?style=for-the-badge&logo=mongodb&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)

![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=FF9900)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![GitLab](https://img.shields.io/badge/GitLab-FCA121?style=for-the-badge&logo=gitlab&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)
![Notion](https://img.shields.io/badge/Notion-000000?style=for-the-badge&logo=notion&logoColor=white)
```

---

## 🎯 Project Template

### Copy-Paste Project Section

```markdown
### 🔵 **Project Name**
Brief description of what it does | Key metrics or numbers
🛠️ `Tech1` `Tech2` `Tech3` `Tech4`  
📊 [Repo →](https://github.com/yourname/project)

---

### 🟢 **Another Project**  
What makes it special | Impact or usage stats
🛠️ `Stack1` `Stack2` `Stack3`  
📊 [Repo →](https://github.com/yourname/project2)
```

### Example Projects

```markdown
### 🎮 **Game Engine**
C++ graphics engine with Vulkan | 60 FPS rendering
🛠️ `C++` `Vulkan` `OpenGL` `Physics`  
📊 [Repo →](https://github.com/user/gameengine)

---

### 🤖 **ML Recommendation System**
E-commerce recommendation engine | 95% accuracy
🛠️ `Python` `TensorFlow` `FastAPI` `PostgreSQL`  
📊 [Repo →](https://github.com/user/rec-system)

---

### 📱 **Mobile App**
Cross-platform app with 50K+ downloads
🛠️ `React Native` `Firebase` `Redux`  
📊 [Repo →](https://github.com/user/mobile-app)
```

---

## 🌈 Color Scheme Presets

### Dark Mode Gradients

**Purple-Cyan-Green (Default)**
```xml
<stop offset="0%" style="stop-color:#7c3aed;stop-opacity:1"/>
<stop offset="50%" style="stop-color:#22d3ee;stop-opacity:1"/>
<stop offset="100%" style="stop-color:#10b981;stop-opacity:1"/>
```

**Blue-Pink-Purple**
```xml
<stop offset="0%" style="stop-color:#3b82f6;stop-opacity:1"/>
<stop offset="50%" style="stop-color:#ec4899;stop-opacity:1"/>
<stop offset="100%" style="stop-color:#a855f7;stop-opacity:1"/>
```

**Orange-Red-Pink**
```xml
<stop offset="0%" style="stop-color:#f97316;stop-opacity:1"/>
<stop offset="50%" style="stop-color:#ef4444;stop-opacity:1"/>
<stop offset="100%" style="stop-color:#f43f5e;stop-opacity:1"/>
```

**Teal-Cyan-Blue**
```xml
<stop offset="0%" style="stop-color:#06b6d4;stop-opacity:1"/>
<stop offset="50%" style="stop-color:#0ea5e9;stop-opacity:1"/>
<stop offset="100%" style="stop-color:#3b82f6;stop-opacity:1"/>
```

---

## 📞 Social Links Template

```markdown
<div align="center">

[<img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />](https://linkedin.com/in/YOUR_HANDLE)
[<img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />](https://github.com/YOUR_HANDLE)
[<img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter" />](https://twitter.com/YOUR_HANDLE)
[<img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=white" alt="LeetCode" />](https://leetcode.com/YOUR_HANDLE)
[<img src="https://img.shields.io/badge/Portfolio-7C3AED?style=for-the-badge" alt="Portfolio" />](https://yourportfolio.com)
[<img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />](mailto:your@email.com)

</div>
```

---

## 📊 Stats Section

```markdown
<div align="center">

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=vision-friendly-dark&hide_border=true&bg_color=0d1117&title_color=7c3aed&icon_color=22d3ee&text_color=e2e8f0&hide=contribs,prs)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_USERNAME&layout=compact&theme=vision-friendly-dark&hide_border=true&bg_color=0d1117&title_color=7c3aed&text_color=e2e8f0)

[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=YOUR_USERNAME&theme=vision-friendly-dark&hide_border=true)](https://github.com/YOUR_USERNAME)

</div>
```

---

## 🏆 Achievements Table

```markdown
| 🥇 | Achievement | Status |
|----|-------------|--------|
| 🎯 | 1000+ LeetCode Problems | ![1000+](https://progress-bar.dev/1000/?scale=3000&title=Problems&width=150&color=22d3ee) |
| ⭐ | Peak Rating 2000+ | ![2000+](https://progress-bar.dev/2000/?scale=3000&title=Rating&width=150&color=7c3aed) |
| 🏗️ | Projects Completed | ![15/50](https://progress-bar.dev/30/?scale=100&title=Progress&width=150&color=10b981) |
| 🔥 | GitHub Streak | 150+ Days 🔥 |
| 📚 | Open Source Contributions | 50+ |
```

---

## ⚙️ Animation Timing Reference

| Duration | Use Case | Code |
|----------|----------|------|
| Fast | UI interactions, pulse | `dur="1s"` |
| Normal | Text transitions | `dur="3s"` |
| Smooth | Title rotation | `dur="12s"` |
| Slow | Background effects | `dur="8s"` |
| Very Slow | Gradient animations | `dur="15s"` |

---

## 🎨 Glow Effects

### Soft Glow (Subtle)
```xml
<filter id="softGlow">
  <feGaussianBlur stdDeviation="2" result="coloredBlur"/>
  <feMerge>
    <feMergeNode in="coloredBlur"/>
    <feMergeNode in="SourceGraphic"/>
  </feMerge>
</filter>
```

### Medium Glow (Default)
```xml
<filter id="glow">
  <feGaussianBlur stdDeviation="4" result="coloredBlur"/>
  <feMerge>
    <feMergeNode in="coloredBlur"/>
    <feMergeNode in="SourceGraphic"/>
  </feMerge>
</filter>
```

### Intense Glow (Strong)
```xml
<filter id="intenseGlow">
  <feGaussianBlur stdDeviation="6" result="coloredBlur"/>
  <feMerge>
    <feMergeNode in="coloredBlur"/>
    <feMergeNode in="SourceGraphic"/>
  </feMerge>
</filter>
```

---

## 🎬 Custom Animations

### Pulse Effect
```xml
<circle cx="100" cy="100" r="10" fill="#22d3ee">
  <animate attributeName="r" values="10;15;10" dur="2s" repeatCount="indefinite"/>
  <animate attributeName="opacity" values="1;0.5;1" dur="2s" repeatCount="indefinite"/>
</circle>
```

### Float Effect
```xml
<rect x="50" y="50" width="100" height="100" fill="#7c3aed">
  <animateTransform
    attributeName="transform"
    type="translate"
    values="0,0; 0,-20; 0,0"
    dur="4s"
    repeatCount="indefinite"/>
</rect>
```

### Fade In/Out
```xml
<text x="100" y="100" fill="#10b981">
  Hello
  <animate attributeName="opacity" values="0;1;0" dur="3s" repeatCount="indefinite"/>
</text>
```

### Color Shift
```xml
<rect x="50" y="50" width="100" height="100" fill="#7c3aed">
  <animate attributeName="fill" 
    values="#7c3aed;#22d3ee;#10b981;#7c3aed" 
    dur="6s" 
    repeatCount="indefinite"/>
</rect>
```

---

## 📝 About Section Templates

### For Beginners
```markdown
- 🎓 Learning web development
- 💻 Passionate about coding
- 🌱 Currently exploring React & Node.js
- 🎯 Building projects to improve skills
```

### For Intermediate
```markdown
- 🎓 BS in Computer Science
- 💼 2+ years in Full Stack Development
- 🚀 Specializing in React & Python
- 🌍 Contributing to open source
```

### For Senior/Lead
```markdown
- 🎓 MS in Computer Science
- 💼 8+ years in system design & architecture
- 🏗️ Led teams of 5+ engineers
- 🚀 Focus on scalable solutions & mentoring
```

---

## 🚀 Quick Replace List

Create a checklist of what to replace:

- [ ] `YOUR_USERNAME` → Your GitHub username
- [ ] `YOUR_NAME` → Your full name
- [ ] `YOUR_EMAIL` → Your email address
- [ ] `YOUR_HANDLE` → Your social media handles
- [ ] Job titles → Your actual titles
- [ ] Projects → Your real projects
- [ ] Skills → Your actual tech stack
- [ ] Links → Your real links
- [ ] Colors → Your preferred theme

---

## 🎯 Top 10 Changes to Make

1. ✅ Change name from "Ayush Rai" to your name
2. ✅ Update job titles to match your role
3. ✅ Replace project examples with your work
4. ✅ Update social media links
5. ✅ Modify tech stack badges
6. ✅ Update GitHub stats username
7. ✅ Change color scheme if desired
8. ✅ Update achievements section
9. ✅ Add your bio information
10. ✅ Update email and contact details

---

<div align="center">

### 💡 Tip: Use Find & Replace (Ctrl+H / Cmd+H) to change multiple instances at once!

**Happy customizing!** 🎨✨

</div>
