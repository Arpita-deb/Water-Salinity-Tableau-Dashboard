# Hamlet Level Tube well and river salinity in Indian Sundarban 2019 Tableau Dashboard

# Introduction:

This interactive dashboard is designed to analyze the salinity levels of tube wells and rivers within the North 24 Parganas and South 24 Parganas districts, collectively known as the Sundarban Region of the Indian Subcontinent. The initiative aligns with the global observance of World Water Day on March 22nd, aiming to highlight and educate about the adverse effects of human-induced water pollution.

Incorporating recent field data, it's evident that water becomes non-potable when salinity surpasses **1 part per thousand (ppt)**, and unsuitable for dry season paddy irrigation beyond **2 ppt**. Alarmingly, in the Sundarban Reclaimed Area, tube-well water salinity has been recorded above 1 ppt in 17 out of 50 surveyed hamlets across Gosaba, Hingalganj, and Patharpratima blocks. Furthermore, salinity levels in the Bidya, Matla, Hooghly, and Raimangal Rivers have been measured at a staggering **13-27 ppt**, underscoring the urgency for action and awareness.

## Salinity:

The salinity of water is a crucial factor in estuarine ecosystems. It refers to the amount of dissolved salts in water.

![Graphic breakdown of water salinity, defining freshwater, brackish water, saltwater, and brine water](https://upload.wikimedia.org/wikipedia/commons/thumb/9/98/Water_salinity_diagram.png/800px-Water_salinity_diagram.png) 

## Measurement:  

It is typically expressed in parts per thousand (ppt), g/L or g/kg(%).

## Salinity Category: 

1. **Oligohaline**: This category corresponds to freshwater from rivers, with a salinity of **0.5 parts per thousand (ppt) or less** ¹². Oligohaline areas are influenced primarily by river inflow.

2. **Mesohaline**: Within the estuary, mesohaline regions have salinity levels ranging from **5.0 to 18.0 ppt** ¹². These areas experience a mix of freshwater and seawater, creating a dynamic environment.

3. **Polyhaline**: Polyhaline zones exhibit higher salinity, typically ranging from **18.0 to 30.0 ppt** ¹². They are closer to the open sea and have salinity levels similar to ocean water.

# About the dataset:

The data for this visualization is collected from World Bank Data Catalog and can be accessed [here](https://datacatalog.worldbank.org/search/dataset/0038270/India---Water--Tube-well-and-River--Salinity-in-Indian-Sundarban). 

This dataset was prepared by Sreejit Roy, Saptarshi Chakraborty, Tapas Kumar Sutradhar and Santadas Ghosh. It contains data about Bidya, Matla, Hooghly, and Raimangal Rivers Rivers and Tubewell from Gosaba, Hingalgunj and Patharpratima blocks of the Sundarban Reclaimed (populated) Area in India.. It contains 2 tables namely **Tubewell Salinity** and **River Salinity** and contains 50 and 43 datapoints repectively. 

# Data Dictionary:

### 1. Tubewell_Salinity

| Column Name | Type | Description |
| :--- | :--- | :--- |
| CD Block  | char |  Community Development (CD) block, also Block, is a sub-division of a Tehsil (administrative unit) in India |
| Gram Panchayet	 | char | local administrative units at the village level |
| Hamlet Name	 | char | Name of the hamlet/village |
| Latitude | float | Latitude of the hamlet/village |
| Longitude	 | float | Longitude of the hamlet/village |
| Tube Well 1	 | float | Salinity of Tube Well 1 water |
| Tube Well 2	 | float | Salinity of Tube Well 1 water |
| Tube Well 3	 | float | Salinity of Tube Well 1 water |
| Tube Well 4	 | float | Salinity of Tube Well 1 water |
| Average Salinity (PPT) | float | Average Salinity of the tube wells water in that area |

### 2. River_Salinity

| Column Name | Type | Description |
| :--- | :--- | :--- |
| District  | char | Name of the district in West Bengal, India |
| Block | char | Community Development (CD) block, also known simply as a Block, is a sub-division of a Tehsil (administrative unit) |
| Gram Panchayet	| char | local administrative units at the village level |
| Hamlet Name	 | char | Name of the hamlet/village |
| Latitude | float | Latitude of the hamlet/village |
| Longitude	 | float | Longitude of the hamlet/village |
| Salinity (ppt) | float | The amount of dissolved salts in water, typically expressed in parts per thousand (ppt) or percentage (%) |	
| Salinity Category | char | Mesohaline/ Polihaline 1/ Polihaline 2/ Polihaline 3 |

# Resource:

* [Water Tubewell and River Salinity in Indian Sundarban Dataset](https://datacatalog.worldbank.org/search/dataset/0038270/India---Water--Tube-well-and-River--Salinity-in-Indian-Sundarban)
* [Salinity - Wikipedia](https://en.wikipedia.org/wiki/Salinity#Classification_of_water_bodies_based_upon_salinity)
* [Graphic breakdown of water salinity, defining freshwater, brackish water, saltwater, and brine water By Peter Summerlin - Own work, CC BY-SA 3.0](https://commons.wikimedia.org/w/index.php?curid=13274737)
