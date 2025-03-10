# Does Income Affect Women's Health Spending? Evidence from India's Formal Sector

# Abstract
This paper examines how women's control over income affects household health investment
decisions by exploiting a 2018 policy change in India that increased take-home pay for women in
the formal sector. Using household-level panel data from 2016-2019, I implement a
difference-in-differences strategy comparing female-majority households in formal versus
informal employment. Results show that beneficiary households increased health expenditure by
1.9% following the policy change. This increase was primarily driven by preventive care, with a
5.9% rise in health enhancement spending and a 3.4% increase in health insurance premiums,
while spending on immediate medical needs showed minimal changes. The effects were
strongest immediately following the policy implementation but declined over time. Analysis of
household characteristics reveals that education levels strongly influence health spending
patterns, with high-education households spending 24% more than basic-education households.
These findings suggest that while increased income prompts higher health investments by
women, the sustainability of these changes may depend on household characteristics and
competing consumption priorities.

# Introduction
Traditional economics has largely focused on understanding and modeling individual
decision-making, in that they assume rational consumers base their decisions in order to
maximise their objective function, given their budget constraint (Almås et al., 2023). However,
some of the most important decisions on allocation of resources are not taken individually, but
within the family. As Agarwal et al. (2022a) points out, research on intra household decision
making exists in various contexts, and is useful to study the distributional effects of public
policies in developing country contexts. We extend this framework by arguing that public
policies can serve as a lens to examine how increased resource control affects household health
investment decisions.

Understanding how households allocate additional income to health investments is crucial for
policy design in developing countries. While extensive research has examined the relationship
between income and health spending, less attention has been paid to how gender shapes these
investment decisions. This gap is particularly relevant in contexts where women's healthcare
access and decision-making power are constrained by social and economic factors (Agarwal et
al., 2022b). Maxwell and Vaishnavi (2011) point out that one of the ways to determine the degree
of agency a woman holds is by studying the extent of their influence in household resource
allocation. They find that there is a positive association between working women and household
decision making.

Building on this literature linking women's employment to household decision-making power,
we examine how formal sector employment—and specifically, changes in women's take-home
pay—affects health investment decisions. The formal sector context is particularly relevant as it
provides both increased income and potentially greater autonomy in spending decisions.
This paper examines how women's health spending responds to increased income by exploiting a
2018 policy change in India that effectively raised take-home pay for women in the formal
sector. Our analysis focuses on three key dimensions: the types of health investments women
prioritize when given additional resources, how household characteristics like education and age
composition influence these choices, and how spending patterns evolve over time after an
income shock.

Several features make this setting particularly suitable for examining women's health investment
decisions. First, India's mixed healthcare system, with both public and private options, allows us
to observe discretionary health spending choices. Second, the formal sector context provides a
well-defined treatment group with clear policy exposure. Third, our detailed household-level
data enables analysis of different types of health spending, from preventive care to curative
treatments.

We find that, given an increase in income, female-headed households in the formal sector
increase their health expenditure by 1.9% compared to households in the informal sector, with a
focus on preventative, long-term health expenditure, although we see a declining effect over
time. Our findings contribute to understanding how income changes translate into health
investments, particularly in contexts where women's healthcare decisions intersect with formal
employment, education, and household dynamics. This has important implications for policies
aimed at improving women's health outcomes through economic empowerment.

# Methodology
## Data Sources
Consumer Pyramid Household Survey

The study uses longitudinal household level survey data from Consumer Pyramid Household
Index from the Center for Monitoring Indian Economy which comprises 174,000 sample
households all across 28 states and 514 districts in India collected triannually. The paper obtains
data from January 2016 to December 2019, providing both pre and post-policy implementation
periods. The CPHS offers several advantages for our analysis. It has detailed expenditure data
across multiple categories including health, leisure, and education, and includes rich household
characteristics including age composition, education levels, and region type. Particularly, it
provides granular health expenditure data broken down into components such as medical
treatments, preventive care, and health enhancement which is helpful for our analysis.

## Two-way fixed effects Difference in Difference Approach
This study employs a two-way fixed effects difference-in-differences (DiD) design to estimate
the causal effect of increased income on health expenditure. The baseline specification is:
Log(Health Expenditure)ᵢ􀀀 = β₀ + β₁Beneficiaryᵢ + β₂Post2018􀀀 + β₃(Beneficiary × Post2018)ᵢ􀀀
+ δᵢ + γ􀀀 + εᵢ􀀀
Where i indexes households and t indexes time (months), Beneficiaryᵢ indicates formal sector
employment which takes the value of 1 for households with majority of females in the formal
sector and 0, otherwise. Post2018􀀀 indicates periods after the policy implementation and takes
the value of 1 where data is prior to February 2018, and 0 otherwise. δᵢ represents household
fixed effects, and γ􀀀 represents time fixed effects. The main coefficient of interest is β₃,
measuring the differential change in health expenditure for beneficiary households after the
policy was implemented. The household fixed effects (δᵢ) control for time-invariant household
characteristics that might affect health expenditure patterns. The time fixed effects (γ􀀀) account
for temporal shocks affecting all households. The study uses logarithmic transformation of the
dependent variable to address skewness in expenditure data and interpret coefficients as
percentage changes.

The baseline model is further augmented with household characteristics:
Log(Health Expenditure)ᵢ􀀀 = β₀ + β₃(Beneficiary × Post2018)ᵢ􀀀 + β₄EduGroupᵢ􀀀 +
β₅AgeGroupᵢ􀀀 + δᵢ + γ􀀀 + εᵢ􀀀

Drawing from prior literature and a DAG approach, we include household education and age
composition as key covariates. Our DAG analysis reveals that both education and household age
composition act as confounders in the relationship between income and health expenditure. This
specification includes education group fixed effects to control for variation in health awareness
and decision-making capacity, age group composition to account for lifecycle differences in
health needs (Vikram and Vanneman, 2019; Parinduri, 2016; Chowdhury et al., 2018). The
importance of controlling for these confounders is evident in our model progression, where the
treatment effect changes from -1.3% to +2.1% after including age controls, suggesting
significant omitted variable bias in the baseline specification (see Table A2 in Appendix). This
underscores the necessity of including these covariates for reliable causal inference.
We consolidate the original CPHS categories into broader groups to improve interpretability
while maintaining its theoretical relevance. Age group categories included in the model are
young-dominated households (combining households with majority children, and
Young-dominated), adult-dominated (households with working-age majority) and senior-present
(households with significant elderly presence). Education Groups included are high-education
(graduate-dominated, graduate-majority, graduate minority households), medium-education (All
matriculates, matriculate-dominated, matriculate majority, matriculate-minority households),
basic-education (Households of some literates, and literate households), and low-education
(illiterate households).

While our main difference-in-differences model estimates the average treatment effect, it masks
potential temporal heterogeneity in how households respond to increased income. To examine
the dynamic effects of the policy, we estimate:
Log(Health Expenditure)ᵢ􀀀 = β₀ + Σₖβₖ(Beneficiary × Quarter)ᵢₖ + β₄EduGroupᵢ􀀀 +
β₅AgeGroupᵢ􀀀 + δᵢ + γ􀀀 + εᵢ􀀀

where Quarter represents quarterly time periods after policy implementation, allowing us to
trace the evolution of the treatment effect over time. This model will help assess whether the
income shock had immediate effects or if households took time to adjust spending patterns and
reveal whether initial changes in health expenditure were sustained over time.
Our difference-in-differences strategy relies on several key assumptions. We argue that the Stable
Unit Treatment Value assumption is likely satisfied in this context because of the clear sectoral
separation that operates in the distinct labor markets with different regulatory environments for
the formal and informal sector, minimizing spillover effects. Since the policy specifically targets
formal sector wages, we assume that it does not affect informal sector workers. Upon visual
inspection of pre-treatment periods from 2016 to 2017 (See Figure 1), we can confirm parallel
movement in average health expenditure between the treatment and control groups supporting
the crucial parallel trends assumptions.

Figure 1: Parallel trends plot (beneficiary vs non-beneficiary health spending)
![Parallel trends plot beneficiary vs non-beneficiary health spending](https://github.com/user-attachments/assets/a22503e6-fa5d-4e61-a526-3327fd2a1732)

While both fixed and random effects specifications were considered, a Hausman test strongly
rejected the consistency of random effects estimators (p < 0.05). This supports our use of fixed
effects to control for unobserved household characteristics that might correlate with both formal
sector employment and health spending decisions. The two-way fixed effects approach also
accounts for time-invariant household characteristics and temporal shocks that could confound
our estimates.

# Results
As shown in Table 1, we see that 60% of the female households are employed in the informal
sector, with self-employed entrepreneurs (street vendors, shop owners, etc.) making up the
highest population, and formal sector workers primarily concentrated in wage labor.
The data also reveals important patterns in household health expenditure from 2016 to 2019.
Total monthly health expenditure shows a substantial increase over the study period, rising from
Rs. 26,306 in 2016 to Rs. 39,634 in 2019 - a 50% increase.

Table 1: Percentage of Female Workers by Employment and Occupation Group
![ Percentage of Female Workers by Employment and Occupation Group](https://github.com/user-attachments/assets/85e47f11-0838-46a4-85ea-90f6acfb5753)

Breaking down this expenditure by category, we see that health enhancement is consistently the
largest component of health spending accounting for approximately 40-43% of total health
expenditure, increasing from Rs. 11,273 in 2016 to Rs. 15,880 in 2019. In terms of medical
service expenditures, spending on doctors fees increased significantly from Rs. 1,121 in 2016 to
Rs. 2,911 in 2019. Spending on hospital fees fluctuated, peaking at Rs. 1,734 in 2018 before
declining, and medical tests doubled from Rs. 432 to Rs. 877 per month from 2016 to 2019.
Expenditure on health insurance premium, representing the smallest share of health expenditure,
shows modest but increasing adoption, rising from Rs. 371 to Rs. 469 per month in 2019. Figure
2 shows the breakdown of the monthly health expenditure components for female-headed
households over the years 2016 to 2019.

Figure 2: Breakdown of Components of Monthly Health Expenditure
![Breakdown of Components of Monthly Health Expenditure](https://github.com/user-attachments/assets/21451ec6-a8ee-49ce-a38b-e93c39f167c7)
Table 2 reports the estimates of equation 2 for the main dependent variable, Log of monthly total
health expenditure. The interaction term Beneficiary:Post_2018 is positive and statistically
significant at the 0.01 level, indicating that female households in the formal sector experienced a
1.9% higher growth in health expenditures post-2018 relative to female households in the
informal sector, after accounting for household age and education composition. This suggests
that the income shock from the 2018 policy had a measurable impact on the health spending
behavior of beneficiary households.
Among the age-related categories, female-headed households with seniors-present exhibit the
largest positive associations with health expenditures compared to the reference group,
households with adults, with an increase of 2.7% (p < 0.01) in monthly health expenditure
compared to adult households.

Table 2: Final Model
![Final Model](https://github.com/user-attachments/assets/ccf9f3b2-67d4-4296-9765-ea36049ae88a)


Notes: Coefficients shown are relative to the base category of Adult-dominated households, and
Basic-education, for age group and education group variables, respectively.
Young-dominated households see an associated increase of 2.3% (p < 0.01), compared to
adult-dominated households, closely following households with seniors present.

In terms of education, female-headed households with majority highly educated individuals
exhibit the highest health expenditures, with a substantial 23.9% higher spending compared to
the reference group, households with basic-education, significant at the 0.01 level. Similarly,
households with medium-education see an associated 13.9% (p < 0.01) increase in health
expenditure compared with households with basic education. On the other hand, households with
low education spend 8.8% (p < 0.01) less than the reference group.

Table 3 gives the estimates for equation 3 reporting the temporal trends in how the policy shock
affected health expenditure. Immediately following implementation, beneficiary households
showed a significant 3.9% increase in health spending, highly significant at the 0.01 level.This
initial effect remained relatively stable through Q2 2018 before showing a slight uptick to 1.3%
in Q3 2018, though this increase was not statistically significant. However, starting in Q1 2019,
we observe a significant decline in the treatment effect. Health expenditure decreased by 1.8% (p
< 0.05) in Q1 2019, with this downward trend continuing and strengthening through subsequent
quarters. By Q4 2019, beneficiary households were spending 3.3% less on health compared to
the initial impact (p < 0.01).

Table 3: Dynamic Treatment Effects Model
![Dynamic Treatment Effects Model](https://github.com/user-attachments/assets/55ce9c31-daec-4b5a-968b-9af9ef79006d)

In order to examine the individual effects of the components of total health expenditure in a
household, two way fixed effects models were run with the log of each component of total health
expenditure as the dependent variable (See Table 4). Examining the components of health
expenditure reveals heterogeneous effects of the income increase across different categories of
health spending.

The strongest effects are observed in preventive and health enhancement-related categories.
Health enhancement expenditure, which includes spending on wellness and preventive care,
shows the largest increase of 5.9%, significant at the 0.01 level, among beneficiary households.

Table 4: Change in Associated Health Expenditure Variables
![Change in Associated Health Expenditure Variables](https://github.com/user-attachments/assets/1242afc2-0499-4418-a2e6-6defa986e5a9)

Similarly, health insurance premium spending increased by 3.4%, also significant at the 0.01
level. In contrast, we find minimal effects on direct medical care expenses. Doctor fees show a
small, insignificant increase of 0.3%, while medical tests show an even smaller increase of 0.1%,
statistically insignificant as well. Hospital fees actually decreased marginally by 0.02%, though
this effect is also not statistically significant.

# Discussion
Following the 2018 policy that increased take-home pay for formal sector employees, our
findings suggest that female-headed households in formal employment increased their health
expenditure by 1.9% compared to similar households in informal employment. This differential
response to the policy-induced income change demonstrates that women's health spending
decisions are responsive to changes in available resources. This finding is similar to studies in
anti-poverty cash transfer literature that show that women as recipients of cash transfers improve
the health status of children, as well as larger increases in spending on health, and nutrition
(Duflo, 2003, Thomas, D. 1990 Gertler and Boyce, 2003).

Breaking down this effect by type of health spending reveals an important pattern: the increase
was primarily driven by preventive and long-term care choices (See Figure 3). Specifically, we
find a 5.9% increase in health enhancement spending and a 3.4% increase in health insurance
premiums, while spending on immediate medical needs like doctor visits and hospitalizations
showed minimal changes. This spending pattern coincides with India's broader push toward
preventive healthcare and insurance coverage during this period, including the launch of
Ayushman Bharat in 2018, a nation-wide government initiative which aimed to increase health
insurance coverage.

Figure 3: Bar Chart breakdown of Health Expenditure by Type
![Bar Chart breakdown of Health Expenditure by Type](https://github.com/user-attachments/assets/054b7a94-acef-4e13-b358-a5a12b49bc5d)

The stronger response in preventive care compared to curative care might reflect both
gender-specific healthcare seeking behaviors and socio-cultural constraints. While women often
face barriers in accessing hospital-based or curative care due to household pressures and social
norms in India (Agarwal et al., 2022b), they tend to be more proactive in preventive healthcare
decisions. Research by Hallyburton and Evarts (2014) shows that women are more likely than
men to seek health information and coordinate healthcare decisions for their families. This
pattern is particularly pronounced among educated women - our finding that high-education
households showed the largest increase in health expenditure aligns with Dluhos-Sebesto et al. ‘s
(2021) evidence that education plays a crucial role in health information seeking and disease
prevention.

The gender role of women as primary health care coordinators for their families might explain
these spending patterns. Studies have documented that women are more likely to consult diverse
healthcare resources, including formal and informal networks, and often search for health
information both for themselves and family members (Rowley et al., 2014; Warner and
Procaccino, 2007). This broader engagement with health information, combined with increased
resources from formal sector employment, might facilitate greater investment in preventive care
even when cultural barriers to hospital-based care persist.

Figure 4 reveals that household composition significantly influences health expenditure patterns
in female-headed households, with senior-present households spending 2.7% more on health
compared to adult-dominated households. This age-composition effect is particularly relevant in
India's demographic context, where population aging intersects with healthcare needs and
household financial decisions. Chowdhury et al. (2018) document that households with elderly
members face substantially higher healthcare burdens, particularly in managing chronic
conditions. This burden is especially pronounced given that over 60% of India's aged population
suffers from at least one non-communicable disease (Mini and Thankappan 2017).

Figure 4: Coefficient plots for education and age effects
![Coefficient plots for education effects](https://github.com/user-attachments/assets/73d311fc-ae34-4feb-ba15-52ecef3df54c)
![ Coefficient plots for age effects](https://github.com/user-attachments/assets/4d3f29e8-f6ae-4521-9354-21efa3ad5914)
Notes: Coefficients shown are relative to the base category of Adult-dominated households, and Basic-education.
The dots represent point estimates and horizontal lines show 95% confidence intervals. All estimates are from the
two-way fixed effects model controlling for household education levels.

The higher spending in senior-present households might reflect both health needs and resource
allocation decisions. Dhak (2014) as cited in Chowdhury et al. (2018) finds that Indian
households often prioritize elderly healthcare needs, even under financial constraints. This
prioritization becomes more feasible when households have access to formal sector income, as
suggested by our findings.

Finally, our temporal analysis shows that while the policy had an immediate positive effect on
health spending, the impact was not sustained long-term. Households appear to have initially
allocated their increased income to health expenditure but adjusted their spending patterns
downward over time. This could reflect either a reallocation of the additional income to other
priorities after meeting initial health needs, as evidenced by the women’s spending on other
expenditure including food, recreation and clothing (see Table A3 in Appendix) or possibly
suggest that the income shock led to a one-time increase in health investments rather than a
permanent change in health spending patterns. This pattern has important implications for
understanding how income shocks translate into sustained health investments, particularly in
developing country contexts where households face multiple resource constraints.

# Conclusion
This paper examines how increased income affects women's health expenditure patterns by
exploiting a 2018 policy change that increased take-home pay in India's formal sector. We find
that female-headed households in formal employment increased their health expenditure by 1.9%
compared to informal sector households, with this increase primarily driven by preventive care
and health insurance spending. The stronger response in preventive rather than curative care,
combined with the significant role of education in health spending decisions, suggests that both
resource constraints and information access influence women's health investment choices.
However, the declining effect over time raises questions about the sustainability of
income-driven health investments.

These findings have important policy implications. While income increases can prompt higher
health investments by women, the temporal pattern suggests that one-time income shocks might
not sustain long-term changes in health spending behavior. This points to the potential value of
combining income-based interventions with health education and sustained support for
preventive care access.

This paper has several limitations that warrant consideration. The CMIE data has been criticized
for underrepresenting women, young adults, and having a bias towards urban, middle-class,
educated households, potentially limiting the generalizability of our findings (Das et al., 2024).
Our short observational window, particularly post-policy, constrains our ability to assess
longer-term effects. Additionally, our treatment group includes all women in the formal sector
rather than just new entrants post-2018, potentially diluting the estimated treatment effect. The
lack of access to a detailed codebook also created challenges in precise variable interpretation.
Future research with longer time horizons and more representative data could help address these
limitations and further illuminate the relationship between women's income and health
investment decisions.

# Appendix
Table A1: Average Monthly Household Health Expenditure in Hundreds INR
![Average Monthly Household Health Expenditure in Hundreds INR](https://github.com/user-attachments/assets/97f3031d-1991-4a92-a263-3c875f7adbbe)
Table A1 presents the average monthly household health expenditure (in hundreds INR) from
2016 to 2019. Total health expenditure increased from Rs. 263.06 in 2016 to Rs. 396.34 in 2019.
Health enhancement consistently represents the largest component after total health expenditure,
increasing from Rs. 112.73 in 2016 to Rs. 158.80 in 2019. Other components show varying
patterns: doctor fees more than doubled from Rs. 11.21 to Rs. 29.11, while hospitalization fees
decreased from Rs. 15.64 to Rs. 7.29 over the study period.

Table A2: Model progression showing how adding covariates changed effects
![Model progression showing how adding covariates changed effects](https://github.com/user-attachments/assets/0a1cd257-7818-4ebc-b941-cf1ea7a00145)
Table A2 shows how the treatment effect evolves with the addition of different controls. The
baseline model without controls shows a decrease of 1.3% in health expenditure. Adding age
group controls changes the direction and magnitude of the effect to a 2.1% increase, suggesting
significant confounding by household age composition. The addition of education controls
stabilizes the effect at 1.9%, which remains robust. This progression demonstrates the
importance of controlling for household characteristics in isolating the policy's impact.

Table A3: Changes in other expenditure categories
![Changes in other expenditure categories](https://github.com/user-attachments/assets/fa24a388-ee96-4526-b3e9-ff0453e93af9)
Table A3 examines changes in non-health expenditure categories following the policy change.
All coefficients are statistically significant at the 0.01 level. Beneficiary households increased
spending on food, clothing and footwear, recreation, and transportation compared to
non-beneficiary households, while decreasing expenditure on bills and rent. These patterns
suggest the policy led to broader changes in household consumption patterns beyond health
spending.

# References
References
Agarwal, S., Chatterjee, S., & Chatterjee, C. (2022). Sweet cash: Is healthcare a normal good for
women in developing countries? SSRN Electronic Journal.
https://doi.org/10.2139/ssrn.4302532
Almås, I., Attanasio, O., & Carneiro, P. (2023). Household decisions and intra-household
distributions. In Elsevier eBooks (pp. 111–149).
https://doi.org/10.1016/bs.hefam.2023.01.008
Armand, A., Attanasio, O., Carneiro, P., & Lechene, V. (2020). The Effect of Gender-Targeted
Conditional Cash Transfers on Household Expenditures: Evidence from a Randomized
Experiment. The Economic Journal, 130(631), 1875–1897.
https://doi.org/10.1093/ej/ueaa056
Chowdhury, S., Gupta, I., Trivedi, M., & Prinja, S. (2018). Inequity & burden of out-of-pocket
health spending: District level evidences from India. The Indian Journal of Medical
Research, 148(2), 180. https://doi.org/10.4103/ijmr.ijmr_90_17
Das, S., Sane, R., & Shah, A. (2024). The usefulness of the CMIE household survey data for
electricity research in India.
https://blog.theleapjournal.org/2024/05/the-usefulness-of-cmie-household-survey.html#gs
c.tab=0
Dhak, B. (2014). Demographic change and catastrophic health expenditure in India. Social
Indicators Research, 122(3), 723–733. https://doi.org/10.1007/s11205-014-0717-4
Dluhos-Sebesto, C., Jethwa, T. E., Bertasi, T. G., Bertasi, R. A., Nishi, L. Y. M., Pantin, S. a. L.,
Argenio, S. L., Shahsamand, A., Omololu, A., & Pujalte, G. G. (2021). Women’s Health
Information Survey: Common health concerns and trusted sources of health information
among different populations of female patients. Women S Health Reports, 2(1), 173–181.
https://doi.org/10.1089/whr.2020.0118
Duflo, E. (2003). Grandmothers and Granddaughters: Old-Age pensions and intrahousehold
allocation in South Africa. The World Bank Economic Review, 17(>1), 1–25.
https://doi.org/10.1093/wber/lhg013
Gertler, P. J., & Boyce, S. (2003). An experiment in Incentive-Based Welfare: The impact of
PROGRESA on health in Mexico. Royal Economic Society Annual Conference 2003.
https://ideas.repec.org/p/ecj/ac2003/85.html
Gram, L., Skordis-Worrall, J., Saville, N., Manandhar, D. S., Sharma, N., & Morrison, J. (2018).
“There is no point giving cash to women who don’t spend it the way they are told to
spend it” – Exploring women’s agency over cash in a combined participatory women’s
groups and cash transfer programme to improve low birthweight in rural Nepal. Social
Science & Medicine, 221, 9–18. https://doi.org/10.1016/j.socscimed.2018.12.005
Hallyburton, A., & Evarts, L. A. (2014). Gender and online Health Information Seeking: A Five
Survey Meta-Analysis. Journal of Consumer Health on the Internet, 18(2), 128–142.
https://doi.org/10.1080/15398285.2014.902268
Macours, K., & Vakis, R. (2009). Changing households’ investments and aspirations through
social interactions : evidence from a randomized transfer program. In World Bank policy
research working paper. https://doi.org/10.1596/1813-9450-5137
Maxwell, M., & Vaishnav, M. (2021). Working Women’s Decision-Making Power at Home:
Evidence from Four North Indian Urban Clusters. Urbanisation, 6(1_suppl), S58–S76.
https://doi.org/10.1177/24557471211025891
Mini, G. K., & Thankappan, K. R. (2017). Pattern, correlates and implications of
non-communicable disease multimorbidity among older adults in selected Indian states: a
cross-sectional study. BMJ Open, 7(3), e013529.
https://doi.org/10.1136/bmjopen-2016-013529
Nanda, P. K. (2018, February 1). Union Budget 2018: Govt cuts women EPF contribution by 4%.
Hindustan Times.
https://www.hindustantimes.com/india-news/union-budget-2018-govt-to-amend-epf-act-t
o-reduce-pf-contribution-of-women-employees-to-8/story-Cg48lG6vkKEKE1MDt6DEp
N.html
Parinduri, R. A. (2016). Does Education Improve Health? Evidence from Indonesia. The Journal
of Development Studies, 53(9), 1358–1375.
https://doi.org/10.1080/00220388.2016.1228880
Rowley, J., Johnson, F., & Sbaffi, L. (2014). Students’ trust judgements in online health
information seeking. Health Informatics Journal, 21(4), 316–327.
https://doi.org/10.1177/1460458214546772
Thomas, D. (1990). Intra-Household resource allocation: an inferential approach. The Journal of
Human Resources, 25(4), 635. https://doi.org/10.2307/145670
Tnn. (2018, February 1). Budget 2018: Women take home more with PF tweak. The Times of
India.
https://timesofindia.indiatimes.com/business/india-business/budget-2018-women-take-ho
me-more-with-pf-tweak/articleshow/62748367.cms
Vikram, K., & Vanneman, R. (2019). Maternal education and the multidimensionality of child
health outcomes in India. Journal of Biosocial Science, 52(1), 57–77.
https://doi.org/10.1017/s0021932019000245
Warner, D., & Procaccino, J. D. (2007). Women seeking health information: Distinguishing the
web user. Journal of Health Communication, 12(8), 787–814.
https://doi.org/10.1080/10810730701672090
World Bank Group. (2018). Evaluations - conditional cash transfers. In World Bank.
https://www.worldbank.org/en/programs/sief-trust-fund/brief/evaluations-conditional-cas
h-transfers
