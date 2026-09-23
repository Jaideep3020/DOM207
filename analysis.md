# Statistical Analysis Report

> Generated from MP_1.ipynb — contains all cases where H0 was **rejected** (p < 0.05)
> Tip-based findings are deferred pending verification of extreme entries (see audit flags).

---

## Part 1 — ANOVA Significant Findings

### Finding 1: CASE 1.1: **Amount** by Day

> **Test Statistics:** F = 3.004 | p = 0.030501

**Observation & Analysis**

One-way ANOVA detected a significant effect of **Day** on **Amount** (F=3.004, p=0.030501). Group breakdown — Sun (n=114, mean=22.80, total=2599.47, 34.6%); Sat (n=117, mean=21.64, total=2532.04, 33.7%); Fri (n=38, mean=21.03, total=798.95, 10.6%); Thur (n=87, mean=18.28, total=1590.62, 21.1%). The highest average Amount is in the **Sun** group (22.80) and the lowest in the **Thur** group (18.28), a difference of **4.52**. The Sun group contributes **34.6%** of total Amount (2599.47 / 7521.08).

**Managerial Insight**

Since **Day** significantly influences **Amount**, prioritise the **Sun** category for operational and revenue strategies. The **Thur** group shows the lowest average Amount (18.28); targeted interventions there could close the **4.52-unit gap** with the best-performing group.

---

### Finding 2: CASE 1.3: **Amount** by PartyGroup

> **Test Statistics:** F = 27.885 | p = < 0.000001

**Observation & Analysis**

One-way ANOVA detected a significant effect of **PartyGroup** on **Amount** (F=27.885, p=< 0.000001). Group breakdown — Medium [3-4] (n=131, mean=25.90, total=3392.58, 45.1%); Large [5+] (n=19, mean=25.46, total=483.68, 6.4%); Small [1-2] (n=206, mean=17.69, total=3644.82, 48.5%). The highest average Amount is in the **Medium [3-4]** group (25.90) and the lowest in the **Small [1-2]** group (17.69), a difference of **8.20**. The Medium [3-4] group contributes **45.1%** of total Amount (3392.58 / 7521.08).

**Managerial Insight**

Since **PartyGroup** significantly influences **Amount**, prioritise the **Medium [3-4]** category for operational and revenue strategies. The **Small [1-2]** group shows the lowest average Amount (17.69); targeted interventions there could close the **8.20-unit gap** with the best-performing group.

---

### Finding 3: CASE 2.2: **Amount** by Smoker & Gender

> **Test Statistics:** Significant terms: Smoker (F=4.335, p=0.038057)

**Observation & Analysis**

Two-way ANOVA found significant effects on **Amount** — significant term(s): Smoker (F=4.335, p=0.038057). Across **Smoker**: Yes mean=22.68; No mean=20.15. Across **Gender**: Male mean=21.62; Female mean=20.44. These effects indicate that both **Smoker** and **Gender** (and possibly their interaction) shape the **Amount** outcome.

**Managerial Insight**

The combination of **Smoker** and **Gender** jointly drives **Amount**. Within Smoker, the **Yes** level yields the highest average (22.68); within Gender, **Male** leads (21.62). Prioritise the **Yes × Male** combination for maximum Amount impact, and review the lowest-performing levels of each factor for targeted improvement opportunities.

---

## Part 2 — T-Test Significant Findings

### Finding 1: Amount | grouped by **Tip** (> 2.88 vs <= 2.88)

> **Test Statistics:** t = 9.4636 | p = < 0.000001 | Δμ = 9.8168 | 95% CI = [7.7744, 11.8591]

**Observation & Analysis**

The bar chart comparison of total **Amount** shows that the **> 2.88** group accounts for **4613.08** in total Amount (from 177 records) with an average of **26.06** per record, while the **<= 2.88** group accounts for **2908.00** total (from 179 records) with an average of **16.25** per record. The dataset records **7521.08** in combined Amount (4613.08 / 7521.08, **~61.3%** from > 2.88). After Welch's independent-samples t-test, a statistically significant difference was observed (t=9.4636, p=< 0.000001), indicating that **Tip** exerts a measurable effect on **Amount**.

**Managerial Insight**

Because the **> 2.88** group produces a higher average Amount (~26.06 vs ~16.25 for <= 2.88), prioritise operational and revenue strategies for the **> 2.88** segment. For the **<= 2.88** group (~16.25 average), consider targeted interventions to close the **9.82-unit gap** with the better-performing segment.

---

### Finding 2: Amount | grouped by **Partysize** (Large (>2) vs Small (<=2))

> **Test Statistics:** t = 7.7208 | p = < 0.000001 | Δμ = 8.1484 | 95% CI = [6.0727, 10.2241]

**Observation & Analysis**

The bar chart comparison of total **Amount** shows that the **Large (>2)** group accounts for **3876.26** in total Amount (from 150 records) with an average of **25.84** per record, while the **Small (<=2)** group accounts for **3644.82** total (from 206 records) with an average of **17.69** per record. The dataset records **7521.08** in combined Amount (3876.26 / 7521.08, **~51.5%** from Large (>2)). After Welch's independent-samples t-test, a statistically significant difference was observed (t=7.7208, p=< 0.000001), indicating that **Partysize** exerts a measurable effect on **Amount**.

**Managerial Insight**

Because the **Large (>2)** group produces a higher average Amount (~25.84 vs ~17.69 for Small (<=2)), prioritise operational and revenue strategies for the **Large (>2)** segment. For the **Small (<=2)** group (~17.69 average), consider targeted interventions to close the **8.15-unit gap** with the better-performing segment.

---

### Finding 3: Amount | grouped by **Time** (Dinner vs Lunch)

> **Test Statistics:** t = 2.0965 | p = 0.036767 | Δμ = 2.2871 | 95% CI = [0.1414, 4.4327]

**Observation & Analysis**

The bar chart comparison of total **Amount** shows that the **Dinner** group accounts for **4922.32** in total Amount (from 224 records) with an average of **21.97** per record, while the **Lunch** group accounts for **2598.76** total (from 132 records) with an average of **19.69** per record. The dataset records **7521.08** in combined Amount (4922.32 / 7521.08, **~65.4%** from Dinner). After Welch's independent-samples t-test, a statistically significant difference was observed (t=2.0965, p=0.036767), indicating that **Time** exerts a measurable effect on **Amount**.

**Managerial Insight**

Because the **Dinner** group produces a higher average Amount (~21.97 vs ~19.69 for Lunch), prioritise operational and revenue strategies for the **Dinner** segment. For the **Lunch** group (~19.69 average), consider targeted interventions to close the **2.29-unit gap** with the better-performing segment.

---

### Finding 4: Amount | grouped by **Day** (Weekend vs Weekday)

> **Test Statistics:** t = 2.8729 | p = 0.004327 | Δμ = 3.0978 | 95% CI = [0.9767, 5.2188]

**Observation & Analysis**

The bar chart comparison of total **Amount** shows that the **Weekend** group accounts for **5131.51** in total Amount (from 231 records) with an average of **22.21** per record, while the **Weekday** group accounts for **2389.57** total (from 125 records) with an average of **19.12** per record. The dataset records **7521.08** in combined Amount (5131.51 / 7521.08, **~68.2%** from Weekend). After Welch's independent-samples t-test, a statistically significant difference was observed (t=2.8729, p=0.004327), indicating that **Day** exerts a measurable effect on **Amount**.

**Managerial Insight**

Because the **Weekend** group produces a higher average Amount (~22.21 vs ~19.12 for Weekday), prioritise operational and revenue strategies for the **Weekend** segment. For the **Weekday** group (~19.12 average), consider targeted interventions to close the **3.10-unit gap** with the better-performing segment.

---

### Finding 5: Gender (Male=1) | grouped by **Time** (Dinner vs Lunch)

> **Test Statistics:** t = 4.4432 | p = 0.000013 | Δμ = 0.2378 | 95% CI = [0.1324, 0.3432]

**Observation & Analysis**

The bar chart comparison of total **Gender (Male=1)** shows that the **Dinner** group accounts for **150.00** in total Gender (Male=1) (from 224 records) with an average of **0.67** per record, while the **Lunch** group accounts for **57.00** total (from 132 records) with an average of **0.43** per record. The dataset records **207.00** in combined Gender (Male=1) (150.00 / 207.00, **~72.5%** from Dinner). After Welch's independent-samples t-test, a statistically significant difference was observed (t=4.4432, p=0.000013), indicating that **Time** exerts a measurable effect on **Gender (Male=1)**.

**Managerial Insight**

Because the **Dinner** group produces a higher average Gender (Male=1) (~0.67 vs ~0.43 for Lunch), prioritise operational and revenue strategies for the **Dinner** segment. For the **Lunch** group (~0.43 average), consider targeted interventions to close the **0.24-unit gap** with the better-performing segment.

---

### Finding 6: Time (Dinner=1) | grouped by **Tip** (> 2.88 vs <= 2.88)

> **Test Statistics:** t = 3.2506 | p = 0.001263 | Δμ = 0.1644 | 95% CI = [0.0649, 0.2638]

**Observation & Analysis**

The bar chart comparison of total **Time (Dinner=1)** shows that the **> 2.88** group accounts for **126.00** in total Time (Dinner=1) (from 177 records) with an average of **0.71** per record, while the **<= 2.88** group accounts for **98.00** total (from 179 records) with an average of **0.55** per record. The dataset records **224.00** in combined Time (Dinner=1) (126.00 / 224.00, **~56.2%** from > 2.88). After Welch's independent-samples t-test, a statistically significant difference was observed (t=3.2506, p=0.001263), indicating that **Tip** exerts a measurable effect on **Time (Dinner=1)**.

**Managerial Insight**

Because the **> 2.88** group produces a higher average Time (Dinner=1) (~0.71 vs ~0.55 for <= 2.88), prioritise operational and revenue strategies for the **> 2.88** segment. For the **<= 2.88** group (~0.55 average), consider targeted interventions to close the **0.16-unit gap** with the better-performing segment.

---

### Finding 7: Time (Dinner=1) | grouped by **Gender** (Male vs Female)

> **Test Statistics:** t = 4.4225 | p = 0.000014 | Δμ = 0.2280 | 95% CI = [0.1265, 0.3295]

**Observation & Analysis**

The bar chart comparison of total **Time (Dinner=1)** shows that the **Male** group accounts for **150.00** in total Time (Dinner=1) (from 207 records) with an average of **0.72** per record, while the **Female** group accounts for **74.00** total (from 149 records) with an average of **0.50** per record. The dataset records **224.00** in combined Time (Dinner=1) (150.00 / 224.00, **~67.0%** from Male). After Welch's independent-samples t-test, a statistically significant difference was observed (t=4.4225, p=0.000014), indicating that **Gender** exerts a measurable effect on **Time (Dinner=1)**.

**Managerial Insight**

Because the **Male** group produces a higher average Time (Dinner=1) (~0.72 vs ~0.50 for Female), prioritise operational and revenue strategies for the **Male** segment. For the **Female** group (~0.50 average), consider targeted interventions to close the **0.23-unit gap** with the better-performing segment.

---

### Finding 8: Time (Dinner=1) | grouped by **Day** (Weekend vs Weekday)

> **Test Statistics:** t = 10.2556 | p = < 0.000001 | Δμ = 0.5012 | 95% CI = [0.4049, 0.5975]

**Observation & Analysis**

The bar chart comparison of total **Time (Dinner=1)** shows that the **Weekend** group accounts for **186.00** in total Time (Dinner=1) (from 231 records) with an average of **0.81** per record, while the **Weekday** group accounts for **38.00** total (from 125 records) with an average of **0.30** per record. The dataset records **224.00** in combined Time (Dinner=1) (186.00 / 224.00, **~83.0%** from Weekend). After Welch's independent-samples t-test, a statistically significant difference was observed (t=10.2556, p=< 0.000001), indicating that **Day** exerts a measurable effect on **Time (Dinner=1)**.

**Managerial Insight**

Because the **Weekend** group produces a higher average Time (Dinner=1) (~0.81 vs ~0.30 for Weekday), prioritise operational and revenue strategies for the **Weekend** segment. For the **Weekday** group (~0.30 average), consider targeted interventions to close the **0.50-unit gap** with the better-performing segment.

---

### Finding 9: Day (Weekend=1) | grouped by **Tip** (> 2.88 vs <= 2.88)

> **Test Statistics:** t = 2.0387 | p = 0.042229 | Δμ = 0.1028 | 95% CI = [0.0036, 0.2020]

**Observation & Analysis**

The bar chart comparison of total **Day (Weekend=1)** shows that the **> 2.88** group accounts for **124.00** in total Day (Weekend=1) (from 177 records) with an average of **0.70** per record, while the **<= 2.88** group accounts for **107.00** total (from 179 records) with an average of **0.60** per record. The dataset records **231.00** in combined Day (Weekend=1) (124.00 / 231.00, **~53.7%** from > 2.88). After Welch's independent-samples t-test, a statistically significant difference was observed (t=2.0387, p=0.042229), indicating that **Tip** exerts a measurable effect on **Day (Weekend=1)**.

**Managerial Insight**

Because the **> 2.88** group produces a higher average Day (Weekend=1) (~0.70 vs ~0.60 for <= 2.88), prioritise operational and revenue strategies for the **> 2.88** segment. For the **<= 2.88** group (~0.60 average), consider targeted interventions to close the **0.10-unit gap** with the better-performing segment.

---

### Finding 10: Day (Weekend=1) | grouped by **Partysize** (Large (>2) vs Small (<=2))

> **Test Statistics:** t = 2.4453 | p = 0.014986 | Δμ = 0.1229 | 95% CI = [0.0240, 0.2218]

**Observation & Analysis**

The bar chart comparison of total **Day (Weekend=1)** shows that the **Large (>2)** group accounts for **108.00** in total Day (Weekend=1) (from 150 records) with an average of **0.72** per record, while the **Small (<=2)** group accounts for **123.00** total (from 206 records) with an average of **0.60** per record. The dataset records **231.00** in combined Day (Weekend=1) (108.00 / 231.00, **~46.8%** from Large (>2)). After Welch's independent-samples t-test, a statistically significant difference was observed (t=2.4453, p=0.014986), indicating that **Partysize** exerts a measurable effect on **Day (Weekend=1)**.

**Managerial Insight**

Because the **Large (>2)** group produces a higher average Day (Weekend=1) (~0.72 vs ~0.60 for Small (<=2)), prioritise operational and revenue strategies for the **Large (>2)** segment. For the **Small (<=2)** group (~0.60 average), consider targeted interventions to close the **0.12-unit gap** with the better-performing segment.

---

### Finding 11: Day (Weekend=1) | grouped by **Time** (Dinner vs Lunch)

> **Test Statistics:** t = 10.1033 | p = < 0.000001 | Δμ = 0.4894 | 95% CI = [0.3940, 0.5849]

**Observation & Analysis**

The bar chart comparison of total **Day (Weekend=1)** shows that the **Dinner** group accounts for **186.00** in total Day (Weekend=1) (from 224 records) with an average of **0.83** per record, while the **Lunch** group accounts for **45.00** total (from 132 records) with an average of **0.34** per record. The dataset records **231.00** in combined Day (Weekend=1) (186.00 / 231.00, **~80.5%** from Dinner). After Welch's independent-samples t-test, a statistically significant difference was observed (t=10.1033, p=< 0.000001), indicating that **Time** exerts a measurable effect on **Day (Weekend=1)**.

**Managerial Insight**

Because the **Dinner** group produces a higher average Day (Weekend=1) (~0.83 vs ~0.34 for Lunch), prioritise operational and revenue strategies for the **Dinner** segment. For the **Lunch** group (~0.34 average), consider targeted interventions to close the **0.49-unit gap** with the better-performing segment.

---
