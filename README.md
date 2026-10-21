# econ3916-lab08-hypothesis-testing
Lab 08 submission
# Hypothesis Testing — Is Job Training Worth It?

## Objective
I tested whether the National Supported Work job training program raised participants' earnings, and whether the effect was large enough and reliable enough to matter.

## Methodology
- I loaded the LaLonde NSW job training experiment (445 people: 185 trainees and 260 controls).
- I ran a one-sample t-test and a two-sample Welch's t-test on 1978 earnings.
- I wrote Welch's t-statistic as a function, welch_t(), and checked it against scipy on the full sample and on five subgroups.
- I computed Cohen's d to judge the size of the effect, not only whether it is significant.
- I ran a power analysis: the power of this study, and the sample size needed to detect d = 0.3.
- I tested the treatment effect in 5 overlapping demographic subgroups, then applied Bonferroni and Benjamini-Hochberg corrections.
- I simulated p-value distributions when the null is true and when it is false.

## Key Findings
- Trainees earned $1,794.34 more in 1978 than controls (Welch's t = 2.6741, p = 0.0079).
- The effect is statistically significant but small: a Cohen's d of 0.27, about a quarter of a standard deviation.
- 2 of the 5 subgroup effects were significant before correction, and 1 after Bonferroni.
