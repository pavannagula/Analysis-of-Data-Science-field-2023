# Analysis on "Is Data Science a Dying Field in 2023" by scrapping the LinkedIn job postings

## Introduction

This project aims to analyze the job market in the data science field to gain valuable insights into its growth, demand, and key trends. By leveraging web scraping techniques to collect job postings from LinkedIn and performing extensive exploratory data analysis (EDA), I have delved into various aspects of the data science job market. My analysis covers job titles, industries, required skills, salaries, educational requirements, and more, all with the goal of understanding the evolving landscape of the data science industry in 2023.

Highlights of our project:

- Data Collection: I've scrapped a comprehensive dataset of 2500 AI family job postings from LinkedIn, ensuring a diverse range of data science positions and capturing a snapshot of the current job market.

- Exploratory Data Analysis (EDA): Through detailed EDA, I explored the distribution of job titles, industries, and the skills and educational qualifications sought by employers. I utilized visualizations to uncover insights into the growth, demand, and key trends within the data science field.

- Insights and Findings: Analysis revealed compelling insights. For instance, the job market witnessed a surge in data science job postings during specific months, indicating a growing demand for data professionals. I've identified the most sought-after skills in the industry, such as Python, Data Analytics, and Cloud Skills. Additionally, I have also discovered that IT Services and Consulting industries were at the forefront of data science job postings, reflecting the increasing adoption of data-driven approaches across sectors.

- Salary Analysis: Examined salary distributions within the data science field, revealing a concentration of salaries between $100,000 and $200,000. This highlights the industry's recognition of the value and expertise that data scientists bring, resulting in competitive compensation packages.

By combining web scraping, EDA techniques, and visualization tools, this project provides unique insights into the data science job market, showcasing its growth, demand, and emerging trends. These findings empower job seekers, professionals, and organizations with valuable knowledge to make informed decisions and navigate the evolving landscape of the data science industry.

## Project Structure
- `data_collection`: web scraping job postings from LinkedIn using the Octoparse parsing tool.
- `Data_Cleaning_Linkedin_Jobs.ipynb`: Covers data cleaning, preprocessing, and feature engineering steps.
- `JD_Skills_Extraction.ipynb`: Implemented Natural Language processing methods like spaCy for extracting skills and educational requirements from the job description.
- `EDA_Linkedin.ipynb`: Conducts in-depth exploratory analysis and generates visualizations.
- `README.md`: Front page of the repository, providing an overview of the project.

## Data Collection and Preprocessing
I have collected job postings from LinkedIn using a web scraping tool, focusing on the AI family of job roles. The data cleaning process involved handling missing values, standardizing data formats, and extracting relevant features such as job titles, company information, seniority levels, and employment types.

## Feature Extraction using NLP
Leveraged the power of natural language processing (NLP) and the spaCy library to extract valuable skills and education information from the job descriptions. This allowed me to gain deeper insights into the specific requirements and qualifications sought by employers in the data science field.

### Skills Extraction
Using spaCy's linguistic features, I performed named entity recognition (NER) to identify and extract relevant skills mentioned in the job descriptions. By analyzing the syntactic structure and context, I identified keywords related to programming languages (e.g., Python, SQL), machine learning techniques (e.g., deep learning, ensemble methods), data visualization tools (e.g., Tableau, Power BI), and cloud platforms (e.g., Azure, AWS). These skills were then used to create binary features indicating the presence or absence of each skill in the job postings.

### Education Information Extraction
To understand the educational requirements, I employed spaCy's part-of-speech tagging and dependency parsing capabilities. By examining the grammatical patterns and relationships within the sentences, I identified educational keywords such as "bachelor's degree," "master's degree," and "Ph.D." Furthermore, I extracted specific disciplines like computer science, statistics, mathematics, or related fields, providing insights into the preferred educational backgrounds for data science roles. Similar to skills extraction, binary features were created to indicate the presence or absence of each education level or discipline in the job postings.

## Exploratory Data Analysis
Through extensive exploratory analysis, I uncovered intriguing insights about the data science job market:
### Distribution of job titles:
- I've visualized the distribution of job titles using bar plots, providing a clear picture of the most prevalent roles in the data science field. The plots revealed that "Data Scientist," "Machine Learning Engineer," and "Software Engineer- AI/ML/DS" were the most common job titles, indicating the high demand for professionals with these skill sets.
 
 ![image](https://github.com/pavannagula/Analysis-on-Is-Data-Science-a-Dying-field-in-2023-by-scrapping-Linkedin-Data-Science-related-jobs/assets/39379433/dad3bc3b-fefb-4156-a285-0566c4b58ec2)


### Geographic insights:
- To gain a regional perspective, I've created choropleth maps to showcase the distribution of job postings across different states. The visualizations highlighted states like "California", "Texas", and "New York" are the highest job demands, key hubs, and hotspots for data science opportunities.
  
![state_wide_job_postings](https://github.com/pavannagula/Analysis-on-Is-Data-Science-a-Dying-field-in-2023-by-scrapping-Linkedin-Data-Science-related-jobs/assets/39379433/83062312-52fe-4ec7-906c-9193a176d96d)

### Number of Job Postings Over Time: 
- I've analyzed the temporal distribution of job postings to understand the dynamics of the data science job market. By plotting the number of job postings over time, I've observed that the majority of job postings occurred during the months of June and July in 2023. This spike in job postings indicates a growing demand for data science professionals and reflects the industry's increasing recognition of the importance of data-driven insights.
  
![Job_Postings_over_Time](https://github.com/pavannagula/Analysis-on-Is-Data-Science-a-Dying-field-in-2023-by-scrapping-Linkedin-Data-Science-related-jobs/assets/39379433/d7b84dac-95ac-43c1-ad8e-6c760ec59062)

Insights: This trend suggests a positive outlook for individuals pursuing a career in data science. The increased number of job postings during this period indicates a favourable job market, with ample opportunities for those with the required skills and qualifications. It also highlights the growing need for data science expertise across various industries.

### Top Skills Mentioned in Job Descriptions
- To identify the most sought-after skills in the data science job market, I've analyzed the job descriptions using natural language processing techniques. By extracting and counting the frequency of skill mentions, I've identified the top skills mentioned in the job descriptions.
  
![Top_skills](https://github.com/pavannagula/Analysis-on-Is-Data-Science-a-Dying-field-in-2023-by-scrapping-Linkedin-Data-Science-related-jobs/assets/39379433/d06ffb35-78e7-4f84-ac26-428d35548e67)

Insights: The analysis revealed that the most frequently mentioned skills in data science job descriptions are Python, Data Analytics, and Cloud Skills. This underscores the significance of these skills in the industry and suggests that employers highly value candidates proficient in these areas. Job seekers looking to stand out in the competitive data science market should focus on developing these skills and showcasing them in their resumes and applications.

## Industry Analysis

By analyzing the distribution of industries in the data science job market, I've gained valuable insights into the sectors actively recruiting data science professionals. My analysis revealed that the IT Services and Consulting industries were at the forefront, with the highest number of job postings. These industries recognize the importance of leveraging data-driven approaches and are actively seeking talent to drive their data science initiatives.

![image](https://github.com/pavannagula/Analysis-on-Is-Data-Science-a-Dying-field-in-2023-by-scrapping-Linkedin-Data-Science-related-jobs/assets/39379433/322317b0-9d18-4b0b-bd1f-b6327dc81dfa)

![image](https://github.com/pavannagula/Analysis-on-Is-Data-Science-a-Dying-field-in-2023-by-scrapping-Linkedin-Data-Science-related-jobs/assets/39379433/ad0f1e42-2256-42f9-85e1-c2e796b945ea)

Insights: The IT Services and Consulting industries emerged as the dominant players in the data science job market. This highlights the growing demand for data science expertise in these sectors and presents exciting opportunities for professionals looking to make an impact in these dynamic industries. By focusing on these sectors, job seekers can align their skills and interests with the industries at the forefront of data-driven innovation.

## Salary Analysis

Through the analysis of the salary distribution in the data science job market, I've gained valuable insights into the earning potential in this field. Our findings indicate that the majority of data science job salaries are distributed between the $100,000 to $200,000 range.

![image](https://github.com/pavannagula/Analysis-on-Is-Data-Science-a-Dying-field-in-2023-by-scrapping-Linkedin-Data-Science-related-jobs/assets/39379433/a9945cbf-4834-45d9-9be7-197370a22d4a)

Insights: The salary distribution graphs and Violin plots showcased a concentration of salaries within this range, indicating that it is a common salary bracket for data science professionals. This range reflects the industry's recognition of the high-demand skills and expertise required for data-driven decision-making. Job seekers in the data science field can expect competitive compensation packages within this salary range.


## Conclusion and Insights
Based on the comprehensive analysis conducted on the data science job market, I can confidently conclude that the field of data science is still evolving and experiencing significant growth. My findings, derived from extensive data scraping, exploratory data analysis, and visualization, provide compelling evidence supporting this conclusion.

Here are the key points that support my conclusion:

1. **Increasing Job Postings**: The temporal analysis of job postings revealed a substantial increase in the number of data science job openings over time. The spike in job postings during specific months, such as June 2023 and July 2023, indicates a growing demand for data science professionals.

2. **Skills in High Demand**: The analysis of job descriptions using natural language processing techniques highlighted the most sought-after skills in the data science job market. Skills such as Python, Data Analytics, Cloud Skills, and Machine Learning emerged as the most frequently mentioned skills, indicating their high demand and critical role in the industry.

3. **Growing Industries**: The industry analysis revealed that the IT Services and Consulting industries were leading in terms of the number of job postings. This indicates the increasing adoption of data-driven approaches and the demand for data science expertise across sectors.

4. **Competitive Salaries**: The analysis of salary distribution indicated that the majority of data science job salaries fell within the $100,000 - $200,000 range. This range reflects the industry's recognition of the value and expertise that data scientists bring to organizations, resulting in competitive compensation packages.

Collectively, these insights paint a compelling picture of the evolving nature of the data science field. The increasing job postings, high demand for specific skills, growing industries, and competitive salaries all indicate a vibrant and dynamic data science job market. By presenting these findings, I can confidently conclude that the data science field is still evolving and experiencing significant growth. Job seekers and professionals in the field can leverage these insights to make informed decisions and navigate the evolving landscape of data science career opportunities.

I hope this conclusion effectively captures the essence of my findings and supports the main aim of showcasing the continuous evolution of the data science field!

## How to Use and Replicate
To replicate this project, follow these steps:
1. Clone the repository to your local machine.
2. Install the required libraries and dependencies listed in the `requirements.txt` file.
3. Run the Jupyter notebooks in the specified order: `data_collection`, `Data_Cleaning_Linkedin_Jobs.ipynb`, `JD_Skills_Extraction.ipynb`, and `EDA_Linkedin.ipynb`.
