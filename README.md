<h1 align="center">Dipesh Ghimire</h1>

<p align="center">
  <a href="https://github.com/DipeshGhimire33/Intern_project">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=1200&color=2B6B73&center=true&vCenter=true&width=700&lines=Messy+data+in.;Trustworthy+models+out.;I+check+the+AI%27s+work." alt="Messy data in. Trustworthy models out. I check the AI's work.">
  </a>
</p>

<p align="center">
  Junior ML engineer (BSc CSIT) · I turn messy, heavily missing, imbalanced data into models that can be trusted.
</p>

<p align="center">
  <a href="https://dipeshghimire33.github.io"><img src="https://img.shields.io/badge/Portfolio-2B6B73?style=for-the-badge&logo=githubpages&logoColor=white" alt="Portfolio"></a>
  <a href="https://dipeshghimire33.github.io/Dipesh_Ghimire_CV.pdf"><img src="https://img.shields.io/badge/Download_CV-B8322A?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="Download CV"></a>
  <a href="https://www.linkedin.com/in/dipesh-ghimire-b00118370/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
</p>

---

## Featured project: sepsis prediction on 1.5M ICU records

An end-to-end machine learning pipeline on the public PhysioNet/CinC 2019 dataset, with a Streamlit demo app. Educational project, not a medical tool.

| | |
|---|---|
| **Data** | 1,552,210 rows from 40,336 ICU patients, 1.8% positive, some lab values up to 99.8% missing |
| **Models compared** | XGBoost, random forest, histogram gradient boosting, logistic regression, linear SVM |
| **Best test result** | XGBoost: PR-AUC 0.093, ROC-AUC 0.791 (random guessing would score about 0.019 PR-AUC) |
| **Code** | [Intern_project](https://github.com/DipeshGhimire33/Intern_project) |

<details>
<summary><b>Where I made the call (click to open)</b></summary>

<br>

- **I overrode the AI on missing values.** It suggested imputing the gaps. I forward-filled within each patient instead, so a patient's last measured value stays theirs until a newer one arrives. A judgment call, not tested against alternatives, and documented as a limitation.
- **I checked the AI on model choice.** I tested its recommendation against four baselines on identical patient-level splits. XGBoost led on PR-AUC and ROC-AUC, while random forest scored slightly higher on F1 and recall, so I report every metric.
- **Safeguard: patient-level splits.** Rows from one patient never sit on both sides of the split, so the score isn't inflated by the model recognising patients.
- **Safeguard: threshold on validation only.** I chose 0.80 on the validation set and applied it unchanged to the test set.

</details>

<details>
<summary><b>What the model can't do (click to open)</b></summary>

<br>

- It catches about a quarter of sepsis observations (recall 0.249), and about 1 in 7 alerts is correct (precision 0.136).
- It has not been validated on another hospital or population.
- The reference ranges behind my features are heuristic, not clinical standards.
- The strongest feature was time in the ICU, which describes model behaviour and not what causes sepsis.

</details>

---

## Tools I use

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

## Also built

**Final-year web application (team of four).** A Django project where I designed the page layout and navigation flow, built most of the frontend, and handled database filling, bug fixing and integration. Commit history is public.

## Currently building

Projects on telecom and business data, to show the same approach outside medicine.

---

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=DipeshGhimire33&show_icons=true&hide_border=true&bg_color=0e1c21&title_color=6fb5bd&text_color=e6eef0&icon_color=6fb5bd&radius=6" alt="GitHub stats">
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=DipeshGhimire33&layout=compact&hide_border=true&bg_color=0e1c21&title_color=6fb5bd&text_color=e6eef0&radius=6" alt="Top languages">
</p>
