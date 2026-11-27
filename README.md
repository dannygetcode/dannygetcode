<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F2027,50:203A43,100:2C5364&height=200&section=header&text=Daniel%20Barrag%C3%A1n&fontColor=FFFFFF&fontSize=60&fontAlignY=38&desc=Economist%20%7C%20Software%20Engineering%20%7C%20Data&descAlignY=58&descSize=20&animation=fadeIn" alt="Daniel Barragán" width="100%"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=20&duration=3500&pause=900&color=2C9FAF&center=true&vCenter=true&width=640&lines=Economist+who+ships+production+code.;From+raw+data+to+decisions+you+can+audit.;Econometrics+in+the+model.+Tests+in+the+pipeline.;Currently+forecasting+the+air+in+Boyac%C3%A1." alt="Typing intro"/>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/daniel-chia-data"><img src="https://img.shields.io/badge/LinkedIn-daniel--chia--data-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://dannygetcode.github.io/simulador-hipotecario/"><img src="https://img.shields.io/badge/Live%20demo-Mortgage%20simulator-2C9FAF?style=for-the-badge&logo=githubpages&logoColor=white" alt="Live demo"/></a>
</p>

<br/>

## About me

I'm an economist from Universidad Pedagógica y Tecnológica de Colombia and a Software Engineering student at Universidad Manuela Beltrán. I build data systems end to end. That covers the schema, the pipeline, the statistics and the screen where someone makes a decision with the result.

I care about the boring parts that keep a system alive after launch day. I test against real infrastructure and write my design decisions down. Every number I ship can be traced back to its source.

<table>
  <tr>
    <td width="50%" valign="top">
      <h4>What the economist brings</h4>
      <ul>
        <li>Logit and Probit models with marginal effects</li>
        <li>Household survey data with expansion factors (DANE)</li>
        <li>Forecasts that report their uncertainty</li>
        <li>A habit of separating association from causation</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h4>What the engineer brings</h4>
      <ul>
        <li>REST APIs in Spring Boot and Python services</li>
        <li>PostgreSQL schemas versioned with migrations</li>
        <li>Docker deployments with CI on every push</li>
        <li>Android apps in Kotlin and web panels in Next.js</li>
      </ul>
    </td>
  </tr>
</table>

## How I work

- In my [report engine](https://github.com/dannygetcode/Motor_Estadistico_Capa_Analitica_CIUMB) the [statistics engine](https://github.com/dannygetcode/Motor_Estadistico_Capa_Analitica_CIUMB/tree/main/src/ciumb_analitica/motor) computes every figure. The LLM only writes the prose around it. A validator then compares each number in the text with the computed result.
- Integration tests run against a real PostgreSQL instance with Testcontainers. CI runs them on every push.
- My larger projects keep ADRs. The next person on the team can read why the system looks the way it does.
- Each service connects with a database role that can only write its own tables. Secrets live in environment variables.
- Forecasts ship with a prediction interval and backtest metrics. Simulated data stays apart from real data.

## Selected work

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>Air quality surveillance and PM10 forecasting</h3>
      <p>My Software Engineering thesis. Seven services with their own OpenAPI contracts watch PM10 in the Sogamoso-Nobsa industrial corridor under Colombian regulation (Res. 2254/2017). They validate hourly readings and compute 24-hour averages. They also propose alert levels and issue a daily 24-hour forecast with a prediction interval. A virtual clock replays a full year of IDEAM data in under 30 minutes.</p>
      <p><code>Python</code> <code>PostgreSQL 16</code> <code>Docker</code> <code>OpenAPI</code> <code>pytest</code></p>
      <p><a href="https://github.com/dannygetcode/Trabajo_de_Grado_Vigilancia_PM10_Sogamoso_Nobsa">Repository</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>Report engine with verified figures</h3>
      <p>Built during my internship at UMB's research center. It turns a question in plain language into a PDF, DOCX, XLSX, HTML or CSV report. Behind it sit an incremental ETL, a data warehouse, a SQL compiler restricted to a whitelist and a statistics engine. The AI layer is optional. If it goes down, the report still ships with a template text.</p>
      <p><code>Python</code> <code>pandas</code> <code>SciPy</code> <code>statsmodels</code> <code>scikit-learn</code> <code>Docker</code></p>
      <p><a href="https://github.com/dannygetcode/Motor_Estadistico_Capa_Analitica_CIUMB/tree/main/src/ciumb_analitica/motor">Statistics engine</a> · <a href="https://github.com/dannygetcode/Motor_Estadistico_Capa_Analitica_CIUMB">Repository</a></p>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>Mortgage access simulator</h3>
      <p>The interactive side of my economics monograph at UPTC on who gets a mortgage in Colombia. It uses Logit and Probit models fitted on DANE household surveys from 2019 and 2024. You change a household's features and a 3D scene shows the estimated probability. Marginal effects and a life-cycle curve sit next to it.</p>
      <p><code>Econometrics</code> <code>JavaScript</code> <code>Three.js</code> <code>GSAP</code></p>
      <p><a href="https://dannygetcode.github.io/simulador-hipotecario/">Live demo</a> · <a href="https://github.com/dannygetcode/simulador-hipotecario">Repository</a></p>
    </td>
    <td width="50%" valign="top">
      <h3>Mercado, an offline grocery budget app</h3>
      <p>An Android app that keeps a running total against a budget while you scan barcodes in the aisle. It reads shelf prices with on-device OCR and has no internet permission. Data lives in an encrypted database. The app also has fingerprint lock and encrypted backups.</p>
      <p><code>Kotlin</code> <code>Jetpack Compose</code> <code>Room + SQLCipher</code> <code>CameraX</code> <code>ML Kit</code></p>
      <p><a href="https://github.com/dannygetcode/App_Mercado">Repository</a></p>
    </td>
  </tr>
</table>

## Tech stack

<table>
  <tr>
    <td width="26%"><b>Economics and statistics</b></td>
    <td>
      <img src="https://img.shields.io/badge/Econometrics-1F3A5F?style=flat-square" alt="Econometrics"/>
      <img src="https://img.shields.io/badge/Logit%20%2F%20Probit-1F3A5F?style=flat-square" alt="Logit and Probit"/>
      <img src="https://img.shields.io/badge/Time%20series%20forecasting-1F3A5F?style=flat-square" alt="Time series forecasting"/>
      <img src="https://img.shields.io/badge/Survey%20data-1F3A5F?style=flat-square" alt="Survey data"/>
      <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="pandas"/>
      <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" alt="NumPy"/>
      <img src="https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white" alt="SciPy"/>
      <img src="https://img.shields.io/badge/statsmodels-4051B5?style=flat-square" alt="statsmodels"/>
    </td>
  </tr>
  <tr>
    <td><b>Data and ML</b></td>
    <td><img src="https://skillicons.dev/icons?i=python,sklearn,fastapi,flask,postgres" alt="Python, scikit-learn, FastAPI, Flask, PostgreSQL"/></td>
  </tr>
  <tr>
    <td><b>Backend</b></td>
    <td>
      <img src="https://skillicons.dev/icons?i=java,spring" alt="Java, Spring"/>&nbsp;
      <img src="https://img.shields.io/badge/Flyway-CC0200?style=flat-square&logo=flyway&logoColor=white" alt="Flyway"/>
      <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT"/>
      <img src="https://img.shields.io/badge/OpenAPI-6BA539?style=flat-square&logo=openapiinitiative&logoColor=white" alt="OpenAPI"/>
    </td>
  </tr>
  <tr>
    <td><b>Frontend and mobile</b></td>
    <td>
      <img src="https://skillicons.dev/icons?i=ts,react,nextjs,tailwind,js,threejs,kotlin,androidstudio" alt="TypeScript, React, Next.js, Tailwind, JavaScript, Three.js, Kotlin, Android Studio"/>&nbsp;
      <img src="https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white" alt="Jetpack Compose"/>
    </td>
  </tr>
  <tr>
    <td><b>Quality and delivery</b></td>
    <td>
      <img src="https://skillicons.dev/icons?i=docker,githubactions,git,azure" alt="Docker, GitHub Actions, Git, Azure"/>&nbsp;
      <img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white" alt="pytest"/>
      <img src="https://img.shields.io/badge/JUnit%205-25A162?style=flat-square&logo=junit5&logoColor=white" alt="JUnit 5"/>
      <img src="https://img.shields.io/badge/Testcontainers-291A3F?style=flat-square" alt="Testcontainers"/>
    </td>
  </tr>
</table>

## Contributions, as a snack

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/dannygetcode/dannygetcode/output/github-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/dannygetcode/dannygetcode/output/github-snake.svg"/>
  <img alt="Snake eating my contribution graph" src="https://raw.githubusercontent.com/dannygetcode/dannygetcode/output/github-snake.svg"/>
</picture>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F2027,50:203A43,100:2C5364&height=100&section=footer" width="100%" alt=""/>
</p>
