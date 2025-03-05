# Dataiku-Data-Engineering-Project-CO2-Emissions-Analysis
![image](https://github.com/user-attachments/assets/25ee4823-f7f3-4f5f-a198-834581c4855d)
![image](https://github.com/user-attachments/assets/45d1efe9-6a4d-4e2c-b175-38af7b2512b5)


Datasets Used

The analysis is based on three datasets from Our World in Data:

CO2_and_Oil.csv – CO₂ emissions per capita and oil production in terawatt-hours.

Urbanization_GDP_and_Population.csv – Urbanization percentage, GDP per capita, and population.

Meat_and_Egg_Production.csv – Meat and egg production in tonnes, and meat supply per capita.

Steps Followed

# 1. Data Import

Uploaded the three datasets into Dataiku DSS.

Checked schema and inferred storage types.

# 2. Data Merging

Used CO2_and_Oil.csv as the base dataset.

Merged Urbanization_GDP_and_Population.csv and Meat_and_Egg_Production.csv using Entity, Code, and Year.

Filtered the dataset to include only data from 2008 to 2012.

Ensured the final dataset had 985 rows and 11 columns.

# 3. Data Cleaning and Transformation

Converted Oil Production, Meat Production, and Egg Production into per capita values by dividing by the population.

Removed original total columns and the population column.

Filtered out global data (Entity == "World").

Replaced missing values in per capita columns with 0.

# 4. Data Aggregation

Aggregated the dataset to compute the average values for each country over the period 2008-2012.

The resulting dataset contained 196 rows (one per country).

# 5. Data Ranking

Created a ranking of the top 25 countries by CO₂ emissions per capita for each year.

Added a new column with ranking values.
