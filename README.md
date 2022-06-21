# 05 Matplotlib - Pymaceuticals

## Background

This project analyzes data from a anti-cancer drug screening. The dataset is from an animal study, where 249 mice with cancer were tracked for their tumor growth through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens. 

Tables, figures and a summary are generated for technical report of the study.

## Skills

matplotlib | pandas | jupyter notebook | data cleaning | statistics | bar plot | pie plot | whisker plot | line plot | scatter plot | linear regression 

## Conclusions

The initial dataset is composed of 249 unique mice and a total of 1893 rows of treatments, however 5 rows of data concerning mouse g989 are duplicated and the instructions ask us to remove all treatments concerning this mouse, which leaves us with a total of 248 unique mice and 1880 rows of treatments in the clean_data.

1. The summary statistics table by drug regimen reveals that there are a total of 10 different group treatments. The mean of the tumor volume per treatment reveals that ramicane and capomulin are the most effective drug regimen at reducing tumor size (~40mm3), whereas ketapril is the least effective (~55mm3).

2. The bar chart reveals the total number of treatments per drug regimen. The plot indicates that the two most effective treatments are also the ones that have the most treatment timepoints measured (>228 each). However, they are followed by the least effective treatment, which had 188 treatment measurements. This might indicate that the number of treatments measured is not relevant for the effectiveness of the treatment. 
 
3. The pie chart shows that the gender distribution of the mice tested is fairly even between males and females, so we wouldn't expect the data to be skewed in regards to sex.

4. Analysis of the last timepoint for each of the four selected treatments indicates that, when considering only the last timepoint, the average tumor volume of all mice at the end of the treatment regimen was reduced for ramicane, and capomulin (<40mm2), whereas infubinol (despite having mouse ID 'c326' as an outlier) and ceftasmin were not effective at the end of the treatment with a high tumor volume >60mm3. The positive effect of the drug at reducing tumor size over time is clearly represented in the line chart of a representative mouse within the capomulin treatment, since the tumor size reduces as the timepoint of treatment increases.

5. Finally, the regression and correlation study shows that there is a strong positive correlation between the weight and the tumor size. This makes sense as the tumor volume will generally contribute to the overall weight of the animal.
