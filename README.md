
## Inspiration💡
The inspiration for this project stems from the persistent global challenge of extreme poverty, despite decades of international efforts to eradicate it. Traditional metrics like GDP have long been used to measure progress, but they fail to capture the lived realities of vulnerable populations. For instance, rising GDP figures often mask deep inequalities, where wealth accumulates at the top while millions remain trapped in poverty. This disconnect between economic growth and human well-being inspired us to explore alternative indicators, such as the Multidimensional Poverty Index (MPI), which provides a more nuanced understanding of poverty by considering factors like education, health, and living standards. Our goal was to uncover actionable insights that could guide policymakers and institutions toward sustainable solutions for alleviating extreme poverty.

## What it does 🎯
This project moves beyond GDP to analyze the drivers of extreme poverty using SAP’s dataset. By focusing on countries with MPI values exceeding 0.15, we identify key socioeconomic and institutional factors contributing to persistent extreme poverty. The analysis aims to:
 - Provide a deeper understanding of the root causes of extreme poverty.
 - Offer targeted policy recommendations for national governments and international organizations like the World Bank and IMF.
Ultimately, this project seeks to empower decision-makers with evidence-based strategies to address poverty effectively and equitably.

## How we built it🔧
Our project leveraged advanced machine learning techniques, including XGBoost , to create a robust index that models poverty effectively. The process began with extensive data cleaning and preprocessing to address significant challenges such as missing values, redundancy, and temporal inconsistencies. Using XGBoost, we trained models to identify key socioeconomic and institutional factors contributing to extreme poverty in countries with MPI values exceeding 0.15. TThe model's ability to handle complex, nonlinear relationships between variables made it ideal for analyzing the intricate interplay of factors such as education, healthcare access, political stability, and economic inequality. To ensure the reliability of our findings, we cross-validated the results against the HDI, demonstrating strong consistency between our index and this widely recognized benchmark.

## Challenges we ran into🤔
 - **Missing Data**: Over 50% of the features had incomplete data, complicating direct comparisons and requiring innovative imputation techniques.
 - **Redundancy**: Some indicators were highly correlated (>0.99 R²), necessitating careful feature selection to avoid multicollinearity.
 - **Threshold Interpretation**: Countries with an MPI value of 0 were automatically classified as “perfect,” even if their actual conditions varied widely (e.g., Singapore vs. Belarus). This required us to focus on countries above the 0.15 threshold for meaningful insights.
 - **Temporal Gaps**: Non-annual reporting for some indicators introduced inconsistencies, which we addressed through mean substitution and forward/backward filling.

## Accomplishments that we're proud of🚀
We are proud of successfully transforming a complex and incomplete dataset into a robust analytical framework that sheds light on the true drivers of extreme poverty. By addressing significant challenges such as missing data, redundancy, and temporal inconsistencies, we developed a streamlined methodology that allowed us to focus on countries with MPI values exceeding 0.15, ensuring our analysis was both meaningful and actionable. A key highlight of our work was the creation of an index that models poverty effectively, capturing the multidimensional nature of deprivation while maintaining strong cross-validation with established benchmarks like the Human Development Index (HDI). This alignment not only reinforces the reliability of our findings but also underscores the importance of moving beyond GDP to adopt more comprehensive measures of human well-being. Through this project, we have demonstrated the value of innovative data-driven approaches in tackling one of the world’s most pressing challenges.

## What we learned📖
Through this project, we gained valuable insights into the complexities of analyzing global poverty and the importance of adopting multidimensional approaches to measure human well-being. We learned that missing and inconsistent data are inevitable in large-scale datasets, requiring innovative solutions like mean substitution and forward/backward filling to ensure meaningful analysis. This process deepened our appreciation for the limitations of traditional metrics like GDP, which often fail to capture the nuanced realities of poverty. Collaborating as a team underscored the value of combining diverse expertise in data science, economics, and policy analysis to tackle multifaceted challenges. Ultimately, we learned that translating complex analytical insights into actionable recommendations is essential for driving real-world impact and fostering sustainable development.

## What's next🔜
Looking ahead, we plan to expand and refine this project in several ways:
 - **Expand Dataset Coverage**: Incorporate additional datasets from sources like the World Bank, UNDP, and regional organizations to enhance the breadth and depth of our analysis.
 - **Develop Predictive Models**: Use machine learning algorithms to predict future trends in MPI based on current socioeconomic indicators, enabling proactive policymaking.
 - **Engage Stakeholders**: Collaborate with governments, NGOs, and international institutions to pilot and evaluate the effectiveness of proposed interventions.
 - **Create a Public Dashboard**: Develop an interactive visualization tool to make our findings accessible to policymakers, researchers, and the general public.
