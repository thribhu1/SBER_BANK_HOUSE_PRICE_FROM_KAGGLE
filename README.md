# SBER_BANK_HOUSE_PRICE_FROM_KAGGLE
The aim of this SBER bank is to predict the price of the property or buildings in Russia. Which helps its customers,developers and lenders to invest into it confidently. Predictions of price are not solely dependent on locality, area, material used , built in area , number of living rooms and number of floors in a building and ; which is related to the metadata of that property. But, also it depends on the russsian economy which is very unstable. This macroeconomic of the country dataset consist of huge set of features such as GDP and its growth , employment rate, birth rate, death rate, average salary growth rate , male to female ratio, ecology type , average retail share per capita in this way it consists of country feature dataset. In addition, this dataset also consists of complete data about the neighbours near by area. The KPI we using here is RMSLE - root mean square log error i.e log of root mean square error which is not affected to outliers and also penalize the underestimation of the price heavily.

**Type of Machine Learning Problem:-
We are predicting house prices based on the the locality and country finance so it is a regression Problem.

**Performance metric :-
This is regression problem we can use Mean square error, Mean Absolute error, Median Absolute error, R Squared (R2), this all can be used but RMSLE (Root Mean Squared Logarithmic Error) is used. In the case of RMSE or MSE the presence of outliers can explode the error term to a very high value. But, in the case of RMSLE the outliers are drastically scaled down because of log which nullify the outlier effect on the model. SO RMSLE is used . we may get doubt MAD can be used but MAD nullify the error greatly compare to mean absolute deviation. Here RMSLE could be a great fit can be used when you don’t want to penalize huge differences when both the values are huge numbers.Also, this can be used when you want to penalize under estimates more than over estimates.

Id :- transaction ID
Timestamp :- date of transaction
Full_sq : total area of property
Life_sq : living area
Floor :- for apartments, floor of the building
Max_floor : number of floors in the building
Material:- wall material used
Build_year :- year built
Num_room :- no of living room
Kitch_sq :- kitchen area
State : condition of the appartment
Product_type :- OwnerOccupier or Investement i
Sub_area :- district located
area_m :- muncipality area in, sq.m.
Raion_popul :- Number of municipality population in district
green_zone_part:- Proportion of area of greenery in the total area
indust_part Share of industrial zones in area of the total area
children_preschool Number of pre-school age population
preschool_quota Number of seats in pre-school organizations
preschool_education_centers_raion Number of pre-school institutions
children_school Population of school-age children
school_quota Number of high school seats in area
school_education_centers_raion Number of high school institutions
school_education_centers_top_20_raion Number of high schools of the top 20 best schools in
Moscow
hospital_beds_raion Number of hospital beds for the district
healthcare_centers_raion Number of healthcare centers in district
University_top_20_raion Number of higher education institutions in the top ten ranking of the
Federal rank
sport_objects_raion Number of higher education institutions
additional_education_raion Number of additional education organizations
culture_objects_top_25 Presence of the key objects of cultural heritage (significant objects for
the level of the RF constituent entities, city)
culture_objects_top_25_raion Number of objects of cultural heritage
shopping_centers_raion Number of malls and shopping centres in district
office_raion Number of malls and shopping centres in district
thermal_power_plant_raion Presence of thermal power station in district
incineration_raion Presence of incinerators
oil_chemistry_raion Presence of dirty industries
radiation_raion Presence of radioactive waste disposal
Railroad_terminal_raion Presence of the railroad terminal in district
big_market_raion Presence of large grocery / wholesale markets
nuclear_reactor_raion Presence of existing nuclear reactors
detention_facility_raion Presence of detention centers, prisons
full_all Total number of population in the municipality
male_f Male population
female_f Female population
young_all Population younger than working age
young_male Male population younger than working age
young_femaleFeale population younger than working age
work_all Working-age population
work_male Male working-age population
work_female Female working-age population
elder_all Population older than working age
elder_male Male population older than working age
elder_female Female population older than working age
0_6_all Population aged 0-6
0_6_male Male population aged 0-7
0_6_female Female population aged 0-8
7_14_all Population aged 7-14
7_14_male Male population aged 7-14
7_14_female Female population aged 7-14
0_17_all Population aged 0-17
0_17_male Male population aged 0-17
0_17_female Female population aged 0-17
16_29_all Population aged 16-19
16_29_male Male population aged 16-19
16_29_female Female population aged 16-19
0_13_all Population aged 0-13
0_13_male Male population aged 0-13
0_13_female Female population aged 0-13
raion_build_count_with_material_info Number of building with material info in district
build_count_block Share of block buildings
build_count_wood Share of wood buildings
build_count_frame Share of frame buildings
build_count_brick Share of brick buildings
build_count_monolith Share of monolith buildings
build_count_panel Share of panel buildings
build_count_foam Share of foam buildings
build_count_slag Share of slag buildings
build_count_mix Share of mixed buildings
Raion_build_count_with_builddate_info Number of building with build year info in district
build_count_before_1920 Share of before_1920 buildings
build_count_1921-1945 Share of 1921-1945 buildings
build_count_1946-1970 Share of 1946-1970 buildings
build_count_1971-1995 Share of 1971-1995 buildings
build_count_after_1995 Share of after_1995 buildings
metro_min_avto Time to subway by car, min.
metro_km_avto Distance to subway by car, km
metro_min_walk Time to metro by foot
metro_km_walk Distance to the metro, km
kindergarten_km Distance to kindergarten
school_km Distance to high school
park_km Distance to park
green_zone_km Distance to green zone
industrial_zone_km Distance to industrial zone
water_treatment_km Distance to water treatment
cemetery_km Distance to the cemetery
incineration_km Distance to the incineration (waste treatment process neary by)
railroad_station_walk_km Distance to the railroad station (walk)
railroad_station_walk_min Time to the railroad station (walk)
ID_railroad_station_walk Nearest railroad station id
railroad_station_avto_km Distance to the railroad station (avto)
railroad_station_avto_min Time to the railroad station (avto)
ID_railroad_station_avto Nearest railroad station id (avto)
public_transport_station_km Distance to the public transport station (walk)
public_transport_station_min_walk Time to the public transport station (walk)
water_km Distance to the water reservoir / river
water_1line First line to the river (150 m)
mkad_km Distance to MKAD (Moscow Circle Auto Road)
ttk_km Distance to the TTC (Third Transport Ring)
sadovoe_km Distance to the Garden Ring
bulvar_ring_km The distance to the Boulevard Ring
kremlin_km Distance to the city center (Kremlin)
big_road1_km Distance to Nearest major road
ID_big_road1 Nearest big road id
big_road1_1line First line to the road (100 m for highwys, 250 m to MKAD)
big_road2_km The distance to next distant major road
ID_big_road2 2nd nearest big road id
railroad_km Distance to the railway / Moscow Central Ring / open areas Underground
railroad_1line First line to the railway (100 m)
zd_vokzaly_avto_km Distance to train station
ID_railroad_terminal Nearest railroad terminal id
bus_terminal_avto_km Distance to bus terminal (avto)
ID_bus_terminal Nearest bus terminal id
oil_chemistry_km Distance to dirty industries
nuclear_reactor_km Distance to nuclear reactor
radiation_km Distance to burial of radioactive waste
power_transmission_line_km Distance to power transmission line
thermal_power_plant_km Distance to thermal power plant
ts_km Distance to power station
big_market_kmDistance to grocery / wholesale markets
market_shop_km Distance to markets and department stores
fitness_km Distance to fitness
swim_pool_km Distance to swimming pool
ice_rink_km Distance to ice palace
stadium_km Distance to stadium
basketball_km Distance to the basketball courts
hospice_morgue_km Distance to hospice/morgue
detention_facility_km Distance to detention facility
public_healthcare_km Distance to public healthcare
university_km Distance to universities
workplaces_km Distance to workplaces
shopping_centers_km Distance to shopping centers
office_km Distance to business centers/ offices
additional_education_km Distance to additional education
preschool_km Distance to preschool education organizations
big_church_kmDistance to large church
church_synagogue_km Distance to Christian chirches and Synagogues
mosque_km Distance to mosques
theater_km Distance to theater
museum_km Distance to museums
exhibition_km Distance to exhibition
catering_km Distance to catering
ecology Ecological zone where the house is located
green_part_500 The share of green zones in 500 meters zone
prom_part_500 The share of industrial zones in 500 meters zone
office_count_500 The number of office space in 500 meters zone
office_sqm_500 The square of office space in 500 meters zone
trc_count_500 The number of shopping malls in 500 meters zone
trc_sqm_500 The square of shopping malls in 500 meters zone
cafe_count_500 The number of cafes or restaurants in 500 meters zone
Cafe_sum_500_min_price_avg Cafes and restaurant min average bill in 500 meters zone
cafe_sum_500_max_price_avg Cafes and restaurant max average bill in 500 meters zone
cafe_avg_price_500 Cafes and restaurant average bill in 500 meters zone
cafe_count_500_na_price Cafes and restaurant bill N/A in 500 meters zone
cafe_count_500_price_500 Cafes and restaurant bill, average under 500 in 500 meters zone
cafe_count_500_price_1000 Cafes and restaurant bill, average 500-1000 in 500 meters zone
cafe_count_500_price_1500 Cafes and restaurant bill, average 1000-1500 in 500 meters zone
cafe_count_500_price_2500 Cafes and restaurant bill, average 1500-2500 in 500 meters zone
cafe_count_500_price_4000 Cafes and restaurant bill, average 2500-4000 in 500 meters zone
cafe_count_500_price_high Cafes and restaurant bill, average over 4000 in 500 meters zone
big_church_count_500 The number of big churchs in 500 meters zone
church_count_500 The number of churchs in 500 meters zone
mosque_count_500 The number of mosques in 500 meters zone
leisure_count_500 The number of leisure facilities in 500 meters zone
sport_count_500 The number of sport facilities in 500 meters zone
market_count_500 The number of markets in 500 meters zone
green_part_1000 The share of green zones in 1000 meters zone
prom_part_1000 The share of industrial zones in 1000 meters zone
office_count_1000 The number of office space in 1000 meters zone
office_sqm_1000 The square of office space in 1000 meters zone
trc_count_1000 The number of shopping malls in 1000 meters zone
trc_sqm_1000 The square of shopping malls in 1000 meters zone
cafe_count_1000 The number of cafes or restaurants in 1000 meters zone
cafe_sum_1000_min_price_avg Cafes and restaurant min average bill in 1000 meters zone
cafe_sum_1000_max_price_avg Cafes and restaurant max average bill in 1000 meters zone
cafe_avg_price_1000 Cafes and restaurant average bill in 1000 meters zone
cafe_count_1000_na_price Cafes and restaurant bill N/A in 1000 meters zone
cafe_count_1000_price_500 Cafes and restaurant bill, average under 500 in 1000 meters zone
cafe_count_1000_price_1000 Cafes and restaurant bill, average 500-1000 in 1000 meters zone
cafe_count_1000_price_1500 Cafes and restaurant bill, average 1000-1500 in 1000 meters zone
cafe_count_1000_price_2500 Cafes and restaurant bill, average 1500-2500 in 1000 meters zone
cafe_count_1000_price_4000 Cafes and restaurant bill, average 2500-4000 in 1000 meters zone
cafe_count_1000_price_high Cafes and restaurant bill, average over 4000 in 1000 meters zone
big_church_count_1000 The number of big churchs in 1000 meters zone
church_count_1000 The number of churchs in 1000 meters zone
mosque_count_1000 The number of mosques in 1000 meters zone
leisure_count_1000 The number of leisure facilities in 1000 meters zone
sport_count_1000 The number of sport facilities in 1000 meters zone
market_count_1000 The number of markets in 1000 meters zone
green_part_1500 The share of green zones in 1500 meters zone
prom_part_1500 The share of industrial zones in 1500 meters zone
office_count_1500 The number of office space in 1500 meters zone
office_sqm_1500 The square of office space in 1500 meters zone
trc_count_1500 The number of shopping malls in 1500 meters zone
trc_sqm_1500 The square of shopping malls in 1500 meters zone
cafe_count_1500 The number of cafes or restaurants in 1500 meters zone
cafe_sum_1500_min_price_avg Cafes and restaurant min average bill in 1500 meters zone
cafe_sum_1500_max_price_avg Cafes and restaurant max average bill in 1500 meters zone
cafe_avg_price_1500 Cafes and restaurant average bill in 1500 meters zone
cafe_count_1500_na_price Cafes and restaurant bill N/A in 1500 meters zone
cafe_count_1500_price_500 Cafes and restaurant bill, average under 500 in 1500 meters zone
cafe_count_1500_price_1000 Cafes and restaurant bill, average 500-1000 in 1500 meters zone
cafe_count_1500_price_1500 Cafes and restaurant bill, average 1000-1500 in 1500 meters zone
cafe_count_1500_price_2500 Cafes and restaurant bill, average 1500-2500 in 1500 meters zone
cafe_count_1500_price_4000 Cafes and restaurant bill, average 2500-4000 in 1500 meters zone
cafe_count_1500_price_high Cafes and restaurant bill, average over 4000 in 1500 meters zone
big_church_count_1500 The number of big churchs in 1500 meters zone
church_count_1500 The number of churchs in 1500 meters zone
mosque_count_1500 The number of mosques in 1500 meters zone
leisure_count_1500 The number of leisure facilities in 1500 meters zone
sport_count_1500 The number of sport facilities in 1500 meters zone
market_count_1500 The number of markets in 1500 meters zone
green_part_2000 The share of green zones in 2000 meters zone
prom_part_2000 The share of industrial zones in 2000 meters zone
office_count_2000 The number of office space in 2000 meters zone
office_sqm_2000 The square of office space in 2000 meters zone
trc_count_2000 The number of shopping malls in 2000 meters zone
trc_sqm_2000 The square of shopping malls in 2000 meters zone
cafe_count_2000 The number of cafes or restaurants in 1500 meters zone
cafe_sum_2000_min_price_avg Cafes and restaurant min average bill in 2000 meters zone
cafe_sum_2000_max_price_avg Cafes and restaurant max average bill in 2000 meters zone
cafe_avg_price_2000 Cafes and restaurant average bill in 2000 meters zone
cafe_count_2000_na_price Cafes and restaurant bill N/A in 2000 meters zone
cafe_count_2000_price_500 Cafes and restaurant bill, average under 500 in 2000 meters zone
cafe_count_2000_price_1000 Cafes and restaurant bill, average 500-1000 in 2000 meters zone
cafe_count_2000_price_1500 Cafes and restaurant bill, average 1000-1500 in 2000 meters zone
cafe_count_2000_price_2500 Cafes and restaurant bill, average 1500-2500 in 2000 meters zone
cafe_count_2000_price_4000 Cafes and restaurant bill, average 2500-4000 in 2000 meters zone
cafe_count_2000_price_high Cafes and restaurant bill, average over 4000 in 2000 meters zone
big_church_count_2000 The number of big churchs in 2000 meters zone
church_count_2000 The number of churchs in 2000 meters zone
mosque_count_2000 The number of mosques in 2000 meters zone
leisure_count_2000 The number of leisure facilities in 2000 meters zone
sport_count_2000 The number of sport facilities in 2000 meters zone
market_count_2000 The number of markets in 2000 meters zone
green_part_3000 The share of green zones in 3000 meters zone
prom_part_3000 The share of industrial zones in 3000 meters zone
office_count_3000 The number of office space in 3000 meters zone
office_sqm_3000 The square of office space in 3000 meters zone
trc_count_3000 The number of shopping malls in 3000 meters zone
trc_sqm_3000 The square of shopping malls in 3000 meters zone
cafe_count_3000 The number of cafes or restaurants in 1500 meters zone
cafe_sum_3000_min_price_avg Cafes and restaurant min average bill in 3000 meters zone
cafe_sum_3000_max_price_avg Cafes and restaurant max average bill in 3000 meters zone
cafe_avg_price_3000 Cafes and restaurant average bill in 3000 meters zone
cafe_count_3000_na_price Cafes and restaurant bill N/A in 3000 meters zone
cafe_count_3000_price_500 Cafes and restaurant bill, average under 500 in 3000 meters zone
cafe_count_3000_price_1000 Cafes and restaurant bill, average 500-1000 in 3000 meters zone
cafe_count_3000_price_1500 Cafes and restaurant bill, average 1000-1500 in 3000 meters zone
cafe_count_3000_price_2500 Cafes and restaurant bill, average 1500-2500 in 3000 meters zone
cafe_count_3000_price_4000 Cafes and restaurant bill, average 2500-4000 in 3000 meters zone
cafe_count_3000_price_high Cafes and restaurant bill, average over 4000 in 3000 meters zone
big_church_count_3000 The number of big churchs in 3000 meters zone
church_count_3000 The number of churchs in 3000 meters zone
mosque_count_3000 The number of mosques in 3000 meters zone
leisure_count_3000 The number of leisure facilities in 3000 meters zone
sport_count_3000 The number of sport facilities in 3000 meters zone
market_count_3000 The number of markets in 3000 meters zone
green_part_5000 The share of green zones in 5000 meters zone
prom_part_5000 The share of industrial zones in 5000 meters zone
office_count_5000 The number of office space in 5000 meters zone
office_sqm_5000 The square of office space in 5000 meters zone
trc_count_5000 The number of shopping malls in 5000 meters zone
trc_sqm_5000 The square of shopping malls in 5000 meters zone
cafe_count_5000 The number of cafes or restaurants in 1500 meters zone
cafe_sum_5000_min_price_avg Cafes and restaurant min average bill in 5000 meters zone
cafe_sum_5000_max_price_avg Cafes and restaurant max average bill in 5000 meters zone
cafe_avg_price_5000 Cafes and restaurant average bill in 5000 meters zone
cafe_count_5000_na_price Cafes and restaurant bill N/A in 5000 meters zone
cafe_count_5000_price_500 Cafes and restaurant bill, average under 500 in 5000 meters zone
cafe_count_5000_price_1000 Cafes and restaurant bill, average 500-1000 in 5000 meters zone
cafe_count_5000_price_1500 Cafes and restaurant bill, average 1000-1500 in 5000 meters zone
cafe_count_5000_price_2500 Cafes and restaurant bill, average 1500-2500 in 5000 meters zone
cafe_count_5000_price_4000 Cafes and restaurant bill, average 2500-4000 in 5000 meters zone
cafe_count_5000_price_high Cafes and restaurant bill, average over 4000 in 5000 meters zone
big_church_count_5000 The number of big churchs in 5000 meters zone
church_count_5000 The number of churchs in 5000 meters zone
mosque_count_5000 The number of mosques in 5000 meters zone
leisure_count_5000 The number of leisure facilities in 5000 meters zone
sport_count_5000 The number of sport facilities in 5000 meters zone
market_count_5000 The number of markets in 5000 meters zone


**Description of each feature in the data set
Data set column analysis



## there are many features in this data set which needs rigorous EDA to get the insight of this data.
