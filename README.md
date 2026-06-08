# Multipartidism and Political Disaffection Among Spanish Youth: A Longitudinal Analysis

This project investigates the relationship between the breakdown of the traditional two-party system in Spain and political disaffection among young citizens. Specifically, it tests whether the emergence of a multipartite system around 2015—marked by the parliamentary arrival of new political actors like *Podemos* and *Ciudadanos* acted as a catalyst to reduce political detachment and increase political interest among the youth.
> **_NOTE:_** Original investigation was written in Spanish.
---

## Table of Contents
- [Hypotheses](#hypotheses)
- [Methodology](#methodology)
- [Key Findings](#key-findings)
- [Conclusions](#conclusion)
- [References](#references)

---

## Hypotheses
**H1:** The transition from a bipartisan to a multiparty system reduced political disaffection among young people in Spain.

---

## Methodology 
The study utilizes data from the European Social Survey (ESS) spanning Rounds 1 through 11 (2002–2023), filtering for respondents in Spain who reached voting age (>= 18 years old) within the surveyed periods. 

- Dependent variable: **Political Disaffection** --> proxied via subjective political interest (polintr), recoded into a binary variable ($1$ = Very/Somewhat interested; $0$ = Little/Not interested).

- Independent Variable: **Political Generations** --> defined by the cohort's first opportunity to vote based on their birth year:

  - Voted before 2011 (Born 1902–1989)
  - Voted in 2011 (Born 1990-1993)
  - Voted in 2015 (Born 1994-1997)
  - Voted in 2019 (Born 1998-2001)
 
### Statistical strategies
*1.* Descriptive analisys

*2.* Graphic visualization

*3.* Exploratory inferential modeling 

### Tools
The analysis was conducted in **Python** (Google Colab environment), using:

- `pandas` and `numpy` for data manipulation,
- `scipy.stats` for hypothesis testing,
- `seaborn` and `matplotlib` for visualization.
  
---
## Key findings
Political interest has steadily ***risen across all generations***, but **younger cohorts show noticeably higher baseline engagement**:
- **Older Generations (Pre-2011):** Show an average interest proportion of 33.3%.
- **The 2019 Cohort:** Displays the highest engagement, with an average of 45.2% of respondents expressing political interest, peaking at nearly 50% in 2023.

However, the logistic regression reveals crucial nuances regarding what actually drives this engagement. Most generational differences are not statistically significant after controlling for time. In that way, the findings provide evidence of a strong period effect rather than a clear cohort effect.

In fact, political interest increased among virtually all generations during the years surrounding the 2008 economic crisis and the 15-M movement (2011). Although younger cohorts tend to exhibit higher levels of political interest, the data do not provide sufficient evidence to conclude that multipartism itself was the primary cause of this increase.

Instead, the rise in political interest appears more closely associated with broader cycles of ***political mobilization*** and social conflict that ***preceded*** the formal collapse of the bipartisan party system.

### Figure 1: Evolution of political interests (2002 - 2023)
![lineplot]()

---
## Conclusion
The initially proposed hypothesis (H1) requires a critical nuance. There is insufficient evidence to claim that the drop in political disaffection was a direct consequence of institutional multipartidism. Rather, political interest increased across society as a whole, suggesting that the most important mechanism was a general period effect linked to political mobilization and crisis, rather than a lasting generational effect produced by the new party system.

This takeaway is reinforced by the fact that the sharpest increase in political interest occurred between 2010 and 2014, heavily influenced by the social mobilization cycles following the 2008 financial crisis (such as the 15-M Movement in 2011).

However, the 2019 Generation stands out as an anomaly: they maintained remarkably high political interest and were the only group whose engagement increased during the COVID-19 pandemic, suggesting they might have uniquely benefited from political socialization entirely embedded within a highly competitive, multi-party environment.

Future research should explore:

Age–period–cohort dynamics;
The impact of the COVID-19 pandemic;
Party identification and ideology;
Whether the higher political interest observed among the 2019 cohort persists over time.

---
## References 
– Bauman, Z. (2003). Modernidad líquida. Fondo de Cultura Económica.

– Constant, B. (1989). De la libertad de los antiguos comparada con la de los modernos. Alianza Editorial.

– Forniés, Á. A. (2011). Causas y riesgos de la desafección política de los jóvenes. In Jornadas la desafección política en la juventud española tras treinta años de vigencia de la construcción (pp. 2-10). Fundación Manuel Giménez Abad de Estudios Parlamentarios y del Estado Autonómico.

– Montero, J. R., Gunther, R., Torcal, M., & Menezo, J. C. (1998). Actitudes hacia la democracia en España: legitimidad, descontento y desafección. Reis, 9-49.

– Putnam, R. D. (2000). Bowling alone: The collapse and revival of American community. Simon and schuster.

– Sotillos, I. D. (2020). La formación de gobiernos en sistemas multipartidistas: la paradoja del caso español. Teoría y realidad constitucional, (45), 261-290.

– Tocqueville, A. de. (2005). La democracia en América. Alianza Editorial.
