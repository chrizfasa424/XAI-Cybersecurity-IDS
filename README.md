# AI-Powered Intrusion Detection System with Explainable AI (XAI)

This repository contains the practical prototype for the academic research paper, **"AI-Powered Cyber Defense In Academic Networks."**

This project's mission is to build a practical, effective, and—most importantly—**transparent** Intrusion Detection System (IDS). It directly addresses the "black box" problem prevalent in modern AI-driven security, as identified in my research.

* **My Research Paper:** https://www.techrxiv.org/users/995622/articles/1356555-ai-powered-cyber-defense-in-academic-networks
* **My LinkedIn:** [www.linkedin.com/in/christian-ohwofasa-c-itp-mcpn-mncs-318927232](http://www.linkedin.com/in/christian-ohwofasa-c-itp-mcpn-mncs-318927232)
* **My Technical Blog:** [https://medium.com/@christianohwofasa](https://medium.com/@christianohwofasa)

## The 3-Phase Research Prototype

This project is broken into three research notebooks, which correspond to the three phases of this research.

1.  **[Phase 1: The Baseline (Random Forest)](./01-Baseline-IDS-RandomForest.ipynb)**
    * This notebook establishes a "classical" machine learning baseline.
    * **Finding:** The Random Forest model is simple but has a "critical failure": it **misses 39% of all real attacks (a recall of 0.61)**.

2.  **[Phase 2: The "Promise" (LSTM)](./02-Advanced-IDS-LSTM.ipynb)**
    * This notebook implements the advanced, sequential Deep Learning model (LSTM) proposed in my paper.
    * **Finding:** The LSTM model is superior, **improving attack recall from 61% to 66%**. It proves that models with "memory" are better at finding complex attacks.

3.  **[Phase 3: The "Proof" (XAI)](./03-ExplainableAI-XAI.ipynb)**
    * This final notebook *proves the thesis* by using Explainable AI (XAI) to open the "black box."
    * **Finding (The "Golden" Evidence):** We proved *why* the LSTM is smarter.
        * The **Random Forest** only looks at basic features like `src_bytes`.
        * The **LSTM** thinks like an analyst, focusing on *behavioral patterns* like `srv_rerror_rate` (the rate of rejection errors), allowing it to find coordinated attacks.

## Key Evidence: The "Brains" of the Models

These two plots, generated in Phase 3, are the core evidence of this research.

#### Plot 1: The "Simple" Brain (Random Forest)
*This model is a "bouncer" looking at basic, static features.*
![Random Forest XAI Plot](httpsDELETED_FOR_PRIVACY)

#### Plot 2: The "Advanced" Brain (LSTM)
*This model is an "intelligence officer" looking for complex, behavioral patterns.*
![LSTM XAI Plot](https://github.com/chrizfasa424/XAI-Cybersecurity-IDS/blob/main/lstm_plot.png?raw=true)

## Dataset

This project uses the benchmark **NSL-KDD Dataset**.
* [`KDDTrain+.txt`](./KDDTrain+.txt)
* [`KDDTest+.txt`](./KDDTest+.txt)

## My Expertise to Deliver This

This project is the synthesis of my career experience and my 2025 "blitz" of advanced certifications and research.

* **Cybersecurity Leadership:** As the **SOC Analyst & IT Leader at Bitsmart Pay**, a FinTech company, I am responsible for applying these concepts to protect real-world financial data.
* **Academic Innovation:** This project is the practical output of my **co-authored research paper**, "AI-Powered Cyber Defense In Academic Networks."
* **Certified Technical Skills:**
    * **Networking (CCNA, Network+):** Deep, practical knowledge of the network traffic this IDS analyzes.
    * **Security (Security+, CySA+):** Certified expertise in the threat analysis and intrusion detection principles being modeled.
    * **Cloud (Azure Fundamentals):** Knowledge to build and deploy this as a modern, scalable cloud-native application.
