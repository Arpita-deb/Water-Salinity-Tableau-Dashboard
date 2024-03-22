# Navigating the Saline Waters: Sundarbans 2019

# Introduction:

This interactive dashboard is designed to analyze the salinity levels of tube wells and rivers within the North 24 Parganas and South 24 Parganas districts, collectively known as the Sundarban Region of the Indian Subcontinent. 

It serves as a crucial tool for stakeholders—including environmental agencies, policy makers, local communities, and non-governmental organizations—focusing on the Sundarban Region of the Indian Subcontinent. By providing detailed analyses of salinity levels in tube wells and rivers, the dashboard supports World Water Day on March 22nd, emphasizing the urgency of addressing water pollution. 

It aims to foster awareness among these key groups about the escalating challenges of water contamination and climate change. The insights gleaned from this dashboard can guide effective decision-making, promote sustainable water management practices, and catalyze initiatives to mitigate the impact of human activities on vital water resources.

## Salinity:

The salinity of water is a crucial factor in estuarine ecosystems. It refers to the amount of dissolved salts in water.

![Graphic breakdown of water salinity, defining freshwater, brackish water, saltwater, and brine water](https://upload.wikimedia.org/wikipedia/commons/thumb/9/98/Water_salinity_diagram.png/800px-Water_salinity_diagram.png) 

## Importance of Salinity:

Salinity levels in estuaries are crucial for various reasons:
* They determine the types of species that can live in these waters. Different species have different salinity tolerances.
* Salinity affects water density, which influences water circulation and the mixing of nutrients.
* It plays a role in the estuary's chemical processes, affecting oxygen levels and the health of the ecosystem.

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

# Data cleaning and Preprocessing:

After downloading the dataset, I've created a copy of it and removed the formattings. After that I've merged the two datasets and renamed it as Merged Sheet. The merged dataset contain 8 columns - Block, Gram Panchayat, Hamlet, Latitude, Longitude, River Salinity (PPT), Salinity Category and Tubewell Salinity (PPT). 
It contain 55 datapoints. 

# Analysis:

* *Number of Districts*: 2
* *Number of Blocks*: 7
* *Number of Gram Panchayat*: 16
* *Number of Hamlets*: 55
* *Average river water salinity*: 22.03255814 ppt
* *Average Tubewell water salinity*: 0.959702501 ppt
* *Average River salinity and number of hamlets by Salinity Category*:

![sal cat](https://github.com/Arpita-deb/Water-Salinity-Tableau-Dashboard/assets/139372731/90528e4e-4bb3-45c8-a57a-4d22928380d2)

* *Top 10 Hamlets in terms terms of average Tubewell Salinity*:

![tubewell sal](https://github.com/Arpita-deb/Water-Salinity-Tableau-Dashboard/assets/139372731/fd403b61-7f70-4a68-b37c-5556ce5e0011)

* *Top 10 Hamlets in terms terms of average River Salinity*:

![river sal](https://github.com/Arpita-deb/Water-Salinity-Tableau-Dashboard/assets/139372731/d1918720-2e43-4fd9-9f50-4d79b91a6e78)

* *Hamlets with Tubewell salinity greater than 1 ppt*:

![1ppt](https://github.com/Arpita-deb/Water-Salinity-Tableau-Dashboard/assets/139372731/52f7a213-6472-4c58-b138-dcf33da033f7)

# Tableau Dashboard:

In the interative tableau dashboard I created two geographical maps of the Indian Sundarban Region showing the Salinity levels of Rivers and Tubewells respectively. One can filter the datapoints according to district, Block, Gram Panchayat, Hamlet or Salinity Level. 

Along with the visualization, I also shared what is salinity, its categories, the salinity level for hamlets in question as well as how Salinity can adversely impact this region.

![Screenshot (359)](https://github.com/Arpita-deb/Water-Salinity-Tableau-Dashboard/assets/139372731/c0039d33-b772-4b9b-b5ed-39a2c3bbbc91)

![Screenshot (360)](https://github.com/Arpita-deb/Water-Salinity-Tableau-Dashboard/assets/139372731/204e3b57-8bd2-426b-a7eb-8d63d2635265)

# Conclusion:

The dashboard reveals that the upstream hamlets of the Delta region exhibit lower salinity levels in river water, yet the groundwater (tubewells) shows higher salinity. Downstream, as river water merges with seawater in estuaries, salinity increases. Consequently, downstream hamlets experience higher salinity in both river water, but surprisingly lower salinity in groundwater.

Data from the World Bank Group indicates that water salinity exceeding 1 part per thousand (ppt) renders it unsuitable for drinking, and surpassing 2 ppt makes it unfit for irrigation. Our analysis indicates that out of 55 hamlets, 17 have tubewell salinity levels above 1 ppt.

On the other hand, the average salinity level for rivers ranges from 13-27 ppt.

# Why Salinity matters?

High salinity affects the Sundarban region in several ways:
* It can lead to **soil degradation**, reducing soil productivity and affecting agriculture.
* Salinity intrusion can threaten the health of freshwater aquatic animals like fish and giant prawns.
* High soil salinity can damage the soil structure, inhibiting the growth of plant species and altering the local ecosystem.
* It also impacts the livelihoods of local communities, as it can cause shortages in drinking water and water scarcity for dry-season irrigation.

These effects highlight the importance of managing salinity levels to protect both the environment and the well-being of the Sundarban communities.

# Limitation of the project:

1. **Limited Dataset Size**: The dataset comprises approximately 50 observations, which restricts our ability to offer a comprehensive analysis of salinity levels across the Sundarban Region.

2. **Outdated Data**: The dataset's timeframe is confined to the year 2019, precluding the possibility of conducting an in-depth time series analysis to track salinity fluctuations and forecast future trends.

3. **Insufficient Supplementary Data**: The absence of additional data, such as geographical and demographic information for the Sundarban area, hampers the enhancement of our analysis.

# Additional Resources:

* [Water Tubewell and River Salinity in Indian Sundarban Dataset](https://datacatalog.worldbank.org/search/dataset/0038270/India---Water--Tube-well-and-River--Salinity-in-Indian-Sundarban)
* Photo by <a href="https://unsplash.com/@vishwasnavadak?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Vishwasa Navada K</a> on <a href="https://unsplash.com/photos/green-trees-beside-river-during-daytime-EK9u6IyUldw?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
* [Salinity - Wikipedia](https://en.wikipedia.org/wiki/Salinity#Classification_of_water_bodies_based_upon_salinity)
* [Graphic breakdown of water salinity, defining freshwater, brackish water, saltwater, and brine water By Peter Summerlin - Own work, CC BY-SA 3.0](https://commons.wikimedia.org/w/index.php?curid=13274737)
* [India - Water (Tube-well and River) Salinity in Indian Sundarban](https://datacatalog.worldbank.org/dataset/india-water-tube-well-and-river-salinity-indian-sundarban)
* [Swallowed by Water, in the Sundarbans There Is Nowhere Else to Go.](https://thediplomat.com/2024/01/swallowed-by-water-in-the-sundarbans-there-is-nowhere-else-to-go/)
