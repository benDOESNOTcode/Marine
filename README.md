Toxic Waters: Marine Pollution and its Impact on Phytoplankton
Project Overview
This project analyzes the impact of increasing plastic pollution in the global oceans on marine biodiversity, specifically focusing on phytoplankton populations. Phytoplankton are critical primary producers of oxygen and play a vital role in regulating Earth's temperature. A decline in their population can lead to significant ecosystem imbalances and contribute to global warming.




Additionally, the project investigates human behavioral responses to pollution by checking whether fishing vessel activity has shifted or decreased in known pollution hotspots.
Datasets Used
The project integrates three major global datasets to correlate pollution, marine life, and human activity:

Microplastic Dataset (1972–2022): Records plastic density across oceans.


Source: NCEI (CSV format).


Scale: 11,671 rows and 22 features.


Key Features: Latitude, Longitude, Year, and Density Class.

Plankton Dataset (1958–2017): Records plankton population density via chlorophyll content.


Source: PANGAEA (Text format).




Scale: 37,722 rows and 49 features.




Key Features: Total Chlorophyll, Sea Surface Temperature (SST), and Surface PAR.


Vessels Dataset (2012–2020): Records global fishing effort.


Source: Global Fishing Watch (CSV format).


Scale: ~56 million rows and 6 columns.


Key Features: Fishing hours, date, and geographic coordinates.

Methodology
The analysis was performed using Python in a Jupyter Notebook environment, following these steps:


Data Cleaning: * Removed irrelevant metadata columns such as 'Event' and 'Paper DOI'.


Handled missing values (NaN) and renamed columns for consistency.


Rounded latitude and longitude values to facilitate merging across different datasets.


Exploratory Data Analysis (EDA):

Segmented data into three distinct time periods for longitudinal analysis: 1973–2000, 2001–2010, and 2011–2022.


Focused on chlorophyll content as a proxy for phytoplankton health.

Visualization:

Generated global maps of fishing effort density.


Created overlays comparing high-pollution regions with active fishing zones.

Key Findings

Phytoplankton Decline: There is a observed decline in phytoplankton populations over the years.



Pollution Correlation: While a potential link between increased plastic density and plankton decline exists, the correlation was found to be not yet statistically significant based on the current model.



Fishing Resilience: Despite the rise in marine pollution, global fishing effort has not decreased, even in heavily polluted areas.


Requirements
To run the analysis notebook (cs252a_fishFood.ipynb), you will need the following Python libraries:

pandas

numpy

matplotlib

geopandas (for processing fishing effort spatial data)

Installation & Usage
Clone the repository:

Bash

git clone https://github.com/[your-username]/marine-pollution-plankton.git
Install dependencies:

Bash

pip install pandas numpy matplotlib geopandas
Open the Jupyter Notebook:

Bash

jupyter notebook cs252a_fishFood.ipynb
