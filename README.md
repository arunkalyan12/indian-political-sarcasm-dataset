\# Indian Political Sarcasm Dataset



A labeled dataset for \*\*sarcasm detection in Indian political headlines\*\*, created as part of the research paper:



\*\*COMPARATIVE ANALYSIS OF MACHINE LEARNING AND DEEP LEARNING TECHNIQUES FOR SARCASM DETECTION IN INDIAN POLITICAL HEADLINES\*\*



\---



\## Authors

\- \*\*S. Sathish Kumar\*\* (Assistant Professor)  

\- \*\*Arunkalyan Muddamsetty\*\*\* (UG Student)  

\- \*\*Yash Tyagi\*\* (UG Student)  

\- \*\*Archana Gaddam\*\* (UG Student)  



\*\*Affiliation:\*\*  

Department of Computer Science and Engineering (Artificial Intelligence and Machine Learning)  

J B Institute of Engineering and Technology (JBIET), Hyderabad, India  



\*\*Corresponding Author:\*\*  

Arunkalyan Muddamsetty – arunmuddamsetty@gmail.com  



\---



\## Dataset Overview



This dataset consists of Indian political news headlines labeled for \*\*sarcasm detection\*\* using a combination of \*\*web scraping and LLM-based annotation (Gemini API)\*\*.



\---



\## Dataset Statistics



\### Raw Dataset

\- Total headlines collected: \*\*32,734\*\*



\### Labeled Dataset (Unbalanced)

\- Total labeled samples: \*\*32,524\*\*



\### Balanced Dataset (Used in Experiments)



| Label            | Count |

|------------------|------:|

| Non-Sarcastic    | 5892  |

| Sarcastic        | 5892  |

| \*\*Total\*\*        | \*\*11784\*\* |



\---



\## Dataset Structure

data/

├── raw/

│ └── raw\_headlines.csv

│

├── processed/

│ ├── full\_dataset.csv

│ └── balanced\_dataset.csv





\- \*\*raw/\*\* → Original scraped headlines  

\- \*\*full\_dataset.csv\*\* → Complete labeled dataset  

\- \*\*balanced\_dataset.csv\*\* → Class-balanced dataset used for experiments  



\---



\## Labeling Methodology



\- Data was labeled using \*\*Google Gemini API\*\*

\- Due to API constraints, labeling was performed in \*\*batches of 10,000 samples\*\*

\- Each headline was classified as:

&#x20; - \*\*Sarcastic\*\*

&#x20; - \*\*Non-Sarcastic\*\*



\---



\## Pipeline



web\_scraping.py → gemini\_labeling.py → dataset creation → balancing





\### Scripts

\- `web\_scraping.py` → Collects political headlines  

\- `gemini\_labeling.py` → Labels data using Gemini API  



\---



\## Usage



You can directly use:

\- `balanced\_dataset.csv` → for training \& evaluation  

\- `full\_dataset.csv` → for custom preprocessing / experiments  



\---



\## Citation (IEEE Format)



If you use this dataset, please cite:

\[1] A. Muddamsetty, S. S. Kumar, Y. Tyagi, and A. Gaddam,

“Indian Political Sarcasm Dataset,” 2026. \[Online].

Available: https://github.com/arunkalyan12/indian-political-sarcasm-dataset





\---



\## Research Context



This dataset was developed for evaluating and comparing:

\- Machine Learning models  

\- Deep Learning models  



for sarcasm detection in the \*\*Indian political domain\*\*.



\---



\## Notes



\- This dataset is intended for \*\*research and educational purposes\*\*

\- Labels are generated using LLM-based annotation and may contain minor noise

\- Contributions and improvements are welcome  



\---



\## Repository Link



https://github.com/arunkalyan12/indian-political-sarcasm-dataset



\---



\## License



This dataset and associated code are licensed under the MIT License - see the LICENSE file for details.

