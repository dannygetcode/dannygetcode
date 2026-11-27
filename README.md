<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F2027,50:203A43,100:2C5364&height=200&section=header&text=Daniel%20Barrag%C3%A1n&fontColor=FFFFFF&fontSize=60&fontAlignY=38&desc=Data%20%7C%20AI%20%7C%20Software%20Engineering&descAlignY=58&descSize=20&animation=fadeIn" alt="Daniel Barragán" width="100%"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3500&pause=900&color=2C9FAF&center=true&vCenter=true&width=620&lines=From+raw+data+to+decisions+you+can+audit.;Trust+the+data.+Verify+the+AI.;Turning+surveys+into+probabilities.;Currently+forecasting+the+air+in+Boyac%C3%A1." alt="Typing intro"/>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/daniel-chia-data"><img src="https://img.shields.io/badge/LinkedIn-daniel--chia--data-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://dannygetcode.github.io/simulador-hipotecario/"><img src="https://img.shields.io/badge/Live%20demo-mortgage%20simulator-2C9FAF?style=flat-square&logo=githubpages&logoColor=white" alt="Live demo"/></a>
</p>

## About me

I'm a software engineer (Universidad Manuela Beltrán) who builds data systems end to end: the schema, the pipeline, the statistics and the screen where someone makes a decision with the result. I care about the boring parts that keep a system alive after launch day: tests against real infrastructure, written-down decisions and numbers that can be traced back to their source.

## How I work

- **Every number has an owner.** In my [report engine](https://github.com/dannygetcode/Motor_Estadistico_Capa_Analitica_CIUMB) the LLM writes the prose but never computes a figure or writes SQL. A validator checks each number in the text against the [statistics engine](https://github.com/dannygetcode/Motor_Estadistico_Capa_Analitica_CIUMB/tree/main/src/ciumb_analitica/motor).
- **Tests run against the real thing.** Integration tests spin up PostgreSQL with Testcontainers, and CI runs them on every push.
- **Decisions are written down.** My larger projects keep ADRs, so the next person knows why something is the way it is.
- **Least privilege by default.** Each service connects with a database role that can only write its own tables, and secrets come from the environment, not from the repository.
- **Forecasts come with their error bars.** A prediction ships with its interval and its backtest, and simulated data never gets mixed with real data.

## Selected work

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>Air quality surveillance and PM10 forecasting</h3>
      <p>My thesis. Seven services with their own OpenAPI contracts watch PM10 in the Sogamoso-Nobsa industrial corridor under Colombian regulation (Res. 2254/2017). They validate hourly readings, compute 24-hour averages, propose alert levels and issue a daily 24-hour forecast with a prediction interval. A virtual clock replays a full year of IDEAM data in under 30 minutes.</p>
      <p><code>Python</code> <code>PostgreSQL 16</code> <code>Docker</code> <code>OpenAPI</code> <code>pytest</code></p>
      <p><a href="https://github.com/dannygetcode/Trabajo_de_Grado_Vigilancia_PM10_Sogamoso_Nobsa">Repository</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>Report engine with verified figures</h3>
      <p>Built during my internship at UMB's research center. It turns a question in plain language into a PDF, DOCX, XLSX, HTML or CSV report. Behind it sit an incremental ETL, a data warehouse, a SQL compiler restricted to a whitelist and a statistics engine. The AI layer is optional: if it goes down, the report still ships with a template text.</p>
      <p><code>Python</code> <code>pandas</code> <code>SciPy</code> <code>statsmodels</code> <code>scikit-learn</code> <code>Docker</code></p>
      <p><a href="https://github.com/dannygetcode/Motor_Estadistico_Capa_Analitica_CIUMB/tree/main/src/ciumb_analitica/motor">Statistics engine</a> · <a href="https://github.com/dannygetcode/Motor_Estadistico_Capa_Analitica_CIUMB">Repository</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Mortgage access simulator</h3>
      <p>An interactive version of my research on who gets a mortgage in Colombia. It runs Logit and Probit models fitted on DANE household surveys (2019 and 2024). You change a household's features and a 3D scene shows the estimated probability, together with marginal effects and a life-cycle curve.</p>
      <p><code>Econometrics</code> <code>JavaScript</code> <code>Three.js</code> <code>GSAP</code></p>
      <p><a href="https://dannygetcode.github.io/simulador-hipotecario/">Live demo</a> · <a href="https://github.com/dannygetcode/simulador-hipotecario">Repository</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>Mercado: offline grocery budget app</h3>
      <p>An Android app that keeps a running total against a budget while you scan barcodes in the aisle. It reads shelf prices with on-device OCR and works without internet permission. Data lives in an encrypted database, with fingerprint lock and encrypted backups.</p>
      <p><code>Kotlin</code> <code>Jetpack Compose</code> <code>Room + SQLCipher</code> <code>CameraX</code> <code>ML Kit</code></p>
      <p><a href="https://github.com/dannygetcode/App_Mercado">Repository</a></p>
    </td>
  </tr>
</table>

## Tech stack

**Data, statistics and ML**

<img src="https://skillicons.dev/icons?i=python,sklearn,fastapi,flask" alt="Python, scikit-learn, FastAPI, Flask"/>&nbsp;
<img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="pandas"/>
<img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" alt="NumPy"/>
<img src="https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white" alt="SciPy"/>
<img src="https://img.shields.io/badge/statsmodels-4051B5?style=flat-square" alt="statsmodels"/>

**Backend and databases**

<img src="https://skillicons.dev/icons?i=java,spring,postgres" alt="Java, Spring, PostgreSQL"/>&nbsp;
<img src="https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white" alt="Flyway"/>
<img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT"/>
<img src="https://img.shields.io/badge/OpenAPI-6BA539?style=flat-square&logo=openapiinitiative&logoColor=white" alt="OpenAPI"/>

**Frontend and mobile**

<img src="https://skillicons.dev/icons?i=ts,react,nextjs,tailwind,js,html,css,threejs,kotlin,androidstudio" alt="TypeScript, React, Next.js, Tailwind, JavaScript, HTML, CSS, Three.js, Kotlin, Android Studio"/>&nbsp;
<img src="https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white" alt="Jetpack Compose"/>

**Quality, delivery and cloud**

<img src="https://skillicons.dev/icons?i=docker,githubactions,git,azure" alt="Docker, GitHub Actions, Git, Azure"/>&nbsp;
<img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white" alt="pytest"/>
<img src="https://img.shields.io/badge/JUnit%205-25A162?style=flat-square&logo=junit5&logoColor=white" alt="JUnit 5"/>
<img src="https://img.shields.io/badge/Testcontainers-291A3F?style=flat-square" alt="Testcontainers"/>

## Contributions, as a snack

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/dannygetcode/dannygetcode/output/github-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/dannygetcode/dannygetcode/output/github-snake.svg"/>
  <img alt="Snake eating my contribution graph" src="https://raw.githubusercontent.com/dannygetcode/dannygetcode/output/github-snake.svg"/>
</picture>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F2027,50:203A43,100:2C5364&height=100&section=footer" width="100%" alt=""/>
</p>
