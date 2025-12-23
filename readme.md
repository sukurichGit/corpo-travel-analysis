<p align="right">
  EN | <a href="README_PL.md">PL</a>
</p>

# 📊 Marketing Analytics of Corporate Travel Data ✈️
### A project analyzing a database containing data from a company that organizes corporate travel. The analysis was conducted with the aim of improving the company's marketing strategy and increasing profits.

***

### For a complete, step-by-step walkthrough of the analysis, including all SQL queries, visualizations, and detailed recommendations, please see the [Full Jupyter Notebook Report](analysis.ipynb).


## 📝 About The Project
### The goal of the project is to simulate the role of a Marketing Analyst/Data Analyst, analyze available data on the company's partners and customers, identify gaps in the marketing strategy, and eliminate those gaps by proposing appropriate solutions. Data Source - **[Kaggle](https://www.kaggle.com/datasets/leomauro/argodatathon2019/data)**

## 🛠️ Tech Stack
*   **Data Analysis & Querying:** SQL (SQLite), Python (Pandas)
*   **Data Visualization:** Matplotlib, Power BI (in progress)
*   **Development Environment:** Jupyter Notebook, VS Code
*   **Version Control:** Git & GitHub

<p align="left">
  <img src="https://img.shields.io/badge/SQL-0769AD?style=for-the-badge&logo=sqlite&logoColor=white" alt="SQLite">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter">
  <img src="https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=matplotlib&logoColor=white" alt="Matplotlib">
  <img src="https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI">
</p>

***
## 🚀 Project Deliverables

*   **Interactive Dashboard:** For a dynamic overview of the key metrics, you can explore the **[Power BI Dashboard](dashboard.pbix)**.
![Dashboard](images/dashboard.png)

*   **PDF Dashboard:** For a overview of the key metrics, you can see the **[Power BI Dashboard in PDF](dashboard.pdf)**.


*   **Detailed Analysis:** For a complete, step-by-step walkthrough of the analysis, please see the **[Full Jupyter Notebook Report](analysis.ipynb)**.

## ❓ Key Business Questions
*   **Which clients are our most valuable partners, and how does their spending structure (flights vs. hotels) differ?**
*   **What are the key travel patterns and preferences?**
*   **Is demographic data (age, gender) a significant factor in our clients' travel behavior, or should we focus on other segmentation criteria?**
*   **How effective are our sales channels – agencies?**

## 📊 Key Insights & Visualizations

### Insight 1: Significant risk of sales concentration,  dependency on a single client

![Insight 1](images/insight_1.png)

 "4You" is our largest client, with spending that doubles the next competitor, driven purely by a higher volume of trips.This creates a significant concentration risk. Our primary goal must be long-term retention.

***

### Insight 2: There are key travel corridors for each company that can be used in building a marketing strategy.

 The analysis revealed that each of our key clients has a dominant business travel corridor — a pair of cities with a high and consistent volume of trips in both directions. The key corridors are:
<ul>
<li><b>4You: Aracaju (SE) ↔ Recife (PE)</b></li>
<li><b>Monsters CYA: Campo Grande (MS) ↔ Sao Paulo (SP)</b></li>
<li><b>Acme Factory: Campo Grande (MS) ↔ Florianopolis (SC)</b></li>
<li><b>Umbrella LTDA: Aracaju (SE) ↔ Florianopolis (SC)</b></li>
<li><b>Wonka Company: Aracaju (SE) ↔ Natal (RN)</b></li>
</ul>
This pattern indicates that these routes are tied to our clients' critical and recurring business operations (e.g., connecting a head office with a major branch). This high predictability and volume give us significant leverage and an opportunity to create a high-margin, value-added service instead of just selling individual tickets.

***

### Insight 3: Some companies have a significantly longer average flight distance.

![Insight 3](images/insight_3.png)

Most likely, these companies either have a wider geographical reach or a greater international business impact. So we need to find solutions to increase the comfort and productivity of passengers (e.g., fast track for economy class, access to business lounges, more prestigious hotel transfers, etc.) who fly farther and longer, and offer them a corresponding package of such services, which will increase our company's revenue through margins on these services

***

### Insight 4: Client base is homogenous from a demographic perspective.

| company       | users_count | average_age | female_count | male_count | nodata_count |
|---------------|-------------|-------------|--------------|------------|--------------|
| 4You          | 453         | 42.7        | 151          | 138        | 164          |
| Acme Factory  | 261         | 42.1        | 85           | 93         | 83           |
| Wonka Company | 237         | 43.1        | 79           | 90         | 68           |
| Monsters CYA  | 195         | 43.8        | 64           | 61         | 70           |
| Umbrella LTDA | 194         | 42.2        | 69           | 70         | 55           |

![Insight 4](images/insight_4.png)

This indicates that our client base is homogenous from a demographic perspective. It implies that factors like a person's company and its travel policies are much stronger predictors of their travel behavior (like choice of class or destination) than their age or gender.

***

### Insight 5: Huge missing opportunity - we are not using agency "FlyingDrops" enough

![Insight 5](images/insight_5.png)

| agency      | economic_flights | first_class_flights | premium_flights |
|-------------|------------------|---------------------|-----------------|
| CloudFy     | 38656            | 38862               | 38860           |
| FlyingDrops | 0                | 38758               | 0               |
| Rainbow     | 38810            | 38798               | 39144           |


FlyingDrops is our exclusive channel for selling our highest-margin product—First Class. The fact that this channel accounts for only 10-15% of bookings, even among our premium customers, is a <b>huge missed opportunity</b>.


---




