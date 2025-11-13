<h1 align="center">Hi, I'm Nikolaos Roukoudis 👋</h1>
<h3 align="center">
  <a href="https://github.com/NikosRoukoudis">
    <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=28&color=1F2937&center=true&width=1500&lines=CS+Student+%7C+Developer+%7C+Tech+Enthusiast" alt="Typing SVG"/>
  </a>
</h3>

---

## 🧑‍💻 About Me
Hi! I'm **Nikolaos Roukoudis**, a **Computer Science student** from Polykastro, Greece.  
I am passionate about **Web Development, App Development, Web Design, and AI**.  

My goal is to create applications that help communities and build professional software solutions.  

<p align="center">
  <a href="https://drive.google.com/file/d/1Djou6dleRK8dUFDFCE8kv5i9cxmleJSH/view?usp=sharing"><img src="https://img.shields.io/badge/Resume-PDF-red?style=for-the-badge&logo=adobeacrobat&logoColor=white"/></a>
</p>
---

## 🛠 Skills

### **Languages**
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

### **Web & Frameworks**
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)

---

## 📁 Portfolio Highlights
- 📱 **App Development**  
- 🌐 **Web Development**  
- 🎨 **Web Design**  
- 🏕️ **AUTH University Camp (Front Desk)**  

---

import { useEffect, useState } from "react";

export default function Projects() {
  const [repos, setRepos] = useState([]);

  useEffect(() => {
    fetch("https://api.github.com/users/YOUR_GITHUB_USERNAME/repos?sort=updated")
      .then((res) => res.json())
      .then((data) => {
        // Optionally filter to only include relevant repos
        const filtered = data.filter(repo => !repo.fork);
        setRepos(filtered);
      });
  }, []);

  return (
    <div>
      <h2>💻 Projects</h2>
      <ul>
        {repos.map(repo => (
          <li key={repo.id}>
            <a href={repo.html_url} target="_blank">{repo.name}</a> - {repo.description}
          </li>
        ))}
      </ul>
    </div>
  );
}


## 📫 Contact Me 
<p align="center">
  <a href="https://www.instagram.com/nikos_roukoudis/"><img src="https://img.shields.io/badge/Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white"/></a>
  <a href="https://www.linkedin.com/in/%CE%BD%CE%B9%CE%BA%CE%BF%CE%BB%CE%B1%CE%BF%CF%82-%CF%81%CE%BF%CF%85%CE%BA%CE%BF%CF%85%CE%B4%CE%B7%CF%82-2a25b5318/"><img src="https://img.shields.io/badge/LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="mailto:roukoudis.nikolaos@gmail.com"><img src="https://img.shields.io/badge/Gmail-ffffff?style=for-the-badge&logo=gmail&logoColor=red" alt="Email Badge" /></a>
</a>
</p>

---

## 📊 GitHub Stats
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=NikosRoukoudis&show_icons=true&theme=radical&hide_title=false" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=NikosRoukoudis&theme=radical" alt="GitHub Streak" />
</p>

---

### 🚀 Thank you for visiting my profile!
Feel free to explore my projects and reach out for collaborations!
