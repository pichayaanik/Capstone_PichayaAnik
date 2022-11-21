# Leveraging Topic Modeling to Extract News Articles for Analysis on Thailand's Digital Competitiveness Ranking
---
#### Pichaya (Anik) Charoonpongsakdi
Data Science Immersive - Capstone Project<br>
Link to the presentation [>>Click here<<](https://docs.google.com/presentation/d/1TooN8ycOvl-FB0gWikqjoO2LvPg2Vlh-09dW1wUhXB8/edit?usp=sharing)

### Summary
This project explores four topic modeling algorithms, namely
(1) K-Mean clustering,
(2) Latent Dirichlet Allocation - LDA
(3) Non-negative Matrix Vectorization - NMF
(4) Top2Vec
as tools for distant reading to extract news articles from BangkokBiz and Matichon corpuses that show the most relevance to 20 soft data based Digital Competitiveness Ranking Indicators.  The results suggest that Top2Vec model performs the best and yields useful topics and articles that can be further used in close reading, policy analysis and ranking development.

### Problem Statement
Digital Council of Thailand (DCT) aims at boosting IMD World Digital Competitivness Ranking, a widely trusted index trusted by governments and private sectors globally and used as an international benchmark for measuring digital readiness. As of 2022, Denmark ranked the 1st from 64 countries, followed by USA and Sweden. For Southeast Asia, Singapore performs the best at the 4th, Malaysia at the 31st. Thailand fares at the 40th, which is in the lower half of the rank, followed by Indonesia at the 51st.

The ranking consists of 54 indicators. 34 out of 54 are hard data based indicators, meaning that these indicators were assessed from numerical features e.g. Pupil-teacher ratio, number of internet users, ranking from other sub-rankings e.g. inclusive internet ranking. On the other hand, the other 20 indicators are evaluated and interpreted from soft data, meaning that the data are collected from surveys and expert interviews by IMD or its local affiliates/representatives and thus are not available for public.

Digital Council of Thailand (DCT) aims at improving the ranking to the **25th by 2525.** To achieve this goal, policy analysts rely to large extent on indicators analysis to make recommendation for improvement. However, examining and analyzing the soft data based indicators are not easy, considering that the primary data are not made available to public. Hence, the process of intensiveresearching, close reading and studying texts from public sources are the crucial part of the process. Nevertheless, the large amount of the incoming text data make it close to impossible for analysts to conduct a comprehensive investigation on the said indicators.

### Project Objective
- To flter & extract news articles related to
Digital Competitiveness Ranking indicators that are based on soft data
for further analysis and close readings

### Datasets
1. **BangkokBiz**

|Topic| Sub-Topic| Description|
|---|---|---|
|size|articles| 361,228|
||metadata|7|
|time||2014-2022|
|categories|top 5 categories|1. Politics
|||2. Finance and Investment|
|||3. Foreign Affairs|
|||4. Economics|
|||5. Lifestyle|

2. **Matichon Corpus**

|Topic| Sub-Topic| Description|
|---|---|---|
|size|articles|432,901|
||metadata|6|
|time||2015-2021|
|category|top 5 categories| 1. Politics|
|||2. News-monitor|
|||3. Region|
|||4. Crime|
|||5. Foreign|



### Conclusion
Among 4 topic modeling algorithms, Top2Vec yields the best result on revealing topic clusters that are related to IMD World Digital Competitiveness Index. It can filter and extract news articles that can be further used in close readings and policy analysis. The indicators and topics pairs that were derived from the BangkokBiz and Matichon corpuses are as follows:

|Domain|IMD Indicator| Top2Vec Topic |
|---|---|---|
|Knowledge| > Foreign highly-skilled personnel| Education |
|  |> Digital/Technological skills | Digital skills|
| |> Employee Training|
| |> Knowledge Transfer|
| Law&Regulation| > Immigration Law| Digital skills|
|| > Scientific research legislation|Smart city
|| > Intellectual property rights| Law and Crime|
|| > Cyber security|  AI|
|| > Development and Application of Technology|EEC
|Investment| > Venture capital| Venture capital|
||> Funding of technological development|
||>Public-private partnerships
|Infrastructure|> Management of cities|Smart city|
||> Banking and financial services|Banking
||> Communication technology|Telecommunications
|Digital Economy|> Agility of companies|Venture capital
||> Opportunities and threats|AI
||> Use of big data and analytics|EEC
||> Internet experience
