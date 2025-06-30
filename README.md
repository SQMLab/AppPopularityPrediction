# App Popularity Prediction

This repository contains the dataset and code for the research paper:

**Can Internal Software Metrics Predict App Popularity at Launch? Yeas! and Nays!**

---

## 📖 Overview

The goal of this project is to investigate whether an app’s popularity can be predicted before launch using only internal software metrics and metadata, without relying on historical popularity data. The dataset includes metrics extracted from the source code of 446 open-source Android apps along with metadata and popularity indicators from the Google Play Store.

---

## 📂 Dataset Description

### 🔹 Source

- **Apps:** Open-source Android apps collected from [F-Droid](https://f-droid.org).
- **Popularity Indicators:** User ratings computed from user reviews and yearly download counts from the Google Play Store.
- **Source Code:** Oldest available version per app to approximate first release collected from [F-Droid](https://f-droid.org).

### 🔹 Contents

The dataset combines three main feature groups:

1️⃣ **Code Metrics**

- **System-Level:** 17 architectural metrics (decoupling, propagation cost, modularity, anti-patterns) via the DV8 tool.
- **Class-Level:** 652 features based on Chidamber & Kemerer (CK) metrics suite and structural attributes.
- **Method-Level:** 406 features covering complexity, fan-in/out, readability, control structures, etc.

2️⃣ **Code Smells**

- 34 design and architectural smells detected with DesigniteJava (e.g., God Class, Cyclic Dependency).

3️⃣ **App Metadata**

- **Genre:** App category (e.g., GAME, FINANCE, SOCIAL, etc.).
- **Ads:** Binary flag for advertisement presence.
- **Permissions:** System permissions requested (e.g., Camera, Location).
- **Activity Count:** Number of declared Android Activities.

### 🔹 Target Variables

- **Average User Rating** (computed from user reviews).
- **DownloadsPerYear** (download count normalized by app age).

---

**SQM Research Lab · University of Manitoba**
