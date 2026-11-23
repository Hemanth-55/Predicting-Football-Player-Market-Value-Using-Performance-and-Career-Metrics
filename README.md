<p align="center">
  <img src="assets/header.svg" alt="Football Player Market Value Model: R² 0.612, about 80% better than linear baselines, €1.7M less error per player, 64 undervalued targets." width="620">
</p>

<h1 align="center">Predicting Football Player Market Value</h1>

<p align="center">
  <img src="https://img.shields.io/badge/R²-0.612-FFB547?style=for-the-badge&labelColor=04060B" alt="R² 0.612">
  <img src="https://img.shields.io/badge/vs%20linear%20baselines-~80%25%20better-35E0FF?style=for-the-badge&labelColor=04060B" alt="About 80% better than linear baselines">
  <img src="https://img.shields.io/badge/undervalued%20targets-64-FFB547?style=for-the-badge&labelColor=04060B" alt="64 undervalued targets">
  <img src="https://img.shields.io/badge/Python-04060B?style=for-the-badge&logo=python&logoColor=35E0FF" alt="Python">
</p>

A machine learning project that predicts a football (soccer) player's **market value** from performance and career data across top European leagues, then uses the gap between model value and market value to find **players the market may be undervaluing**.

## ⚽ The question

Transfer fees are huge and noisy. A club's scouting team can't watch every player in every league. Can a model point them to the players whose performance is worth more than their price tag?

## 🧠 Approach

| Step | What I did | Why |
|---|---|---|
| Data | Player performance and career metrics across top European leagues | One consistent view of players across competitions |
| Feature engineering | **Log-transformed** skewed features | A few superstar valuations dominate the raw scale |
| Rebalancing | **SMOTE** to rebalance under-represented groups in the training data | Keeps the model from only learning the common cases |
| Models | **Gradient Boosting**, tested against linear baselines | Captures non-linear effects that linear models miss |
| Scouting output | Ranked players where model value is clearly above market value | Turns predictions into a shortlist a scout can use |

## 📊 Results

| Metric | Result |
|---|---|
| R² (Gradient Boosting) | **0.612** |
| Improvement over linear baselines | **~80%** |
| Valuation error reduction | **€1.7M per player** |
| Undervalued transfer targets identified | **64** |

## 🏟️ Why it matters

The model doesn't replace scouts. It helps them decide where to look first: 64 players whose numbers say they are worth a closer look than their market price suggests.

## 🗂️ Status

The code and notebook will be added to this repository soon.

---

<p align="center"><sub>Part of my sports analytics work · <a href="https://hemanthkumargopi.vercel.app">hemanthkumargopi.vercel.app</a> · <a href="https://github.com/Hemanth-55">@Hemanth-55</a></sub></p>
