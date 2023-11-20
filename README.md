# Palestine_Israel_fatalaties
This project shows the total number of fatalaties of both palestinians and israelis from october 2000 to october 2023

##### Dataset: https://statistics.btselem.org/en

##### Data Visualisation: 


# Introduction

The conflict between Israel and Palestine is a protracted and deeply entrenched struggle that has shaped the geopolitical landscape of the Middle East for decades. At the heart of the conflict lies the issue of territory, with Israel having occupied Palestinian territories, including Gaza, for nearly 75 years. The occupation has given rise to a myriad of complex challenges, exacerbating tensions and contributing to a cycle of violence.

One of the key points of contention is the establishment of illegal settlements in the West Bank, further complicating the prospects for a peaceful resolution. These settlements, deemed illegal under international law, have been a source of ongoing friction, as they encroach upon land that is central to the Palestinian quest for statehood. The issue of settlements, coupled with historical grievances and competing national aspirations, continues to be a focal point of the conflict.

Understanding the historical context and the impact of prolonged occupation is crucial in comprehending the multifaceted nature of the Israel-Palestine conflict. As the international community grapples with potential solutions, the challenge remains to address the deep-rooted issues and find a path toward a just and sustainable resolution for both parties involved.


# Ask 

The following questions will aid the analysis process:
1. which regiion was subjected to the most fatalities.
2. which year encountered the most fatalities.
3. which citizinship had the highest fatalities. 


#### Data source:
The total number of fatalaties of both palestinians and isrealis will be analysed and interpreted from Oct 2000 to Oct 2023.

#### Data structure:
The following columns are included in this dataset: name, gender, age, citizenship, event_location_region, date_of-death, place-of_residence, place-of_residence-district, type_of_injury, killed_by. 

#### Process:
Due to the size of the dataset, the file is imported to bigquery to analyse the data using SQL. 


# Data Exploration

1. The total number of rows are checked. The total is 11124. 

<img width="546" alt="image" src="https://github.com/AAGH98/Palestine_Israel_fatalaties/assets/141926743/46e84090-9bf1-4629-b2ec-00249d8de766">

2. The table below shows all column names and their data types.

<img width="284" alt="image" src="https://github.com/AAGH98/Palestine_Israel_fatalaties/assets/141926743/ad4e9451-c40d-46ba-a484-af1b8df26eba">

3. During the cleaning process, the data is checked for any null values.

<img width="595" alt="image" src="https://github.com/AAGH98/Palestine_Israel_fatalaties/assets/141926743/db5ce3b6-f0a6-4523-b804-e0034f1eb5ba">

- The table below shows the null values in each column.

<img width="1156" alt="image" src="https://github.com/AAGH98/Palestine_Israel_fatalaties/assets/141926743/7ee0a177-f04f-43a7-a958-57807a66e386">




4. Since the column 'name' does not have any null values, it is checked for any duplicates.

<img width="551" alt="image" src="https://github.com/AAGH98/Palestine_Israel_fatalaties/assets/141926743/3363cd26-5155-4c02-ad4f-db7660a77149">


- There are no duplicate rows. 

5. The citizenship column is checked to see how many citizenships are available. There are 2 citizenships. 

<img width="587" alt="image" src="https://github.com/AAGH98/Palestine_Israel_fatalaties/assets/141926743/5b75891c-1248-4f7a-bef1-e17499c903e8">


6. The event_location_region is checked to how many regions are in this dataset. There are 3 regions. 

<img width="816" alt="image" src="https://github.com/AAGH98/Palestine_Israel_fatalaties/assets/141926743/2cffb824-378e-4f03-b1a8-90ce258d956f">



# Data Cleaning

A new table wil clean data is created. This will allow the analysis to be more accurate and reliable. 

- All rows with missing values are removed.


<img width="1122" alt="image" src="https://github.com/AAGH98/Palestine_Israel_fatalaties/assets/141926743/96689a9e-71c7-4e52-a14e-c25469eb61ec">

- Total rows returned are 10,670 so 454 rows were removed.




# Analyse and Share 

The data was stored and prepared for appropriate analysis. Multiple tables have been queried using SQL and visualised in tableau. 

The follwing dashboard on Tableau was created. It shows the total fatalities of palestinians and israeilis from october 2000 to September 2023.

<img width="1214" alt="image" src="https://github.com/AAGH98/Palestine_Israel_fatalaties/assets/141926743/09728747-56a8-4f19-8cd5-3f25d3f2c13a">

#### Per Region:

- Three regions were included in this dataset, which shows where the fatalities occured.
- The most fatalities occured in the gaza strip with approximatley 7,000 fatalities in 23 years.
- This shows that the majority of the conflict took place in the Gaza strip.


#### Total Fatalities:

- This table shows the total number of fatalities and who they were killed by.
- The green colour represents Palestinians and the blue colour represents Israelis, which shows that approximatley 90% of Palestinians were killed by Israeli security forces and 9.23% of Israelis were killed by Palestinian civilians. 


#### Per Year:

- Overal, Palestinians have a higher fatality rate than Israelis, which increased to a peek of approximatley 2,500 Palestinain fatalities in 2014.
- Israeli fatalities have been steadily low throughout the years.  













