<!-- ===== BANNER ===== -->
<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:003300,100:00FF00&height=200&section=header&text=Hack2You&fontColor=00FF00&fontSize=50&animation=fadeIn&desc=C%20%7C%20Hacker%20in%20Training&descSize=18&descAlignY=68" alt="banner" width="100%" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=26&duration=2000&pause=700&color=00FF00&center=true&vCenter=true&background=003300&width=550&lines=%3E+Hack2You;%3E+Learning+C+%26+Python...;%3E+System+Access+Granted+%E2%9C%94" alt="Typing SVG" />
</div>

---

<div align="center">

```c
struct Hacker {
    char  name[]    = "Nishant";
    int   age       = 14;
    int   class     = 9;
    char  learning  = 'C';
    char  knows[]   = "Python";
    char  platform  = "CodeChef";
    char  channel[] = "Hack2You";
};
```

</div>

---

### 🧑‍💻 About Me

- 👾 **Name** — Nishant | Class **9th** | Age **14**
- ⚡ Currently deep diving into **C Programming**
- 🐍 Already **conquered Python** — 1 year ago
- 🏆 Grinding **CodeChef** — Beginner problems? Done. Next level loading...
- 🎥 Sharing my journey on → **[Hack2You](https://www.youtube.com/@Hack2YouLegend)**
- 🚀 Started at **14** — imagine where I'll be at **18**
- 💡 Motto → *"Code today. Dominate tomorrow."*

---

### 🛠️ Tech Stack

<div align="center">

![C](https://img.shields.io/badge/C-003300?style=for-the-badge&logo=c&logoColor=00FF00)
![Python](https://img.shields.io/badge/Python-003300?style=for-the-badge&logo=python&logoColor=00FF00)
![VS Code](https://img.shields.io/badge/VSCode-003300?style=for-the-badge&logo=visual-studio-code&logoColor=00FF00)
![GitHub](https://img.shields.io/badge/GitHub-003300?style=for-the-badge&logo=github&logoColor=00FF00)
![CodeChef](https://img.shields.io/badge/CodeChef-003300?style=for-the-badge&logo=codechef&logoColor=00FF00)
![Linux](https://img.shields.io/badge/Linux-003300?style=for-the-badge&logo=linux&logoColor=00FF00)

</div>

---

### 🏆 GitHub Trophies

<div align="center">
<img src="https://github-profile-trophy.vercel.app/?username=Hack2YouLegend&theme=matrix&no-frame=true&no-bg=true&margin-w=4&column=7" alt="trophies" />
</div>

---

### 📊 GitHub Stats

<div align="center">
<img src="https://github-readme-stats.vercel.app/api?username=Hack2YouLegend&hide_border=false&include_all_commits=true&count_private=false&title_color=00FF00&text_color=00FF00&icon_color=00FF00&bg_color=003300&border_color=00FF00" alt="GitHub Stats" width="48%" />
<img src="https://streak-stats.demolab.com/?user=Hack2YouLegend&hide_border=false&background=003300&border=00FF00&ring=00FF00&fire=00FF00&currStreakNum=00FF00&currStreakLabel=00FF00&sideNums=00FF00&sideLabels=00FF00&dates=00FF00&stroke=00FF00" alt="GitHub Streak" width="48%" />
</div>

<div align="center">
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Hack2YouLegend&layout=compact&hide_border=false&title_color=00FF00&text_color=00FF00&bg_color=003300&border_color=00FF00" alt="Top Languages" width="40%" />
</div>

---

### 📈 Activity Graph

<div align="center">
<img src="https://github-readme-activity-graph.vercel.app/graph?username=Hack2YouLegend&bg_color=003300&color=00FF00&line=00FF00&point=ffffff&area=true&hide_border=false&border_color=00FF00" alt="Activity Graph" width="100%" />
</div>

---

### 🐍 Contribution Snake

<div align="center">
<img src="https://raw.githubusercontent.com/Hack2YouLegend/Hack2YouLegend/output/github-contribution-grid-snake-dark.svg" alt="Snake animation" />
</div>

---

### 🌐 Connect With Me

<div align="center">

<a href="https://www.youtube.com/@Hack2YouLegend">
  <img src="https://img.shields.io/badge/YouTube-003300?style=for-the-badge&logo=youtube&logoColor=00FF00" alt="YouTube" />
</a>
<a href="https://www.codechef.com/users/Hack2YouLegend">
  <img src="https://img.shields.io/badge/CodeChef-003300?style=for-the-badge&logo=codechef&logoColor=00FF00" alt="CodeChef" />
</a>
<a href="https://github.com/Hack2YouLegend">
  <img src="https://img.shields.io/badge/GitHub-003300?style=for-the-badge&logo=github&logoColor=00FF00" alt="GitHub" />
</a>

</div>

---

<!-- FOOTER -->
<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00FF00,100:003300&height=100&section=footer" width="100%" />

![Profile Views](https://komarev.com/ghpvc/?username=Hack2YouLegend&color=00FF00&style=flat&label=Profile+Views)

⭐️ From [Hack2YouLegend](https://github.com/Hack2YouLegend)
</div>
name: Generate Snake Animation

on:
  schedule:
    - cron: "0 0 * * *"
  workflow_dispatch:

jobs:
  generate:
    runs-on: ubuntu-latest
    timeout-minutes: 10
    
    steps:
      - name: generate snake.svg
        uses: Platane/snk/svg-only@v3
        with:
          github_user_name: Hack2YouLegend
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      - name: push snake.svg to output branch
        uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
<!-- ===== BANNER ==== <!--
