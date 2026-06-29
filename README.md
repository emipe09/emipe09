<div align="center">
  <img src="https://user-images.githubusercontent.com/74038190/235224431-e8c8c12e-6826-47f1-89fb-2ddad83b3abf.gif" width="100px" />
  
  <h1>Olá, eu sou o Marcos Paulo! 👋</h1>
  <h1>Hello, I'm Marcos Paulo! 👋</h1>

  <h3>Engenharia da Computação @ UFOP 🎓</h3>
  <h3>Computer Engineering @ UFOP 🎓</h3>

  <p>
    <b>Mobile Developer • Back-End Developer • Data Science Researcher</b>
  </p>

  <a href="https://www.linkedin.com/in/marcos-paulo-04892b216/" target="_blank">
    <img src="https://img.shields.io/badge/-LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>

  <a href="mailto:mpmarcos1016@gmail.com">
    <img src="https://img.shields.io/badge/-Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</div>

<br/>

# 👨‍💻 Sobre Mim | About Me

🇧🇷  
Sou estudante de Engenharia da Computação apaixonado por desenvolver software de impacto e transformar dados complexos em soluções inteligentes.

Minha trajetória combina:
- 📱 Desenvolvimento Mobile
- ⚙️ Engenharia Back-End
- 📊 Ciência de Dados e Machine Learning

Atualmente atuo como **Estagiário em Desenvolvimento Mobile na SYSDAM**, desenvolvendo aplicações cross-platform com foco em performance, escalabilidade e experiência do usuário.

Também possuo experiência como **Desenvolvedor Back-End (Node.js)** na residência de software da **iUUL**.

---

🇺🇸  
I'm a Computer Engineering student passionate about building impactful software and transforming complex data into intelligent solutions.

My journey combines:
- 📱 Mobile Development
- ⚙️ Back-End Engineering
- 📊 Data Science & Machine Learning

Currently, I work as a **Mobile Development Intern at SYSDAM**, developing cross-platform applications focused on performance, scalability and user experience.

I also have experience as a **Back-End Developer (Node.js)** at the software residency program from **iUUL**.

---

# 🔬 Pesquisa & Fórmula 1 | Research & Formula 1

🇧🇷  
Uma das minhas maiores paixões é pesquisa e machine learning aplicado.

Atualmente, meu principal projeto de pesquisa e TCC é focado em:

🏎️ **Predição de Tempos de Volta na Fórmula 1 utilizando Machine Learning**

O projeto envolve:
- Modelagem de ritmo de corrida
- Integração de dados meteorológicos
- Estratégias de validação com Sliding Window
- Análise de pilotos, equipes e pneus
- Processamento de dados inspirado em telemetria real

Meu objetivo é unir:
- Rigor estatístico
- Engenharia de software
- Análise de motorsport
- Interpretabilidade em machine learning

para construir modelos robustos de análise de performance na Fórmula 1.

---

🇺🇸  
One of my biggest passions is research and applied machine learning.

Currently, my main research project and undergraduate thesis focuses on:

🏎️ **Formula 1 Lap Time Prediction using Machine Learning**

The project involves:
- Race pace modeling
- Weather integration
- Sliding window validation strategies
- Driver/team/tire performance analysis
- Telemetry-inspired data processing

My goal is to combine:
- Statistical rigor
- Software engineering
- Motorsport analytics
- Machine learning interpretability

to create robust predictive models for Formula 1 performance analysis.

---

# 📂 Projeto em Destaque | Featured Project — F1-MultiCircuit-LapTimeModel

🇧🇷  
Código de pesquisa e material suplementar do meu **TCC**, base do artigo *"Multi-Circuit Formula 1 Lap Time Prediction: A Hybrid Deep Learning Approach for Race Pace Analysis"* (**KDMiLe 2026**). O projeto modela o `LapTime_seconds` a partir de dados públicos de corrida do **FastF1**, com um protocolo de validação temporal que espelha uma corrida real: janela expansiva no bloco de modelagem e um **holdout sequencial** nas últimas voltas.

**🏁 Escopo (5 GPs do regulamento técnico 2022–2025):**
Bahrein 🇧🇭 • Arábia Saudita 🇸🇦 • Estados Unidos 🇺🇸 • Itália 🇮🇹 • Hungria 🇭🇺

**🤖 Modelos comparados:**
- **Linear Regression** (expanding-window) — baseline interpretável
- **XGBoost** (expanding-window, espaço de busca Optuna por circuito) — baseline não-linear
- **LSTM Hybrid** *(modelo selecionado)* — baseline LR-EW + LSTM que prediz o **resíduo** `LapTime_seconds − baseline_prediction`, mantendo um forte componente linear enquanto a rede captura a estrutura complexa restante

**🔬 Metodologia:**
- Ordenação cronológica multi-temporada (por ano e, dentro de cada ano, por número da volta)
- Validação **Sliding-Window** / **Expanding-Window** nos primeiros 80% + **holdout sequencial** nos últimos 20%
- Métricas: **RMSE, MAE, R², desvio-padrão do resíduo, intervalos de confiança via bootstrap** e o indicador de estabilidade **COS_MAE / COS_RMSE**
- Otimização de hiperparâmetros com **Optuna** e rastreamento de experimentos com **MLflow**
- **Interpretabilidade** via coeficientes da regressão, importância de features e **SHAP** no XGBoost
- Análise por piloto, equipe, composto de pneu e condições meteorológicas
- Geração automática de tabelas **LaTeX** para o artigo

**🛠️ Stack do projeto:** Python • Pandas • NumPy • Scikit-Learn • XGBoost • TensorFlow/Keras • FastF1 • Optuna • MLflow • SHAP

---

🇺🇸  
Research code and supplementary material for my **undergraduate thesis (TCC)**, the foundation of the paper *"Multi-Circuit Formula 1 Lap Time Prediction: A Hybrid Deep Learning Approach for Race Pace Analysis"* (**KDMiLe 2026**). The project models `LapTime_seconds` from public **FastF1** race data with a temporal protocol that mirrors a real race: expanding-window validation inside the modeling block and a final **sequential holdout** on the last laps.

**🏁 Scope (5 Grand Prix from the 2022–2025 technical-regulation era):**
Bahrain 🇧🇭 • Saudi Arabia 🇸🇦 • United States 🇺🇸 • Italy 🇮🇹 • Hungary 🇭🇺

**🤖 Compared models:**
- **Linear Regression** (expanding-window) — interpretable baseline
- **XGBoost** (expanding-window, circuit-specific Optuna search space) — non-linear baseline
- **LSTM Hybrid** *(selected model)* — LR-EW baseline + an LSTM predicting the **residual** `LapTime_seconds − baseline_prediction`, keeping a strong linear component while the network captures the remaining complex structure

**🔬 Methodology:**
- Multi-season chronological ordering (by year, then by lap number within each year)
- **Sliding-Window** / **Expanding-Window** validation over the first 80% + **sequential holdout** on the last 20%
- Metrics: **RMSE, MAE, R², residual standard deviation, bootstrap confidence intervals** and the **COS_MAE / COS_RMSE** stability indicator
- Hyperparameter optimization with **Optuna** and experiment tracking with **MLflow**
- **Interpretability** through regression coefficients, feature importance and **SHAP** on XGBoost
- Analysis by driver, team, tire compound and weather conditions
- Automatic generation of **LaTeX** tables for the paper

**🛠️ Project stack:** Python • Pandas • NumPy • Scikit-Learn • XGBoost • TensorFlow/Keras • FastF1 • Optuna • MLflow • SHAP

---

# 🚀 Main Stack | Stack Principal

<div align="center">

## 📱 Mobile Development

<img src="https://img.shields.io/badge/React_Native-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
<img src="https://img.shields.io/badge/Expo-1B1F23?style=for-the-badge&logo=expo&logoColor=white" />
<img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" />

<br><br>

## ⚙️ Back-End & Databases

<img src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white" />
<img src="https://img.shields.io/badge/Express.js-404D59?style=for-the-badge" />
<img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" />
<img src="https://img.shields.io/badge/MySQL-005C84?style=for-the-badge&logo=mysql&logoColor=white" />
<img src="https://img.shields.io/badge/Sequelize-52B0E7?style=for-the-badge&logo=sequelize&logoColor=white" />

<br><br>

## 📊 Data Science & AI

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
<img src="https://img.shields.io/badge/Scikit_Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" />
<img src="https://img.shields.io/badge/XGBoost-EC4B26?style=for-the-badge&logo=xgboost&logoColor=white" />
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
<img src="https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white" />

<br><br>

## 🛠️ Languages & Tools

<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
<img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white" />
<img src="https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white" />
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" />

</div>

---

# ⚡ Foco Atual | Current Focus

- 📱 Mobile Engineering with React Native & Expo
- 🧠 Machine Learning Research
- 🏎️ Formula 1 Data Analytics
- 📈 Predictive Modeling
- 🏗️ Clean Architecture & Scalable Systems

---

<div align="center">

### “Always trying to become 1% better every day.”

</div>
