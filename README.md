# The Overlooked Statistic: Underdiagnosis Among Minorities

🔗 **View Project Website**: [stellacwxxvi.github.io](https://stellacwxxvi.github.io/)

## 📖 Overview

This project investigates disparities in the diagnosis rates of ADHD and learning disabilities among children in the United States, focusing specifically on differences across **race, gender, and socioeconomic status**. Inspired by personal experience and driven by data science, this research aims to surface inequities that may be overlooked in traditional healthcare and educational systems.

## 💡 Motivation

Growing up in predominantly white institutions, I observed that most diagnosed individuals were white, male, and from upper-income families. This project stems from a desire to explore whether those patterns reflect broader structural biases and disparities in diagnostic access and outcomes—especially among young girls and minorities.

## 🧪 Research Questions & Hypotheses

**Main Questions:**
1. Are children from lower-income households under- or over-diagnosed with ADHD or learning disabilities?
2. How do diagnosis rates vary by race and gender?

**Hypotheses:**
- Children from higher-income families will have higher diagnosis rates (❌ Not supported).
- Boys will be diagnosed more frequently than girls (✅ Supported).
- Racial bias influences diagnosis rates (✅ Partially supported, especially for multiracial children).

## 🗂️ Data Source

- **Dataset**: [CDC NHIS 2019–2023](https://www.cdc.gov/nchs/nhis/about/index.html#cdc_survey_profile_collected-whats-collected)
- **Questionnaire**: [Sample Child Questionnaire (PDF)](https://www.cdc.gov/nchs/data/nhis/Sample-Child-Questionnaire.pdf)

This data is publicly available through the CDC/NCHS and focuses on U.S. household survey responses regarding ADHD and learning disabilities in children, segmented by sex, race, and poverty level.

## 🛠️ Tools & Technologies

- **Language**: Python 3
- **Libraries**: `pandas`, `matplotlib`, `numpy`, `json`
- **Source Control**: Git & GitHub
- **Data Source Access**: CDC’s official GitHub repo via `git clone`

## 📊 Analysis Summary

### 1. **Prevalence by Income Level**

Children from low-income households had **consistently higher diagnosis rates** for both ADHD and learning disabilities across all five years. This contradicted the initial hypothesis that high-income children would be diagnosed more frequently due to better healthcare access.

### 2. **Prevalence by Race**

- **Highest Rates**: Children identified as both "Black and White"
- **Lowest Rates**: "Asian only" children
- The data revealed **multiracial children had the highest prevalence**, suggesting racial identity and how it intersects with diagnosis is more nuanced than expected.

### 3. **Prevalence by Sex**

- **Boys were nearly twice as likely** to be diagnosed with ADHD or learning disabilities than girls.
- Girls saw a spike in diagnoses during the COVID-19 pandemic but overall remained underrepresented.

## 📈 Visualizations

- **Line Graphs**: Prevalence trends over time by income, race, and sex
- **Bar Charts**: Mean prevalence comparisons between groups
- **Merged DataFrames**: Combining ADHD and LD rates for clearer comparison

All visualizations were generated with Python and `matplotlib`.

## 🧮 Modeling Questions

### 1. Does poverty level predict diagnosis likelihood?

- **Method**: Linear Regression
- **Goal**: Understand the effect of socioeconomic status over time on diagnosis rates.

### 2. How do race and gender predict diagnosis disparities?

- **Method**: Decision Tree Classifier
- **Goal**: Reveal non-linear patterns in diagnostic rates across demographic intersections.

## 📌 Key Takeaways

| Hypothesis | Supported? | Evidence |
|-----------|------------|----------|
| White, high-income kids are diagnosed more | ❌ No | Low-income groups had higher rates |
| Boys are diagnosed more than girls         | ✅ Yes | Nearly double diagnosis rates |
| Racial bias affects diagnosis rates         | ✅ Partial | Highest rates among multiracial kids |

## 🧠 Reflection

Diagnosis isn't just about healthcare access—**it's about visibility, advocacy, and systemic biases.** Lower-income and under-resourced schools may pursue diagnoses for additional support funding. Cultural stigmas, referral bias, and teacher awareness also shape diagnosis outcomes.

This project helped me realize how public health data can illuminate **inequities hidden within "objective" systems**. There is still much to uncover about how identity shapes diagnosis.

---

## 🚀 How to Reproduce

Clone the CDC dataset and run the notebook:

```bash
git clone https://github.com/HHS-NHIS/SHS_TABLES_CHILDREN.git
cd SHS_TABLES_CHILDREN/www
```

Run the Jupyter notebook or Python script after setting up a suitable environment.
