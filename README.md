# Description
One of the major challenges in drug development is having acceptable levels of efficacy and safety throughout all
the phases of clinical trials followed by the successful launch in the market. While there are many factors such as
molecular properties, toxicity parameters, mechanism of action at the target site, etc. that regulates the therapeutic
action of a compound, a holistic approach directed towards data-driven studies will invariably strengthen
the predictive toxicological sciences. Our quest for the current study is to find out various reasons as to why an
investigational candidate would fail in the clinical trials after multiple iterations of refinement and optimization.
We have compiled a dataset that comprises of approved and withdrawn drugs as well as toxic compounds and
essentially have used time-split based approach to generate the training and validation set. Five highly robust
and scalable machine learning binary classifiers were used to develop the predictive models that were trained
with features like molecular descriptors and fingerprints and then validated rigorously to achieve acceptable
performance in terms of a set of performance metrics. The mean AUC scores for all the five classifiers with the
hold-out test set were obtained in the range of 0.66–0.71. The models were further used to predict the probability
score for the clinical candidate dataset. The top compounds predicted to be toxic were analyzed to estimate
different dimensions of toxicity. Apparently, through this study, we propose that with the appropriate use of
feature extraction and machine learning methods, one can estimate the likelihood of success or failure of
investigational drugs candidates thereby opening an avenue for future trends in computational toxicological
studies.

# Data Collection
The compounds (small molecules) used to prepare the dataset in this
study were retrieved from DrugBank, DrugCentral, Liver
Toxicity Knowledge Base (LTKB), post-market withdrawn drugs, Tox21, and Inxight drugs. The SMILES (Simplified Molecular
Input Line Entry System) of all these compounds was cleaned,
and corresponding name of each drug was cross verified using the Online
Chemical Modeling Environment (OCHEM). While compiling
the drugs, though we retrieved drugs with multiple stereochemical
forms but if two or more stereochemical isomers of a drug is present in the same or different categories (approved or withdrawn) then only one
form was retained. This was done so as avoid redundancy in the set as we
have computed only the 2D descriptors wherein the stereoisomer information
is not available. Similarly, based on the InChIKey, the overall
redundancy was also removed and only the unique set was considered
for further processing. The selection of compounds from the Tox21
dataset was performed as described by Wu and co-workers,
wherein only those molecules which were reported to be active agonists
or antagonists in any one or more Tox21 assays, were considered.

# Web server

The tool is available at https://acds.neist.res.in:8502/ and als in the Advanced Module of Molecular Property Diagnostic Suite - Covid 19 (https://mpds.neist.res.in:8085/)

# Cite
John, L., Mahanta, H. J., Soujanya, Y., & Sastry, G. N. (2023). Assessing machine learning approaches for predicting failures of investigational drug candidates during clinical trials. Computers in biology and medicine, 153, 106494.
