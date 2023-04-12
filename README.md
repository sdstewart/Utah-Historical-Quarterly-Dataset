# Utah Historical Quarterly Dataset

Datasets from the article: "Who Tells Your Story? Analyzing a Century of Utah History" Utah Historical Quarterly 91, no. 1 (2023): 40-55. 
Link: https://scholarlypublishingcollective.org/uip/uhq/article-abstract/91/1/40/343256/Who-Tells-Your-Story-Analyzing-a-Century-of-Utah

Datasets were created by Spencer Stewart, Eliza McKinney, Dakota Bybee, and Seth Van Duzor. Special thanks to Holly George, Jed Rogers, and the Utah State Historical Society. 

Utah Historical Quarterly (UHQ) Dataset (JSON): Contains metadata and text for articles published in UHQ from 1928 to 2021 obtained from the ISSUU platform. This includes article titles, author names, volume, issue, year, pages, description (usually the abstract), url, full text, references, and the length of the text. We also generated a "gender" category for authors (see note below). 

UHQ Historical Figures Dataset (csv): List of historical figures that appeared in the pages of the quarterly. We used Named Entity Recognition (spaCy) to extract  names from the quarterly, cleaned the results, ran the names through a gender prediction package (see note below), then counted the frequency with which the different names appeared in the pages of the quarterly. 

Citation Dataset (csv): Contains metadata for scholarship that cited UHQ articles. (Obtained from Google Scholar in June 2022)

Note on gender:
The gender prediction package that we used was created by Lincoln Mullen and draws from historical census records to predict a person's assigned gender at birth. This approach doesn't account for complex gender identities. Subsequently, when available, we consulted author bios or other historical sources to avoid any unintentional misgendering. While recognizing the complexities of gender classification, this approach was nevertheless illustrative in highlighting the sharp disparity in representation between men and women in the quarterly. 

Lincoln Mullen (2021). gender: Predict Gender from Names Using Historical Data. R package version 0.6.0. https://github.com/lmullen/gender
