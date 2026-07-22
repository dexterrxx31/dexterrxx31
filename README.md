<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&pause=2000&color=94E2D5&center=true&vCenter=true&width=600&lines=riyan%40backend%3A~%24+whoami;Backend+Engineer+%7C+Python+%C2%B7+Go+%C2%B7+AWS" />
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&pause=2000&color=179299&center=true&vCenter=true&width=600&lines=riyan%40backend%3A~%24+whoami;Backend+Engineer+%7C+Python+%C2%B7+Go+%C2%B7+AWS" alt="Riyan Ahmad — Backend Engineer" />
</picture>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-riyanahmad-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/riyanahmad/)
[![Email](https://img.shields.io/badge/Email-riyanahmad99-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:riyanahmad99@gmail.com)
[![X](https://img.shields.io/badge/X-dex__riyan-1c1c1c?style=flat-square&logo=x&logoColor=white)](https://twitter.com/dex_riyan)
[![Discord](https://img.shields.io/badge/Discord-dexterrxx-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.gg/qnqR2rphEH)
![Profile Views](https://komarev.com/ghpvc/?username=dexterrxx31&color=94e2d5&style=flat-square)

</div>

## `$ whoami`

Backend engineer who builds **scalable microservices** with Python (FastAPI/Django) and ships them on **AWS** — Lambda, S3, SNS, DynamoDB, CloudWatch. I care about the unglamorous parts: API contracts (OpenAPI/AsyncAPI), performance under load, deterministic tests (Pytest), and CI/CD that never surprises you. Lately I've been going deeper into **Go for hot paths** and **video streaming infrastructure** — and exploring deep learning with PyTorch on the side.

## `$ cat spotlight/showrunner.md`

> **[showrunner](https://github.com/dexterrxx31/showrunner)** — an AI-programmed linear TV channel. A cloud playout engine that turns a media library into a 24/7 HLS live stream, with Claude as the programming director: *"90s action night, family-friendly until 21:00"* → a validated schedule, on air.

```
 Ingest & normalize ─────────────▶ Segment store (pre-cut HLS, S3/nginx)
 (FFmpeg + Celery)                          │
        │                                   ▼
 Schedule API ──▶ Timeline resolver ──▶ Manifest generator ──▶ Player
 (FastAPI + PG)   (wall clock → asset)  (stateless, Go origin)  (hls.js)
        │
        ▼
 XMLTV EPG · SCTE-35 markers       AI director (Claude tool-use)
```

- **Stateless manifest-stitching core** — the architecture behind real FAST channels; every manifest is a pure function of `(clock, catalog, schedule)`. Verified drift-free over a 24-hour soak.
- **Go manifest origin** — hot path rewritten in Go, byte-for-byte matched against the Python reference, **~16× throughput** (~147k req/s).
- **AI programming director** — Claude tool-use generates schedules; deterministic validation is the safety rail.
- **Broadcast-grade extras** — multi-channel, XMLTV EPG, SCTE-35 ad markers, optional true-encode branded playout.
- **99 Python tests + Go tests**, CI green.

`Python` · `FastAPI` · `Go` · `FFmpeg` · `Celery` · `PostgreSQL` · `Claude API`

## `$ ls ~/stack`

| | |
|---:|---|
| **Languages** | ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white) ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white) |
| **Backend** | ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white) ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white) ![Express](https://img.shields.io/badge/Express-1c1c1c?style=flat-square&logo=express&logoColor=white) ![Celery](https://img.shields.io/badge/Celery-37814A?style=flat-square&logo=celery&logoColor=white) |
| **Data** | ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=flat-square&logo=amazondynamodb&logoColor=white) ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white) ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) |
| **Cloud & Infra** | ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) |
| **Media** | ![FFmpeg](https://img.shields.io/badge/FFmpeg-007808?style=flat-square&logo=ffmpeg&logoColor=white) ![HLS](https://img.shields.io/badge/HLS-1c1c1c?style=flat-square&logo=applepodcasts&logoColor=white) |
| **ML** | ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white) |
| **Testing** | ![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white) ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white) |

## `$ ls ~/projects`

| Project | What it is | Stack |
|---|---|---|
| **[showrunner](https://github.com/dexterrxx31/showrunner)** | AI-programmed 24/7 linear TV channel — cloud HLS playout engine | Python · Go · FastAPI · FFmpeg · Claude API |
| **[streamvault](https://github.com/dexterrxx31/streamvault)** | Full-stack video streaming platform — JWT auth, HTTP 206 range streaming | Java · Spring Boot · Angular · TypeScript |
| **[DeepLearning_PyTorch](https://github.com/dexterrxx31/DeepLearning_PyTorch)** | Deep learning notebooks & experiments | PyTorch · Jupyter |
| **[DataStructuresAlgorithms](https://github.com/dexterrxx31/DataStructuresAlgorithms)** | DSA implementations & problem solving | C++ |

## `$ git log --stat`

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats-sigma-five.vercel.app/api?username=dexterrxx31&show_icons=true&theme=catppuccin_mocha&hide_border=true&include_all_commits=true" />
  <img height="170" src="https://github-readme-stats-sigma-five.vercel.app/api?username=dexterrxx31&show_icons=true&theme=catppuccin_latte&hide_border=true&include_all_commits=true" alt="GitHub Stats" />
</picture>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=dexterrxx31&layout=compact&theme=catppuccin_mocha&hide_border=true&langs_count=8" />
  <img height="170" src="https://github-readme-stats-sigma-five.vercel.app/api/top-langs/?username=dexterrxx31&layout=compact&theme=catppuccin_latte&hide_border=true&langs_count=8" alt="Top Languages" />
</picture>

</div>

---

<div align="center">

*"First, solve the problem. Then, write the code."* — John Johnson

</div>
