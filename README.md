Water Risk Profile of Corn, Soybean, and Potato in Minnesota (1951-2024)
This repository contains analysis code and data for evaluating water risk during critical growth stages of three major crops in Central Minnesota.
Project Overview
This project examines whether precipitation has historically met crop water demands during the most sensitive growth stages for:

Corn (VT-R1 stage: tasseling to silking)
Soybean (R3-R4 stage: pod formation)
Potato (Tuber initiation to bulking)

The analysis spans 74 years (1951-2024) across 13 Central Minnesota counties, combining historical climate data with field observations from 2023-2024.
Key Findings

Precipitation rarely matched evapotranspiration (ET) demands during water-sensitive growth stages
Rainfall met only 56% of corn water needs, 63% of soybean needs, and 53% of potato needs during critical periods
High year-to-year variability means crops face unpredictable water stress
No clear long-term trend of increasing or decreasing water risk was found
Bottom line: Irrigation remains essential for stable crop production in Central Minnesota, just as it has been historically

Repository Structure
Water-Risk-Profile/
├── Corn/           # Corn growth stage analysis and water risk calculations
├── Soybean/        # Soybean growth stage analysis and water risk calculations  
├── Potato/         # Potato growth stage analysis and water risk calculations
└── Results/        # Output figures, maps, and summary statistics
Methodology
Growth Stage Tracking

Uses Accumulated Growing Degree Days (AGDD) to predict when crops reach water-sensitive stages
Field data collected at Becker and Saint Paul, MN in 2023-2024
Crop-specific base temperatures:

Corn & Soybean: 50°F (10°C)
Potato: 44.6°F (7°C)



Water Demand Analysis

Compares precipitation to reference evapotranspiration (ET₀) and crop-adjusted ET (ETc)
Uses crop coefficients (Kc): 1.2 for corn, 1.15 for soybean and potato
Identifies timing mismatches between rainfall and peak water demand

Study Area
13 Central Minnesota counties: Wadena, Cass, Crow Wing, Todd, Morrison, Douglas, Otter Tail, Pope, Stearns, Sherburne, Benton, Hubbard, and Kandiyohi
Data Sources

Climate data: NOAA nClimGrid (1951-2024) - daily temperature and precipitation
Field observations: GEMS (Genetics, Environment, Management, Socioeconomics) sensor network
Evapotranspiration: Climate Engine (Hargreaves-Samani reference ET model)

Running the Analysis
The analysis uses Python with custom classes for each crop:

CornGDD - Calculates corn growing degree days
SoybeanGDD - Calculates soybean growing degree days
PotatoGDD - Calculates potato growing degree days

Requirements:

Python 3.x
Climate data from NOAA nClimGrid
County-level gridded temperature and precipitation data

Citation
If you use this code or data, please cite:

Subedi, S., Rozanov, A., Blumenfeld, K., Kantar, M., Sharma, V., & Runck, B. (2025). The Water Risk Profile of Corn, Soybean, and Potato in Minnesota from 1951-2024. Crop Science (submitted).

Funding
This project was funded by the Minnesota Environment and Natural Resources Trust Fund as recommended by the Legislative-Citizen Commission on Minnesota Resources (LCCMR).
Authors

Samikshya Subedi - GEMS Informatics Center, University of Minnesota
Aleksei Rozanov - GEMS Informatics Center, University of Minnesota
Kenneth Blumenfeld - Department of Soil, Water and Climate, University of Minnesota
Michael Kantar - University of Hawaii at Manoa
Vasudha Sharma - Department of Soil, Water and Climate, University of Minnesota
Bryan Runck - GEMS Informatics Center, University of Minnesota

Contact
For questions about this research, contact:

Bryan Runck: runck014@umn.edu
Vasudha Sharma: vasudha@umn.edu
