# project-covid
In this repo you will find all I used to perform statistical analysis on Mexico's COVID data.

All the data cleaning and analysis I performed can be found in MX_COVID.ipynb. The raw data I used can be found at: https://www.gob.mx/salud/documentos/datos-abiertos-bases-historicas-direccion-general-de-epidemiologia
The data dictionaries provided by the Mexican government are found in datos_abiertos_covid19.zip. When the file is unzipped, you will have a folder containing the dictionaries.
I created a virtual environment to work on this project, and all the requirements needed for reproducability are found in requirements.txt.

When performing my analysis, I attempted to answer the following questions:
1. Did Christmas lead to a peak in COVID cases in Mexico?
2. Is the indigenous minority of Mexico's population harder hit by the virus?

I performed Chi-square tests to answer both questions. 
I found a statistically significant relationship between time period and COVID cases, which led me to conclude that there was an increased number of cases after Christmas.
As one can see after taking a lot at the data dictionaries, there are 7 different classifications for determining whether an individual has COVID. Because of this, I performed two different analyses when answering the second question. I performed the Chi-square tests twice: once with only definitve classifications, and once with all classifications. Upon doing this, I got some interesting results. When using all classifications--non-definitive and definitive alike--there was a statistically significant relationship. In this case, there were less positive cases in those self-identifying as indigenous than those who do not identify as indigenous. On the other hand, when using only the definitive classifications, there was also a statistically significant relationship. This relationship was less statistically significant, and completely opposite to the previous finding: there were more positive cases in those who identify as indigenous.