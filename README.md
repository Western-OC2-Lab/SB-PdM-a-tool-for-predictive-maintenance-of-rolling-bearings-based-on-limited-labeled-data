# SB-PdM-a-tool-for-predictive-maintenance-of-rolling-bearings-based-on-limited-labeled-data
SB-PdM is a Similarity-Based (SB) Predictive-Maintenance (PdM) code to perform Predictive Maintenance (PdM) of rolling bearings without the need to train a classifier. It is a non-machine learning tool, where the classification task is performed by applying a similarity measure between test sample and class-reference labeled samples in the feature space. Specifically, a labeled reference vibration segment should be available for each operational condition "class". The monitoring of process integrity is then achieved by continuously measuring the similarity in the feature space between generated vibration segments and the labeled reference vibration segments. Accordingly, the classification of different operational conditions is achieved by evaluating the resulting similarity scores. The higher the similarity between a vibration segment and specific labeled reference segment, the higher the likelihood that they belong to the same condition "class".


<p float>
<img src="https://github.com/Western-OC2-Lab/SB-PdM-a-tool-for-predictive-maintenance-of-rolling-bearings-based-on-limited-labeled-data/blob/main/SB_PdM.png"/> 
</p>


The main aspects of the framework are feature extraction and similarity measure. Extracted features should be engineered so that they fulfill two main requirements:
<ul>
<li>Describe the inherent characteristics of all operational conditions “classes” in the data.
<li>Have high-discrimination degree between the different operational conditions in the data. 
<br>
</ul>
Regarding the similarity measure, it should provide a quantitative value that represents the similarity score between the two inputs. Accordingly, the similarity score can be used to assess the probability that the two inputs belong to the same class. The higher the similarity score, the higher the probability that they belong to the same class. In SB-PdM, The similarity measure is applied to the extracted features to quantify the similarity between the labeled reference vibration segments and the generated vibration segment in the feature space. Hence, it works as a similarity-based classifier. In contrast to supervised classification, where a labeled dataset is required for training, similarity-based classification requires one labeled reference vibration segment for each operational condition "class". This flexibility in data availability meets the requirements of most real-world industrial applications; especially in the early phases of solution deployment where only a limited amount of labeled data is available.

The Performance of the tool is evaluated on [the Case Western Reserve University (CWRU) bearing dataset](https://engineering.case.edu/bearingdatacenter). The tool is implemented in Python and Jupyter notebook provided. A  [code](https://github.com/Western-OC2-Lab/SB-PdM-a-tool-for-predictive-maintenance-of-rolling-bearings-based-on-limited-labeled-data/blob/main/Vibration_Dataset_Creation.ipynb) for processing .mat vibration files and creating the dataset is included as well.<br>


## Contact Information
For all inquiries or collaboration opportunities please contact: <br>

Email : saburakh@uwo.ca or Abdallah.Shami@uwo.ca <br>
Github: [SulAburakhia](https://github.com/SulAburakhia) or [Western OC2 Lab](https://github.com/Western-OC2-Lab) <br>
Google Scholar: [OC2 Lab](https://scholar.google.com.eg/citations?user=oiebNboAAAAJ&hl=en); [Sulaiman Aburakhia](https://scholar.google.com/citations?user=8x-pPSYAAAAJ&hl=en)


## Citation

If you find this repository useful in your research, please cite as:

S. A. Aburakhia, T. Tayeh, R. Myers and A. Shami, "Similarity-Based Predictive Maintenance Framework for Rotating Machinery", the Fifth International Conference on Communications, Signal Processing, and their Applications (ICCSPA’22), Cairo, Egypt, 27-29 December 2022.

