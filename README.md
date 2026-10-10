# Fertilizer Applicator Calibration & Rate Calculator

A simple web app that helps farmers and agricultural engineers check whether a fertilizer applicator is applying the right amount of fertilizer, before it goes into the field.

Built as an Agricultural and Environmental Engineering project: **"Development of a Software-Based Fertilizer Applicator Calibration and Application Rate Calculator for Smallholder Farmers."**

**Live app:** _paste your GitHub Pages link here_

## The problem

An applicator that is not calibrated can:

- **Over-apply** fertilizer, which wastes money and can cause nutrient runoff and leaching into water sources
- **Under-apply** fertilizer, which limits crop yield
- **Apply unevenly**, which causes patchy crop growth

## What it does

| Tab | What it calculates |
|---|---|
| **1. Farm Calculator** | Total fertilizer needed for a field (area × rate) and the number of 50 kg bags to buy |
| **2. Calibration** | The actual application rate from a measured test run, compared with the target rate |
| **3. Ground Speed** | Travel speed in km/h from a timed distance |

The Calibration tab also gives:

- A colour verdict: 🟢 correctly calibrated (within 5% of target), 🟡 slightly low, 🔴 too high
- A gauge bar showing how far the rate is from the target
- An environmental warning when the rate is more than 15% above target

## How the calibration works

1. Effective width = number of outlets × row spacing
2. Effective area = calibration distance × effective width
3. Area in hectares = area in m² ÷ 10,000
4. Application rate = fertilizer collected ÷ area in hectares

**Example:** 20 m distance, 0.8 kg collected, 0.75 m row spacing, 4 outlets
→ width 3.0 m → area 60 m² (0.006 ha) → rate ≈ **133.3 kg/ha**

## How to use it

1. Open the live link in any browser (phone or laptop)
2. Pick a tab and type your values; results update as you type
3. In the Calibration tab, enter your target rate to see the verdict and gauge

## Built with

HTML, CSS and plain JavaScript. There is no database, no server and no libraries.

## Files

- `index.html`: the whole app (page, styles and calculations)
- `manifest.json`, `icon-192.png`, `icon-512.png`: let phones install it as an app

## Author

Oyegbile Oluwatosin Simeon (Matric No. 231327)
