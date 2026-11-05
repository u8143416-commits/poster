# Fire Severity and Animal Species Richness in Southeastern Australia
## Extended Abstract
### Aim
In 2019–2020, large-scale bushfires occurred in Australia. Following the fires, researchers conducted surveys of animals in different areas of southeastern Australia. I want to use the existing data to study whether there are differences in animal species richness in regions with different levels of fire severity. At the same time, I also want to know if the time of the survey and the geographical location are related to animal species richness. My prediction is that the higher the severity of the fire, the fewer animal species I expect to observe in the survey.
### Main Results
This study utilized 24 landscape locations and a total of 72 survey records. I analyzed the relationships between fire severity, geographical location, survey period, and camera survey time and the species richness of animals using a mixed-effects model.
The model results showed that the coefficients for low to moderate fire severity and high fire severity were -3.14 and -2.59 respectively, while the coefficient for extremely high fire severity was 8.21. However, the 95% confidence intervals of these three coefficients all included 0, so there was not sufficient evidence to indicate a clear relationship between fire severity and animal species richness.
Compared with the first survey, the estimated species richness in the second and third surveys was 3.72 and 5.62 lower respectively. No clear differences were found between different regions. Additionally, the longer the camera survey time, the more animal species were typically recorded.
There are two points to note in this section: Firstly, the model not finding a clear relationship does not mean that wildfires have no impact on animals at all. Secondly, the differences in survey periods cannot directly prove a decrease in animal numbers because we are analyzing the species richness recorded by cameras.
### Implications
My analysis did not reveal a clear relationship between the severity of the fire and the overall species richness of the animals. Spencer et al. (2022) also found that there was no significant difference in the overall species richness between the burned area and the unburned area, but the distribution of some animals was different. This indicates that the overall species richness did not change significantly, but it does not mean that all animals were not affected. Gorta et al. (2023) discovered that different biological groups responded differently to wildfires, and in some areas, there was an increase in biodiversity after the fire, while extremely severe fires might also be associated with a decline in biodiversity. Therefore, my results are consistent with some of the findings of previous studies, but they do not prove that the fire had no impact on the animals. This study has several limitations. Firstly, although there were 72 survey records, there were only 24 independent landscape locations in reality, so it might be difficult to detect smaller effects. Secondly, the species richness of animals comes from camera surveys, and some animals that are not easily captured by cameras might not have been recorded, and the deployment times of cameras in different survey periods also varied. Finally, my analysis did not directly compare the animals in the same landscape before and after the fire, so it is impossible to determine whether the fire truly caused a decrease in species richness, nor can it prove that the animal community has recovered.
## How to Reproduce the Analysis
This analysis was carried out using R version 4.5.2.
The main R packages used were:
- lme4 (version 2.1.0)
- ggplot2 (version 4.0.2)
The analysis is saved in fire_analysis.Rmd.
The original dataset is data_frame_landscapes_time_dryad.csv.
To reproduce my analysis:
1. Download the files from this GitHub repository.
2. Keep `fire_analysis.Rmd` and `data_frame_landscapes_time_dryad.csv` in the same folder.
3. Open `fire_analysis.Rmd` in RStudio.
## References

Linley et al. (2024). Widespread resilience of animal species, functional diversity, and predator–prey networks to an unprecedented gigafire. Journal of Applied Ecology.
https://doi.org/10.1111/1365-2664.14815

Spencer et al. (2022). One year on: rapid assessment of fauna and red fox diet after the 2019–20 mega-fires in the Blue Mountains, New South Wales. Australian Zoologist.
https://doi.org/10.7882/AZ.2022.033

Gorta et al. (2023). Multi-taxon biodiversity responses to the 2019–2020 Australian megafires. Global Change Biology.
https://doi.org/10.1111/gcb.16955
## Data Source 
The data used in this project came from Linley et al. (2024), "Widespread resilience of animal species, functional diversity, and predator–prey networks to an unprecedented gigafire."

I downloaded the original dataset from Dryad:
https://doi.org/10.5061/dryad.5qfttdzgn

The dataset contains 24 landscapes across three study areas, with three survey periods for each landscape, giving 72 observations in total.

The original data file is `data_frame_landscapes_time_dryad.csv`.

The dataset is available under the Creative Commons CC0 1.0 licence. It can be copied, used, and shared without permission. The original data source is cited in this project.
## Generative AI Declaration

I used ChatGPT (OpenAI) to help me check and correct errors in my R code and improve the logic of my analysis. I wrote the basic code myself, but used ChatGPT to help me find problems and make corrections. English is not my first language, so I also used ChatGPT to check grammar and improve the clarity of my writing. I have explained the use of AI in the relevant sections of my R Markdown file. I reviewed the changes and checked the code and results in RStudio.
