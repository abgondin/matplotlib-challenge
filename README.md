# 05 Matplotlib - Pymaceuticals

## Background

This project analyzes data from a anti-cancer drug screening. The dataset is from an animal study, where 249 mice with cancer were tracked for their tumor growth through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens. 

Tables, figures and a summary are generated for technical report of the study.

## Skills

matplotlib | pandas | jupyter notebook | data cleaning | statistics | bar plot | pie plot | whisker plot | line plot | scatter plot | linear regression 

## Conclusions

The initial dataset is composed of 249 unique mice and a total of 1893 rows of treatments, however 5 rows of data concerning mouse g989 are duplicated and the instructions ask us to remove all treatments concerning this mouse, which leaves us with a total of 248 unique mice and 1880 rows of treatments in the clean_data.

1. The summary statistics table by drug regimen reveals that there are a total of 10 different group treatments. The mean of the tumor volume per treatment reveals that ramicane and capomulin are the most effective drug regimen at reducing tumor size (~40mm3), whereas ketapril is the least effective (~55mm3).

<img width="518" alt="Screen Shot 2022-06-21 at 10 34 57 pm" src="https://user-images.githubusercontent.com/77761497/174800739-2d9a3263-d42b-4346-aad8-c4c2f063fe11.png">

2. The bar chart reveals the total number of treatments per drug regimen. The plot indicates that the two most effective treatments are also the ones that have the most treatment timepoints measured (>228 each). However, they are followed by the least effective treatment, which had 188 treatment measurements. This might indicate that the number of treatments measured is not relevant for the effectiveness of the treatment. 

<img width="387" alt="Screen Shot 2022-06-21 at 10 35 18 pm" src="https://user-images.githubusercontent.com/77761497/174800949-da64bc32-6055-478d-b017-f0cb0d781815.png">
 
3. The pie chart shows that the gender distribution of the mice tested is fairly even between males and females, so we wouldn't expect the data to be skewed in regards to sex.

<img width="177" alt="Screen Shot 2022-06-21 at 10 35 47 pm" src="https://user-images.githubusercontent.com/77761497/174801070-ad84427a-d9b0-409d-a783-a9dab572b842.png">

4. Analysis of the last timepoint for each of the four selected treatments indicates that, when considering only the last timepoint, the average tumor volume of all mice at the end of the treatment regimen was reduced for ramicane, and capomulin (<40mm2), whereas infubinol (despite having mouse ID 'c326' as an outlier) and ceftasmin were not effective at the end of the treatment with a high tumor volume >60mm3. 
 
<img width="389" alt="Screen Shot 2022-06-21 at 10 36 03 pm" src="https://user-images.githubusercontent.com/77761497/174801225-6917d0d6-a677-45e4-99be-4e0a7a9b54d7.png">

The positive effect of the drug at reducing tumor size over time is clearly represented in the line chart of a representative mouse within the capomulin treatment, since the tumor size reduces as the timepoint of treatment increases.

<img width="381" alt="Screen Shot 2022-06-21 at 10 36 24 pm" src="https://user-images.githubusercontent.com/77761497/174801493-04243c24-28a7-4d36-b066-8df71ebc90f8.png">

5. Finally, the regression and correlation study shows that there is a strong positive correlation between the weight and the tumor size. This makes sense as the tumor volume will generally contribute to the overall weight of the animal.

<img width="385" alt="Screen Shot 2022-06-21 at 10 36 37 pm" src="https://user-images.githubusercontent.com/77761497/174801661-069d7377-a945-4c61-bbe2-a02395ff2eac.png">

