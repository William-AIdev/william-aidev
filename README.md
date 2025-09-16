<!-- 头像与标题 -->
<h1 align="center">Hi, I'm William (Mengqi) Wang</h1>
<p align="center">
  Full-Stack Engineer · Python · React/Next.js · API Design · CI/CD
</p>

<p align="center">
  <a href="https://github.com/william-aidev"><img src="https://komarev.com/ghpvc/?username=william-aidev&style=flat-square" /></a>
  <a href="mailto:william.mq.wang@gmail.com"><img src="https://img.shields.io/badge/Email-contact-blue?style=flat-square" /></a>
  <img src="https://img.shields.io/badge/Location-Sydney,%20AU-informational?style=flat-square" />
</p>

---

## Tech stack
**Backend**
![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python)
![Flask](https://img.shields.io/badge/Flask-API-000?logo=flask)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-ORM-red)
![SQL](https://img.shields.io/badge/SQL-Structured%20Query%20Language-025E8C?logo=database&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-DBMS-4479A1?logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-DB-336791?logo=postgresql)

**Frontend**
![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=000)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?logo=javascript&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-13-000?logo=nextdotjs)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-UI-38B2AC?logo=tailwindcss)

**DevOps & Tools**
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-CI%2FCD-2088FF?logo=githubactions)
![Docker](https://img.shields.io/badge/Docker-containers-2496ED?logo=docker)
![Jira](https://img.shields.io/badge/Jira-agile-0052CC?logo=jira)
![Postman](https://img.shields.io/badge/Postman-testing-FF6C37?logo=postman)

---

## Stats

---

name: Metrics
on:
  schedule:
    - cron: "0 */24 * * *"   # 每天更新一次
  workflow_dispatch:

jobs:
  github-metrics:
    runs-on: ubuntu-latest
    steps:
      - uses: lowlighter/metrics@latest
        with:
          # 你的 GitHub 用户名
          token: ${{ secrets.METRICS_TOKEN }}
          user: william-aidev
          template: classic
          base: header, activity, community, repositories
          config_timezone: Australia/Sydney
          
          # 插件
          plugin_stars: yes
          plugin_stars_limit: 5
          
          plugin_languages: yes
          plugin_languages_ignored: html, css
          plugin_languages_limit: 8
          
          plugin_isocalendar: yes
          plugin_isocalendar_duration: full-year
          plugin_isometric: yes

