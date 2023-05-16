# Utah Historical Quarterly Dataset

Datasets from the article: "Who Tells Your Story? Analyzing a Century of Utah History" Utah Historical Quarterly 91, no. 1 (2023): 40-55. 
Link: https://scholarlypublishingcollective.org/uip/uhq/article-abstract/91/1/40/343256/Who-Tells-Your-Story-Analyzing-a-Century-of-Utah

Datasets were created by Spencer Stewart, Eliza McKinney, Dakota Bybee, and Seth Van Duzor. Special thanks to Holly George, Jed Rogers, and the Utah State Historical Society for their support of this project.

*Utah Historical Quarterly (UHQ) Dataset (JSON)*: Contains metadata and text for articles published in UHQ from 1928 to 2021 as obtained from the ISSUU platform. This includes article titles, author names, volume, issue, year, pages, description (usually  abstract), url, full text, references, and the word length of the full text. We also generated a "gender" category for authors (see note below). 

*UHQ Historical Figures Dataset (CSV)*: List of historical figures that appeared in the pages of the quarterly. We used Named Entity Recognition (spaCy) to extract person names from the quarterly, cleaned the results, ran the names through a gender prediction package (see note below), then counted the frequency with which the different names appeared in the pages of the quarterly. 

*Citation Dataset (CSV)*: Contains metadata for scholarship that cited UHQ articles. (Obtained from Google Scholar in May 2022)

Note on gender:
The gender prediction package that we used was created by Lincoln Mullen and draws from historical census records to predict a person's assigned gender at birth. When available, we consulted author bios or other historical sources to avoid any unintentional misgendering. But we still recognize that this approach doesn't account for the full spectrum of gender identities. Despite the problems of gender classification in data analysis, we nevertheless still found this approach illustrative in highlighting the sharp disparity in representation between men and women in the quarterly. 

Lincoln Mullen (2021). gender: Predict Gender from Names Using Historical Data. R package version 0.6.0. https://github.com/lmullen/gender
