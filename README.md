# Data-Warehouse-Proj-1

Special Requirements for CITS5504 and CITS3401

    For CITS3401 Students: You must use both the Fatal Crashes - December 2024 dataset and the Fatalities - December 2024 dataset for your project.

    For CITS5504 Students: You must use the Fatal Crashes - December 2024 dataset and the Fatalities - December 2024 dataset. Additionally, 

        you are required to utilise at least one of the following datasets: Dwelling Count Data or Population Data. You may choose to incorporate both of these additional datasets if desired.

    OR

        you may choose to merge your own additional data sources with the Fatal Crashes - December 2024 and Fatalities - December 2024.

    For both CITS5504 and CITS3401 students, you are encouraged to identify at least 8 dimensions in your project.

Data Warehousing Design and Implementation

Design a data warehouse for the dataset(s) by following the four steps below of dimensional modelling (i.e., Kimball's four steps).

    Identify the process being modelled.

    Determine the grain at which facts can be stored.

    Choose the dimensions

    Identify the numeric measures for the facts.

To realise the four steps, we can start by drawing and refining a StarNet with the above four questions in mind.

    Think about a few business questions that your data warehouse could help answer.

    Draw a StarNet to identify the dimensions and concept hierarchies for each dimension. This should be based on the lowest level of information you have access to.

    Use the StarNet footprints to illustrate how the business queries can be answered with your design. Refine the StarNet if the desired queries cannot be answered, for example, by adding more dimensions or concept hierarchies.

    Once the StarNet diagram is completed, draw it using software such as Microsoft Visio (free to download under Azure Education) or a drawing program/website of your own choice. A Hand-printed StarNet diagram is also welcome!

    Implement a star or snowflake schema using PostgreSQL. For the fact table and dimension tables, clearly state which ones are measures and dimensions, and indicate the dimension references.

    Use PostgreSQL to build a multi-dimensional analysis service solution, with a cube designed to answer your business queries. Make sure the concept hierarchies match your StarNet design.

    Use Power BI/Tableau to visualise the data returned from your business queries.

Association Rule Mining

NOTE: you are not allowed to use Microsoft Visual Studio, R, or Weka to do association rule mining in this project. Only Python code will be considered (for association rule mining) in this project.

Make sure you complete the relevant lab before attempting this task. The lab content may help you complete this task. 

You are expected to select a subset (or all) of the attributes to mine interesting patterns. To rank the interestingness of the extracted rules, use support, confidence, and lift.

In the submitted PDF, you need to:

    Explain and discuss which association rules mining algorithms were used with references.

    Explain the top k rules (where k ≥ 1) that have "Road User" on the right-hand side, ranked by lift and confidence.

    Explain the meaning of these k rules in plain English.

    Share insights derived from the mining results. If no meaningful rules are discovered, explore potential reasons for this outcome.

    Based on the rules, provide and explain at least THREE (3) recommendations to the government on how to improve road safety for road users.

What to Submit

The following are the files needed for Project 1 submission.

NOTE: 

    In-text citations and end-text references are required in this project report, following the IEEE referencing style.

    Include team members' information in the report, such as team members' names and student IDs.

    A comprehensive PDF report that includes the following key components:

        Design, implementation, and usage of the data warehouse:  Explain and discuss the design, implementation, and usage of the data warehouse to answer your queries, such as the fact table, dimension tables, and concept hierarchies design. When designing your data warehouse, you may select any number of columns/attributes as dimensions and measures. Please justify your design by explaining your assumptions or reasoning behind your choices with references.

    NOTE: The data warehouse design should demonstrate concept hierarchies and good dimension modelling. An overly simple design will result in low marks for the project.

        Schema, Starnet and query footprints: Provide and explain your StarNet diagrams and the query footprints. Discuss which schema you used and justify your choice with references.

        Data cleaning, preprocessing, and ETL process: Describe your ETL process in detail. Include descriptions of the techniques used, discuss your ETL principles, explain the reasoning behind the key steps, and provide screenshots illustrating the process flow with references. 

    NOTE: During the ETL process, you may remove some rows from the dataset. However, the number of dropped rows should not exceed 5% of the total dataset. Removing too many rows will result in a low mark for the ETL section. 

        Visualisation of query results: Present the findings from your business queries using appropriate charts, graphs, and other visualisations. Ensure the insights are clearly communicated and easily understandable to stakeholders.

        Association rules mining: See the Association Rules Mining section above. 

    All scripts you used (e.g. Python, PostgreSQL) with clear and well-structured comments.

    The Power BI/Tableau file (.pdf file).

    All CSV files you used for building and populating your database.

NOTE: All files need to be zipped up in a single zip file and submitted to LMS (Under the Projects channel that can be found in the left navigation panel).
Marking Scheme
Scheme
Marks

Schema of each dimension and concept hierarchies for each dimension

5

Corresponding StarNet to illustrate query capabilities of the data warehouse

5

At least 5 types of business queries that the StarNet can answer

5

Data warehouse schema and fact table design

5

Data cleaning/pre-processing/ETL process for data transformation (include code, screenshots, and detailed explanations)

10

SQL Script file for building the database and loading the datasets

5

Visualise corresponding to the 5 business queries with appropriate charts

5

Association rule mining meaningful set-up

5

Interpretation of top rules and suggestions

5

Coherence between the design and implementation, quality and complexity of the solution, reproducibility of the solution

5

Overall report quality

5

Total

60