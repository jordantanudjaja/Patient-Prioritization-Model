# Novo-Nordisk---Patient-Prioritization-Model
My team name is Impact Consulting Group (ICG) and this is a year-long project with Novo Nordisk to develop a Patient Ranking Model for the company to prioritize targeting specific patients most receptive to taking the company's anti-obesity drug, Saxenda

<h2>Background</h2>

Novo Nordisk (NN) is a leading global healthcare company that focuses on obesity, diabetes and haemophilia. More than one-third of US adults live with obesity, a serious chronic disease that increases the risk of having or acquiring other medical conditions, including depression, high blood pressure, etc. NN is developing anti-obesity medicines (AOMs) that can help Persons with Obesity (PwOs) lose excess weight. It currently has one FDA-approved medication, Saxenda, and has more AOMs in its pipeline. Despite the large proportion of PwOs in the US, NN has limited promotional resources that must be directed to selected segments of patients and prescribers that are expected to be the most appropriate and promotionally responsive. NN has considerable structured and unstructured commercial data, but lacks the data science knowledge required to extract relevant promotional response insights from that data. Therefore, this project seeks to apply machine learning and predictive modeling techniques to help the company process their data and derive insights that can guide their marketing decisions.

<h2>Methodology</h2>
<ol>
  <li>Created a patient-level relational database in SQL workbench by aggregating all the claim-level dataset from the Diagnosis (Dx), Procedure (Px), and Prescription (Rx) database and combining it with a socioeconomic dataset, created in Microsoft Excel using Policy Map datafiles from 2018. This relational database will act as the source of data for our machine learning model.</li>
  <li>Built the predictive model by using an unsupervised machine learning algorithm to cluster similar patients together into distinct groups, visualizing their characteristics and ranking them based on our insights and analysis of each group.</li>
  <li>Compiled a ZIP code level dataset from our patient level relational database, and ran a separate clustering algorithm to group similar ZIP codes together and conducted a similar visualization analysis to rank the different ZIP code groups.</li>
  <li>Combined both of the clustering models to classify each patient into one of 30 small buckets (1-A to 5-F). We analyzed each of these buckets to rank the top 15 according to how receptive each group of patients are to taking Saxenda, and designated similar buckets to higher-level categories.</li>
  <li>Recommended a few investment strategies and marketing campaigns to target certain patient categories over others, and justified those strategies by calculating estimated revenue earnings using NN’s patient investment data</li>
</ol>

<h2>Folders</h2>
<ul>
  <li><b>Final Report and Presentation:</b> Contains ICG's final report on the project and the Power Point presentation to the client</li>
  <li><b>Jupyter Notebook and Data:</b> Contains Python code for the Data Cleaning, Machine Learning, and Data Visualization of the model, and excel and csv files for socioeconomic data up to year 2018 and plantrak data for Saxenda patients</li>
  <li><b>SQL codes:</b> Contains SQL code in pdf format for the creation of the Patient Relational Database, comprised of patient-level data, prescriber-level data, and plantrak-level data</li>
  <li><b>Tableau Heatmaps:</b> Contains Tableau files that showcases heatmaps of the 4 Patient Groups generated from the ranking model: Enthusiasts, Convertibles, Potentials, Rejects</li>
</ul>
