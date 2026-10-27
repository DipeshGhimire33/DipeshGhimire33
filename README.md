<h1 align="center">Dipesh Ghimire</h1>

<p align="center">
  <a href="https://github.com/DipeshGhimire33/Intern_project">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=1200&color=2B6B73&center=true&vCenter=true&width=700&lines=Messy+data+in.;Trustworthy+models+out.;I+check+the+AI%27s+work." alt="Messy data in. Trustworthy models out. I check the AI's work.">
  </a>
</p>

<p align="center">
  Junior ML Engineer (BSc CSIT) · I turn messy, heavily missing, imbalanced data into models that can be trusted.
</p>

<p align="center">
  <a href="https://github.com/DipeshGhimire33"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"></a>
  <a href="https://dipeshghimire33.github.io"><img src="https://img.shields.io/badge/Portfolio-2B6B73?style=for-the-badge&logo=githubpages&logoColor=white" alt="Portfolio"></a>
  <a href="https://dipeshghimire33.github.io/Dipesh_Ghimire_CV.pdf"><img src="https://img.shields.io/badge/Download_CV-B8322A?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="Download CV"></a>
  <a href="https://www.linkedin.com/in/dipesh-ghimire-b00118370/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
</p>

---

## Featured Projects

### 1. Sepsis Prediction on 1.5M ICU Records

An end-to-end machine learning pipeline using the public PhysioNet/CinC 2019 dataset, with a Streamlit demo app. This is an educational project, not a medical tool.

|                      |                                                                                                                  |
| -------------------- | ---------------------------------------------------------------------------------------------------------------- |
| **Data**             | 1,552,210 rows from 40,336 ICU patients, with 1.8% positive observations and some lab values up to 99.8% missing |
| **Models compared**  | XGBoost, Random Forest, Histogram Gradient Boosting, Logistic Regression, Linear SVM                             |
| **Best test result** | XGBoost: PR-AUC 0.093, ROC-AUC 0.791                                                                             |
| **Key focus**        | Missing-value handling, patient-level splitting, model comparison, and validation-based threshold selection      |
| **Code**             | [Intern_project](https://github.com/DipeshGhimire33/Intern_project)                                              |

<details>
<summary><b>Where I made the call (click to open)</b></summary>

<br>

* **Missing-value handling:** I used forward filling within each patient so that a patient's last measured value remained available until a newer measurement appeared. This was a judgment call, not a method proven superior through comparative testing.
* **Model comparison:** I compared XGBoost against four baseline models using identical patient-level splits and evaluated multiple performance metrics.
* **Patient-level splitting:** Rows from the same patient were kept out of both training and testing to reduce patient-level data leakage.
* **Threshold selection:** I selected a threshold of 0.80 using validation data and applied it unchanged to the test set.

</details>

<details>
<summary><b>What the model can't do (click to open)</b></summary>

<br>

* It catches about a quarter of positive sepsis observations, with recall of 0.249 and precision of 0.136.
* It has not been validated on another hospital or population.
* The reference ranges used in the features are heuristic rather than established clinical standards.
* The strongest feature was time in the ICU, which describes model behaviour and does not establish causation.

</details>

---

### 2. Nepal Cybercrime Data Analysis

An exploratory data analysis project investigating reported cybercrime trends in Nepal. I collected and consolidated cybercrime-related aggregate data from multiple sources, then developed a structured workflow to analyze reporting patterns, cybercrime mediums, victim groups, and provincial trends.

|                         |                                                                                                                                           |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| **Data collection**     | Cybercrime reporting, medium, victim-group, population, and literacy data gathered from multiple sources                                  |
| **Time period**         | Fiscal years 2022/23–2024/25 for cybercrime reporting data                                                                                |
| **Data processing**     | Data cleaning, label standardization, consolidation, and cross-dataset validation                                                         |
| **Feature engineering** | Year-over-year changes, cybercrime medium categories, and province-level analytical features                                              |
| **Analysis**            | Annual reporting trends, cybercrime mediums, victim groups, and provincial patterns                                                       |
| **Tools**               | Python, Pandas, NumPy, Jupyter Notebook, Streamlit                                                                                        |
| **Key decision**        | Evaluated machine learning feasibility and avoided unreliable predictive modelling because the available aggregate data were insufficient |
| **Code**                | [Nepal Cybercrime Analysis](YOUR_CYBERCRIME_GITHUB_REPOSITORY_URL)                                                                        |
| **Live demo**           | Coming soon                                                                                                                               |

<details>
<summary><b>Challenges and analytical decisions (click to open)</b></summary>

<br>

* **Multi-source data collection:** Worked with cybercrime-related datasets gathered from multiple sources rather than relying on a single unified dataset.
* **Data consolidation:** Standardized inconsistent labels, reporting categories, and data structures to make comparisons across datasets possible.
* **Feature engineering:** Developed analytical features to examine yearly changes, cybercrime medium categories, and provincial reporting patterns.
* **Cross-dataset validation:** Compared annual totals across application, medium, and victim-group datasets, identifying a five-case discrepancy in the 2022/23 victim-group total.
* **Contextual analysis:** Examined provincial reporting alongside population and literacy indicators while recognizing that associations do not establish causation.
* **Responsible machine learning decisions:** Concluded that three annual observations and only seven provincial observations for demographic comparisons were insufficient for robust predictive modelling.

</details>

---

## Tools I Use

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" alt="pandas">
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" alt="NumPy">
  <img src="https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn">
  <img src="https://img.shields.io/badge/XGBoost-337AB7?style=flat-square" alt="XGBoost">
  <img src="https://img.shields.io/badge/SHAP-6A5ACD?style=flat-square" alt="SHAP">
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white" alt="Jupyter">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white" alt="Streamlit">
  <img src="https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white" alt="Django">
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git">
</p>

---

## Also Built

**Final-year web application (team of four).** A Django project where I designed the page layout and navigation flow, built most of the frontend, and handled database filling, bug fixing, and integration. Commit history is public.

---

## Currently Building

Exploring telecom and business datasets to apply data analysis and machine learning techniques beyond healthcare and cybersecurity.

---

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=DipeshGhimire33&show_icons=true&hide_border=true&bg_color=0e1c21&title_color=6fb5bd&text_color=e6eef0&icon_color=6fb5bd&radius=6" alt="GitHub stats">
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=DipeshGhimire33&layout=compact&hide_border=true&bg_color=0e1c21&title_color=6fb5bd&text_color=e6eef0&radius=6" alt="Top languages">
</p>
