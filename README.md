🚀 Overview

This project analyzes system metrics — CPU, Memory, Network In, and Network Out — to detect abnormal system behavior without ground-truth labels.

Two complementary approaches were implemented:

Statistical Baseline: Rolling Mean + Rolling Standard Deviation

Model-Based Detection: Isolation Forest

The goal is to identify spikes, drops, contextual anomalies, and multivariate inconsistencies in system performance.

🛠️ Methods Used
1️⃣ Statistical Detection

Rolling window baseline

±3σ anomaly thresholds

Time-aware deviation detection

2️⃣ Model-Based Detection

Isolation Forest

Multivariate anomaly detection

Distribution-agnostic modeling

📈 Key Insights

CPU anomalies are spike-driven with narrow variance.

Memory anomalies often appear as gradual shifts or sudden drops.

Network metrics are highly volatile; only extreme bursts are anomalous.

Both methods detect different anomaly types → complementary coverage.

📊 Evaluation Strategy

Since no labels exist, anomalies were validated using:

Time-series visualization

Distribution analysis

Cross-method overlap

Infrastructure behavior alignment
