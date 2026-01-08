# 🌊 Toxic Waters: Marine Pollution & Phytoplankton

**How microplastics and human activity are reshaping the lungs of our oceans**

---

## Why This Matters

Phytoplankton may be microscopic, but their impact is planetary. They generate **over 50% of Earth’s oxygen**, regulate global climate, and anchor the marine food web. Today, these organisms face mounting pressure from **microplastic pollution** and **intensifying human activity**.

This project explores how pollution and fishing behavior intersect with phytoplankton health at a **global, multi-decade scale**.

---

## 🎯 Project Objectives

This study investigates three tightly linked questions:

* **Marine Health:** Does increasing plastic density correlate with declining phytoplankton levels?
* **Human Behavior:** Do commercial fishing vessels avoid highly polluted ocean regions—or continue operating regardless?
* **Long-Term Change:** How have these relationships evolved over the last 50 years?

---

## 📊 Data at a Glance

We integrate **three large-scale global datasets** to capture biological, environmental, and human dynamics.

| Dataset             | Time Span | Source               | Key Variables                  |
| ------------------- | --------- | -------------------- | ------------------------------ |
| **Microplastics**   | 1972–2022 | NCEI                 | Plastic density, coordinates   |
| **Phytoplankton**   | 1958–2017 | PANGAEA              | Chlorophyll-a, SST             |
| **Fishing Vessels** | 2012–2020 | Global Fishing Watch | Fishing hours, vessel location |

In total, the pipeline processes **56+ million rows of spatiotemporal data**.

---

## 🛠️ Methodology

The analysis was built entirely in **Python**, emphasizing scalability and reproducibility.

### 1. Data Engineering

* Cleaned metadata and handled missing values
* Standardized spatial coordinates (latitude/longitude)
* Aligned datasets across time and space

### 2. Temporal Analysis

To capture long-term trends, data were segmented into three eras:

* **1973–2000:** Pre-globalization baseline
* **2001–2010:** Rapid industrial expansion
* **2011–2022:** Modern high-impact period

### 3. Spatial Modeling

* Used **GeoPandas** to map fishing density
* Overlaid vessel activity with known plastic accumulation zones

### 4. Environmental Correlation

* Modeled **chlorophyll-a** as a proxy for phytoplankton health
* Tested correlations between plastic density, temperature, and biological decline

---

## 💡 Key Findings

### 📉 Global Decline

Phytoplankton levels show a **consistent downward trend** across most ocean basins.

### 🧪 Plastic vs. Biology

* Plastic density correlates with reduced chlorophyll-a
* The relationship is **not yet statistically significant**, suggesting compounding stressors such as warming oceans

### 🚢 Human Behavior

Commercial fishing effort shows **no measurable decline** in heavily polluted regions.

> Economic activity continues—even where environmental degradation is most severe.

---

## 🚀 Getting Started

### Prerequisites

Ensure the following packages are installed:

* `pandas`
* `numpy`
* `matplotlib`
* `geopandas`

### Installation

```bash
git clone https://github.com/[your-username]/marine-pollution-plankton.git
cd marine-pollution-plankton
pip install pandas numpy matplotlib geopandas
```

### Run the Analysis

```bash
jupyter notebook cs252a_fishFood.ipynb
```

---

## 🔭 Future Work

* Incorporate **causal modeling** (e.g., panel regressions)
* Add **ocean circulation data** to track plastic transport
* Extend analysis to **species-level biodiversity impacts**

---

## 📌 Takeaway

This project highlights a critical disconnect: **marine ecosystems are deteriorating, yet human activity remains unchanged**. Understanding—and visualizing—this gap is a necessary step toward informed policy and sustainable ocean management.

---

*CS252A · Environmental Data Science · Global Ocean Health*
