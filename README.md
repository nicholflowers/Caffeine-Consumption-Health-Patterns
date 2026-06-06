# Caffeine-Consumption-Health-Patterns

An interactive visualization exploring how caffeine intake relates to stress, sleep, and lifestyle factors across 20 countries.

## Overview

Caffeine is one of the most widely consumed stimulants in the world, but its relationship to stress varies significantly by person. This project visualizes how caffeine connects to stress levels and how factors like country, age, sleep, and physical activity shape that relationship.

## The Visualization

The centerpiece is a human body silhouette that responds in real time to user inputs. As users adjust caffeine intake, sleep hours, age, smoking status, alcohol use, and physical activity, the silhouette reflects the predicted stress level through a color gradient from blue (low stress) to amber to red (high stress). The color extends across the head, arms, and hands to make the mapping intuitive at a glance.

Animated coffee particles flow through the body, scaling in quantity with caffeine intake. Smoker status triggers visible smoke particles. At high stress levels, the silhouette pulses with a glow effect. The goal was to make the data feel embodied rather than abstract, so users could immediately see how changing one variable shifts the outcome.

Controls include selection across 20 countries and 54 coffee products, a caffeine slider (0-800mg), sleep hours, and toggles for smoking, alcohol, and physical activity.

## Design Process

The project went through two major iterations.

**Iteration 1** was a traditional D3.js dashboard with scatter plots, histograms, heatmaps, and metric cards. It worked for exploring the data but made the relationships between variables difficult to see and compare.

**Iteration 2** replaced the dashboard with the interactive silhouette. The shift was driven by a core design question: how do you make someone feel the relationship between caffeine and stress rather than just read it off a chart?

**Usability Study:** 12 user interviews (3 per team member) generated 41 feedback items prioritized using the MoSCoW framework. Key fixes included adding a color legend, making the predicted stress value more prominent, adding context about what the stress percentage represents, correcting the color scheme from green to blue, and preventing caffeine from auto-updating when switching countries.

## Data

Global Coffee Health Dataset from Kaggle (10,000 synthetic records across 20 countries).

## Stack

D3.js, HTML/CSS, JavaScript, GitHub Pages
