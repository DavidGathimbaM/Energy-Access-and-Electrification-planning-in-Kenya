# Energy Access and Electrification Planning in Kenya
![Electricity Grid](images/electricity-4666566_1280.jpg)
### Introduction

The **Rural Electrification Programme** in Kenya aimed to achieve universal electricity access across the country, resulting in **76%** of Kenyan households gaining electricity access. This initiative significantly boosted rural economic resilience in Kenya. However, since its conclusion in 2022, the country has seen a notable decline in electricity access, particularly in generation capacity and reliability.

![image](https://github.com/user-attachments/assets/953010f9-2466-4700-a767-07f338d702dc)

This project supports the World Bank's Mission 300, which aims to connect 300 million people in Sub-Saharan Africa to electricity by 2030. By leveraging data-driven insights, this project aims to guide energy planning and distribution in Kenya **to scale up connectivity** - a critical factor in addressing the country’s development needs.

### Problem Statement

Kenya’s population has been steadily increasing over the years. Notably, economic planning has not kept pace with this rapid growth.  As a result, an annual estimate of 4.4% rural-urban migration occurs, driven largely by youth seeking employment. However, this migration may not yield stable opportunities, as the Federation of Kenya Employers (FKE) reports a high youth unemployment rate of 67%.

To address the challenges posed by Kenya’s growing population, rising unemployment, and high rates of rural-to-urban migration, the government must implement strategic, long-term economic interventions. 

Prioritizing rural electrification and expanding energy access will stimulate local investments, promote the growth of small and medium-sized enterprises (SMEs), and enhance agricultural productivity through the adoption of advanced technologies. Most critically, fostering job creation within rural areas will drive sustained economic growth, increase household income, and build resilience within rural economies.


### Objective

This project utilizes geospatial data for Kenya to support strategic objectives in wind renewable energy planning.

**Classification and clustering algorithms** were applied to identify areas with sparse grid infrastructure and high population density, to highlight regions where wind farms and wind microgrids could be feasible solutions. 

**Findings:**

The machine learning analysis identified regions suitable for microgrids to be relatively densely populated, with an average of approximately 95.19 people per square kilometer. These areas also experience slightly stronger wind conditions, with an average speed of 6.14 m/s at 100 meters above ground level, making them well-suited for wind farms and microgrid installations.

Grid infrastructures in these regions were found to be significantly limited. Given the region's population density, there is clearly a higher demand for electricity but limited transmission capacity.

Approximately 50% of the population lives below the $2.15 poverty line, highlighting the high likelihood of rural-to-urban migration and the urgent need for economic empowerment.

### Business Understanding
This project addresses the pressing issue of low electricity access rates in Kenya, where approximately 25% of the population lacks reliable electricity.

The project's objective is to use data-driven analysis to identify optimal regions for decentralized electrification solutions, such as wind microgrids.

The topic is critical due to the social and economic impact of energy access on poverty reduction, economic development, and quality of life.

The primary audience includes government entities, NGOs, and private investors interested in sustainable electrification.

By providing a structured approach to identifying high-impact regions for renewable energy projects, the project can support better resource allocation, reduce infrastructure costs, and promote sustainable development.

This project builds upon previous research in energy demand prediction, renewable energy potential assessment, and the socio-economic impact of electrification.

### Data Understanding
The following data was used to achieve the project objectives:

Latitudes & Longitudes: These are Kenya’s spatial identifiers sourced from the Global Wind Atlas'.

Population Density: This is the estimated number of people living within a 1 km² area, covering data from the year 2000 to 2020. Source: WorldPop Hub.

Grid Infrastructure: Includes data on grid infrastructure, such as transmission lines and substations, sourced from the World Bank’s Global Electrification Platform (GEP).

Wind Renewable Energy Potential: This identifies regions with high potential for wind renewable energy, based on wind speed measurements at 100 m/s above ground level and sea level. Source: Global Wind Atlas.

Income Distribution: This is the proportion of the Kenyan population living in households with consumption or income per person below the $2.15 poverty line. Source: World Bank’s Global Subnational Poverty Atlas (GSAP).

These datasets collectively enable the assessment and mapping of regions with low electrification rates, high electricity demand, and renewable energy potential.

**1. Data Extraction & Visualization: Kenya's Electricity Generation & Demand**
![image](https://github.com/user-attachments/assets/868f9990-2897-4582-a46d-994cbdeeca32)

**2. Data Extraction and Visualization: Renewable Potential**
![image](https://github.com/user-attachments/assets/65687bda-52c1-4401-afad-493b503a8867)

![image](https://github.com/user-attachments/assets/4222fe30-5520-4e09-8b18-72c3479c25c3)

The map provides a clear visual aid for identifying regions where wind  energy can address gaps in electricity access.
![image](https://github.com/user-attachments/assets/d64e2c80-7350-4e70-ad47-1ded781202cb)

**3. Data Extraction & Visualization: Kenya's Population Density**
![image](https://github.com/user-attachments/assets/4b3cd2c0-0779-49b6-b16b-4ee36cdd3c9c)
![image](https://github.com/user-attachments/assets/59a33379-3a05-4e20-8ed9-6d5291bb900b)

![image](https://github.com/user-attachments/assets/efc414c2-e6f1-499c-a8bc-c41042d0e47d)
![image](https://github.com/user-attachments/assets/fd37e226-4766-4cd2-95a3-500357e7a245)


**4. Data Extraction & Visualization: Kenya's Income Level**
![image](https://github.com/user-attachments/assets/a7c1a68d-780d-4b66-aec5-1fb5d4d63da5)

% of population living in households with consumption or income per person below the $2.15 poverty line.
![image](https://github.com/user-attachments/assets/4b3e107b-14db-46e6-a44e-014dc9fcc6d9)

**5. Data Extraction & Visualization: Grid Infrustructure**
![image](https://github.com/user-attachments/assets/5d0c83f7-3051-4f7e-90bc-376b1d636f53)

![image](https://github.com/user-attachments/assets/2887e454-701f-4b34-9f15-a49d363b5c53)
![image](https://github.com/user-attachments/assets/60e5ebd1-d1da-4f88-ab10-8e5844c408a8)


**6. Datasets Merging**
![image](https://github.com/user-attachments/assets/405ac42a-0af9-40a8-9d00-c617394a19b3)
![image](https://github.com/user-attachments/assets/40be7d09-b0a8-4476-b1c0-a291019a7aa6)


### Machine Learning
**(a). Clustering Algorithms**
Objective 1:
Identify regions with sparse grid infrastructure and high population density where wind farms and microgrids could be feasible. This will be determined by analyzing population density projections, income distribution, and wind speed.
**1. K-Means Clustering**
![image](https://github.com/user-attachments/assets/9eb313a9-3d17-4953-b462-bf071b2cca76)
![image](https://github.com/user-attachments/assets/1d10de48-1877-4660-bf97-53e2b80f082b)
From the above visualization, using 2 clusters is the optimal choice for segmenting regions based on grid infrastructure sparsity and wind microgrid feasibility.

![image](https://github.com/user-attachments/assets/149ee52c-fdd3-4a62-aa09-14249fe705b2)

**Explore cluster characteristics**
*Findings;*
**1. Cluster 0**
The areas in cluster 0 are **relatively densely populated** with approximately 95.19 people per square kilometers.

The wind conditions in this cluster are slightly stronger than in Cluster 1, with an average speed of 6.14 m/s at 100 meters above ground level. Therefore, these regions are suitable for both **wind farms and wind microgrids**.

The grid infrastructure in Cluster 0 is significantly limited, with a value of 0.000096. Given the region's population density, there is clearly **high demand for electricity but limited transmission capacity**.

The average income distribution of Cluster 0 is 41.999, indicating that approximately **50% of the population lives below the $2.15 poverty line**. Therefore, this cluster has a higher proportion of people living in poverty.

**2. Cluster 1**
Compared to Cluster 0, the regions in Cluster 1 have a **slightly lower population density** of 94.17 people per square kilometer.

Wind conditions in Cluster 1 are **generally calmer**, with an average wind speed of 5.80 m/s at 100 meters above ground level.

Cluster 1 has a **higher presence of grid structures**, with a grid value of 0.5524, indicating that these regions are likely more developed compared to those in Cluster 0 and have higher access to electricity/energy.

The average income distribution in Cluster 1 is 21.06, indicating that **only 21.06% of the population in these regions lives below the $2.15 poverty line**.

**Evaluation**
-A **Davies-Bouldin Index of 0.73315** indicates that the clusters are relatively compact and distinct.
-A **Calinski-Harabasz Score of 995263.1557610929** data points in each cluster are tightly grouped together, and the clusters themselves are well-separated.

Conclusively, this model has successfully created meaningful clusters with a significant difference between them.
### Recommendations

The **government of Kenya** in collaboration with the **private sector** should adopt this deployment model as a strategic guide for the placement of wind farms and microgrids. This approach will enhance energy and electricity access, promote sustainable development, and strengthen the economic resilience of rural communities.
