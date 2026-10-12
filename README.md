# Shivam Singh Chauhan

B.Sc. Information Engineering at **TUM** (Campus Heilbronn) · Working student in data & AI engineering at **Allianz Global Investors**

I build data and ML systems that have to work on messy, real-world signals — Wi-Fi channel data, low-resource language pairs, and large financial datasets — and I care about measuring honestly whether they work.

---

### Selected projects

**[WiSentinel](https://github.com/WiSentinel-TUM-CPS-Project/WiSentinel)** — *camera-free presence detection and localization through walls using Wi-Fi CSI* (TUM CPS project, team of 5)
I owned the **Localization Engine** ([code on `second_prototype`](https://github.com/WiSentinel-TUM-CPS-Project/WiSentinel/tree/second_prototype/Localized_Engine)):
- Physics-based features from raw CSI: **time of flight** from the channel impulse response (inverse FFT), **angle of arrival** with the **MUSIC** algorithm (antenna covariance → eigendecomposition → noise-subspace spectrum), and a spatial-correlation eigenvalue ratio
- RSSI baselines: **path-loss trilateration** and **KNN fingerprinting** on a surveyed grid, evaluated with MAE/RMSE
- Presence classifier + x/y position regressors, and a **real-time pipeline** that maps a live capture to a position on the floor plan

**[Reference-Free-MT-QE](https://github.com/shivamsinghchauhan18/Reference-Free-MT-QE)** — *translation quality estimation without references for German → Upper Sorbian (a low-resource language)*
A MetricX-style **Gemma-3 12B** regressor fine-tuned with QLoRA on 749k synthetic pseudo-labelled examples, LLM-as-a-judge with GPT-5-mini / Gemini 2.5 Flash, and a meta-evaluation of 10+ metrics on the WMT 2025 dev set. Finding: LLM judges' agreement drops 40–65 % within a single MT system, so it mostly reflects system-level differences. (Research report with Paul Hagner.)

**[Fundamental-Analysis](https://github.com/shivamsinghchauhan18/Fundamental-Analysis)** — *multi-agent financial analytics terminal*
Ten containerised agents (collection, statistics, correlation/CAPM, Monte-Carlo valuation, network analysis, sentiment, macro) orchestrated over PostgreSQL, served through a FastAPI dashboard; deployable in one click.

**[goldenduckie](https://github.com/shivamsinghchauhan18/goldenduckie)** — *autonomous Duckiebot: detection, lane following and safe stopping* (TUM Bachelor practical course, team project)

---

### Toolbox
Python · PyTorch / Lightning · Hugging Face (PEFT, LoRA/QLoRA) · scikit-learn · PySpark / Databricks · SQL / PostgreSQL · FastAPI · Docker · ROS · MATLAB · Java
