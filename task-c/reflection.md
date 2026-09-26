# Task C — Research Reflection

> **BAFAD Accelerated Research Track · Fall 2026**
> Complete **after** finishing Tasks A and B.

---

## Instructions

Write your responses directly in this file (replace the placeholder text).
Aim for **150–200 words total** across both questions.
Be specific — reference your actual experience with the data and code.

---

## Question 1 — Connecting the Work to Research

*After completing Tasks A and B, how does hands-on data exploration relate to the research problem described in **Anomaly Detection in Tactical Sensor Streams** (the document you read before the Canvas quiz)?*

Consider: What patterns did you observe in the SMAP data? How might those patterns complicate or inform the design of an autoencoder-based anomaly detector?

**Your response (75–100 words):**

The SMAP data showed that anomalies were relatively rare, with only 24 of 500 timesteps (4.8%) labeled as anomalous. I also observed substantial overlap between normal and anomalous values in `chan_00`, suggesting that anomalies may not always appear as obvious extreme values in a single channel. This could complicate an autoencoder-based detector because it must learn relationships across multiple channels and over time rather than simply identify unusually high or low values. These patterns suggest training the autoencoder primarily on normal observations and using reconstruction error across multiple telemetry channels to identify unusual multivariate patterns.

---

## Question 2 — Self-Assessment of Readiness

*What specific gaps in your current knowledge — Python skills, statistics concepts, or ML background — do you expect to encounter if you join the research group? What is your plan for addressing them?*

Be honest. There are no wrong answers — this helps us plan the onboarding schedule.

**Your response (75–100 words):**

One gap I expect to encounter is becoming more proficient with Python for statistical analysis and machine learning. I have some experience working with Python and pandas, but I am still developing confidence with more advanced libraries and techniques used to build, train, and evaluate machine-learning models. I also expect to need a deeper understanding of statistical concepts related to anomaly detection, such as model evaluation, threshold selection, class imbalance, and distinguishing meaningful anomalies from normal variation.

---

*Submission: commit this file to your fork and include it in the GitHub repo URL you submit on Canvas.*
