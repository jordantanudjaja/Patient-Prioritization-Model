# Novo-Nordisk---Patient-Priortization-Project
Year-long project with Novo Nordisk to develop a Patient Ranking Model for the company to prioritize targeting specific patients most receptive to taking the company's anti-obesity drug, Saxenda

Background

Novo Nordisk (NN) is a leading global healthcare company that focuses on obesity, diabetes and haemophilia. More than one-third of US adults live with obesity, a serious chronic disease that increases the risk of having or acquiring other medical conditions, including depression, high blood pressure, etc. NN is developing anti-obesity medicines (AOMs) that can help Persons with Obesity (PwOs) lose excess weight. It currently has one FDA-approved medication, Saxenda, and has more AOMs in its pipeline. Despite the large proportion of PwOs in the US, NN has limited promotional resources that must be directed to selected segments of patients and prescribers that are expected to be the most appropriate and promotionally responsive. NN has considerable structured and unstructured commercial data, but lacks the data science knowledge required to extract relevant promotional response insights from that data. Therefore, this project seeks to apply machine learning and predictive modeling techniques to help the company process their data and derive insights that can guide their marketing decisions.

Methodology

Our approach to this problem is divided into 5 major steps. First, we created a patient-level relational database in SQL workbench by aggregating all the claim-level dataset from
the Diagnosis (Dx), Procedure (Px), and Prescription (Rx) database and combining it with a socioeconomic dataset, created in Microsoft Excel using Policy Map datafiles from 2018. This relational database will act as the source of data for our machine learning model.

Our next step is to build the predictive model by using an unsupervised machine learning algorithm to cluster similar patients together into distinct groups, visualizing their characteristics and ranking them based on our insights and analysis of each group.

Next, we compiled a ZIP code level dataset from our patient level relational database, and ran a separate clustering algorithm to group similar ZIP codes together and conducted a similar visualization analysis to rank the different ZIP code groups.

Subsequently, we combined both of the clustering models to classify each patient into one of 30 small buckets (1-A to 5-F). We analyzed each of these buckets to rank the top 15 according to how receptive each group of patients are to taking Saxenda, and designated similar buckets to higher-level categories.

Finally, we recommended a few investment strategies and marketing campaigns to target certain patient categories over others, and by using NN’s patient investment data, we calculated an estimate of the revenue earnings to justify our proposed strategies.
