The total number of residents in champaign county is: 209689. Total sutdents 44,087.
We can randomly put them into 5 home address, which is shown as the Residents column in Home.csv

Home_id.csv and Hospital_id.csv are home/hospital_name with id. id is the node id in OSMnx, which has been used to find the travel_time.(id combinations is the first column in Travel_time.csv) The ids and their pairs can be use to construct nodes and edges.

Age_group.csv contains the hospitalization(%), death(%), positive_cases(%) and recovery_time. For hospitalization(%), maybe it can be used to distribute % of people to self-quarantine or to become inpatient. Death(%) can be added with the negative_reduction_of_mortality_rate（multiply） (written as negative can help to solve the minimization problem) in treatment.csv, so that death rate can be reduced differently by different treatments.
 
travel time matrix

hospital id name 年龄段bed
home id 人数

Reduction_mortality(recovery_time)_rate(%) of Treatment.csv is to multiply the death(%) and recovery_time in each age group. For simplicity, the death(%) of ICU is also the reduction rate of ICU(Assume people go to ICU have 100% to death, then the death rate in ICU would be the 100% * reduction death in ICU)
The price in Treatment.csv is for patients with no insurance, because we are now in government perspective.

For simplicity, the number of beds/ventalitors/ICU-beds are assumed to be available number.