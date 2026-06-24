# ☕ Global Caffeine Consumption & Health Patterns

**An interactive visualization that maps caffeine, sleep, and lifestyle data onto a human silhouette that responds in real time.**

See it: https://nicholflowers.github.io/Caffeine-Consumption-Health-Patterns/

## 📌 Overview

Caffeine is one of the most widely consumed stimulants in the world, but its relationship to stress varies significantly from person to person. This project turns that relationship into an interactive visualization: a tool that lets anyone adjust caffeine, sleep, age, and lifestyle factors and watch the predicted stress level shift in real time.

## 🎯 Project Goals

- Build an interactive, real-time visualization of how caffeine relates to stress and lifestyle factors
- Make the relationship feel embodied and immediate rather than abstract, so changing one variable visibly shifts the outcome
- Let users explore the data interactively across countries, coffee products, and personal factors

## 🗂️ Dataset

| Source | Description |
| --- | --- |
| [Global Coffee Health Dataset](https://www.kaggle.com/datasets/uom190346a/global-coffee-health-dataset) (Kaggle) | 10,000 synthetic records across 20 countries, covering caffeine intake, stress, sleep, and lifestyle factors. |

## 🎨 The Visualization

The interactive visualization is a human body silhouette that responds in real time to user input. As users adjust caffeine intake, sleep hours, age, smoking status, alcohol use, and physical activity, the silhouette reflects the predicted stress level through a color gradient from blue (low stress) to amber to red (high stress). The color extends across the head, arms, and hands to make the mapping intuitive at a glance.

Animated coffee particles flow through the body, scaling in quantity with caffeine intake, and smoker status triggers visible smoke particles. At high stress levels, the silhouette pulses with a glow effect. The goal was to make the data feel embodied rather than abstract, so users could immediately see how changing one variable shifts the outcome.

**Controls:** selection across 20 countries and 54 coffee products, a caffeine slider (0 to 800 mg), sleep hours, and toggles for smoking, alcohol, and physical activity.

## 🔁 Design Process

The project went through three major iterations, with a usability study informing the final round of refinements.

### 🔹 Iteration 1: Traditional Dashboard

A D3.js dashboard with scatter plots, histograms, heatmaps, and metric cards. It worked for exploring the data but made the relationships between variables difficult to see and compare.

### 🔹 Iteration 2: Interactive Silhouette

The dashboard gave way to the interactive silhouette, driven by a core design question: how do you make someone *feel* the relationship between caffeine and stress rather than just read it off a chart?

### 🔹 Usability Study

Twelve user interviews generated 41 feedback items, which were prioritized with the MoSCoW framework to separate the must-fix issues from lower-priority refinements.

### 🔹 Iteration 3: Usability-Driven Refinements

The prioritized feedback drove a final round of improvements: adding a color legend, making the predicted stress value more prominent, adding context about what the stress percentage represents, correcting the color scheme from green to blue, and preventing caffeine from auto-updating when switching countries.

## 🧠 Skills Demonstrated

- **Interactive data visualization:** building a real-time, input-driven D3.js display that maps several variables onto a single embodied figure
- **Design iteration:** moving from a conventional dashboard to a novel representation when the first approach failed to convey the relationships
- **User research:** running a 12-person usability study and prioritizing 41 findings with the MoSCoW framework
- **Visual encoding:** translating a predicted value into intuitive color, particle, and motion cues

## 🧰 Stack

D3.js, HTML/CSS, JavaScript, GitHub Pages
