# TBpred: SVM-Based Prediction of Subcellular Localization of Mycobacterial Proteins Using Evolutionary Information and Motifs

TBpred is a computational web server developed for predicting the subcellular localization of mycobacterial proteins.

The tool predicts whether a mycobacterial protein belongs to cytoplasmic, integral membrane, secretory, or membrane-attached protein classes. TBpred uses support vector machine-based models, evolutionary information from PSSM profiles, HMM profiles, MEME/MAST motif search, and hybrid prediction strategies.

Web Server: https://webs.iiitd.edu.in/raghava/tbpred/



## Citation

Rashid, M., Saha, S., and Raghava, G. P. S. Support Vector Machine-based method for predicting subcellular localization of mycobacterial proteins using evolutionary information and motifs. BMC Bioinformatics, 8, 337, 2007.

https://doi.org/10.1186/1471-2105-8-337

This tool and dataset is also available on Zenodo at



## About the Research

Mycobacterium species include important pathogenic organisms such as Mycobacterium tuberculosis. Many mycobacterial proteins remain functionally unannotated, and knowing their subcellular localization can help understand their biological role, virulence, antigenic potential, and suitability as drug or vaccine targets.

Existing subcellular localization methods were developed mainly for eukaryotic, Gram-positive, Gram-negative, or human proteins. However, mycobacteria have a unique and complex cell wall structure, so a dedicated organism-specific prediction method was needed.

TBpred was developed to predict the subcellular location of mycobacterial proteins directly from protein sequence information.

Data Compilation: The study used 852 mycobacterial proteins extracted from Swiss-Prot. These proteins were grouped into four major subcellular localization classes: 340 cytoplasmic proteins, 402 integral membrane proteins, 50 secretory proteins, and 60 membrane-attached proteins.

Methodology: TBpred uses machine learning and motif-based approaches. The study developed models using amino acid composition, dipeptide composition, PSSM profiles generated from PSI-BLAST, HMM profiles, MEME/MAST motifs, and hybrid combinations of these methods.



## Key Features

### 1. Mycobacterial Subcellular Localization Prediction

Predictive Modeling: Allows users to submit mycobacterial protein sequences and predict their likely subcellular localization.

The tool predicts four major classes:

- Cytoplasmic proteins
- Integral membrane proteins
- Secretory proteins
- Membrane-attached proteins

Organism-Specific Prediction: TBpred was developed specifically for mycobacterial proteins, making it more suitable for Mycobacterium-related studies than general bacterial localization predictors.



### 2. SVM-Based Prediction Models

Amino Acid Composition Model: The amino acid composition-based SVM model achieved 82.51% overall accuracy with 68.47% average accuracy.

Dipeptide Composition Model: The dipeptide composition-based SVM model achieved 80.39% overall accuracy with 67.63% average accuracy.

PSSM-Based Model: The PSSM profile-based SVM model achieved 86.62% overall accuracy with 73.71% average accuracy.

Evolutionary Information: The PSSM-based model performed better than simple composition-based models, showing that evolutionary information improves subcellular localization prediction.



### 3. Motif and Hybrid Prediction

HMM-Based Prediction: HMM profiles were developed for each localization class, but their standalone performance was limited.

MEME/MAST Motif Prediction: MEME was used to discover motifs, and MAST was used to search these motifs in protein sequences.

Motif Strength: MEME/MAST performed well for secretory and membrane-attached proteins, while SVM performed better for cytoplasmic and integral membrane proteins.

Hybrid Model: The best hybrid model combined PSSM-based SVM prediction with MEME/MAST motif search.

Hybrid Performance: The hybrid model achieved 86.8% overall accuracy and 89.00% average accuracy.

Reliability Index: TBpred provides a reliability index to indicate confidence in prediction. About 62% of sequences with reliability index greater than or equal to 3 were predicted with about 95% accuracy.



### 4. Integrated Web-Bench

Sequence Submission: Users can submit mycobacterial protein sequences for prediction.

Prediction Options: Users can choose amino acid composition, dipeptide composition, PSSM-based SVM, or hybrid prediction models.

Hybrid Default Utility: The hybrid method combines motif-based prediction and PSSM-based SVM prediction for improved class-wise performance.

Output: The server predicts the subcellular localization class of the submitted protein.

User-Friendly Interface: TBpred provides a web-based platform for researchers working on mycobacterial protein annotation.



## Applications

Mycobacterial Genome Annotation: TBpred can help annotate newly sequenced or hypothetical mycobacterial proteins.

Tuberculosis Research: The tool can support studies on Mycobacterium tuberculosis proteins and their possible biological roles.

Drug Target Discovery: Subcellular localization can help prioritize proteins as potential drug targets.

Vaccine Candidate Identification: Secretory and membrane-attached proteins may act as surface antigens and can be useful for vaccine research.

Virulence Studies: TBpred can help identify proteins associated with host-pathogen interaction and mycobacterial pathogenicity.

Proteome-Scale Analysis: The tool can be used for large-scale prediction of localization patterns in mycobacterial proteomes.



## Contact and Authors

Prof. G.P.S. Raghava 

Email: raghava@iiitd.ac.in

Department of Computational Biology, 

Indraprastha Institute of Information Technology (IIIT-Delhi), New Delhi, India.


## Support

This work was supported by the Council of Scientific and Industrial Research and the Department of Biotechnology, Government of India.

This work has IMTECH communication number 02/2007.
