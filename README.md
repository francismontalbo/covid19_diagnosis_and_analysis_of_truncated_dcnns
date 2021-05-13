<p> Author: Francis Jesmar P. Montalbo </p>
<p> Affiliation: Batangas State University </p>
<p> Email: francismontalbo@ieee.org </p>
<p><a href="https://francismontalbo.github.io">Personal Webpage</a></p>
***PLEASE CONTANCT ME IF YOU ARE HAVING TROUBLE. I CAN OFFER ASSITANCE***
  
***:heavy_exclamation_mark:This GitHub repository serves as a support for a submitted article in INFORMATION FUSION ISSN: 1566-2535 for publication.*** 


<p>CITATION</p>

# Graphical Abstract

<b>Made with <a target=_blank href="https://draw.io">draw.io</a></b>
<img src="/graphics/Montalbo_graphical_abstract_covid19.jpg" alt="comparative_study" width="1000">

# Dataset: 
## CT SCAN
<p><a href="https://www.kaggle.com/maedemaftouni/large-covid19-ct-slice-dataset">Large COVID-19 CT scan slice dataset.</a><p>
<h3>Citation</h3>
<p>M. Maftouni, "Large COVID-19 CT scan slice dataset", Kaggle.com, 2021. [Online]. Available: https://www.kaggle.com/maedemaftouni/large-covid19-ct-slice-dataset.</p> 
<p>X. Yang, X. He, J. Zhao, Y. Zhang, S. Zhang, and P. Xie, “COVID-CT dataset: A CT scan dataset about COVID-19,” 2020, arXiv:2003.13865. [Online]. Available: http://arxiv.org/abs/2003.13865</p>
<p>P. Afshar et al., “COVID-CT-MD, COVID-19 computed tomography scan dataset applicable in machine learning and deep learning”, Scientific Data, vol. 8, no. 1, 2021. doi: 10.1038/s41597-021-00900-3.</p>
<p>J. Paul Cohen, P. Morrison, and L. Dao, “COVID-19 image data collection,” 2020, arXiv:2003.11597. [Online]. Available: http://arxiv.org/abs/2003.11597.</p>  
<p>S. Morozov et al., “Mosmeddata: Chest ct scans with covid-19 related findings,” 2020, arXiv:2005.06465. [Online]. Available: https://arxiv.org/abs/2005.06465.</p> 
<p>M. Rahimzadeh, A. Attar, and S. M. Sakhaei, “A fully automated deep learning-based network for detecting covid-19 from a new and large lung ct scan dataset,” medRxiv, 2020. [Online]. Available: https://www.medrxiv.org/content/early/2020/06/12/2020.06.08.20121541.</p>
<p>M. Jun et al., “COVID-19 CT Lung and Infection Segmentation Dataset,” Zenodo, Apr, vol. 20, 2020. Available: https://zenodo.org/record/3757476#.YJfUtrUzZBc.</p>
<p>"COVID-19." 2020. [Online]. Available: http://medicalsegmentation.com/covid19/.  [Accessed: 02-March-2021].</p>


## CHEST X-RAY
<p><a href="https://data.mendeley.com/datasets/9xkhgts2s6/1">Curated Dataset for COVID-19 Posterior-Anterior Chest Radiography Images (X-Rays).</a></p>
<h3>Citation</h3>
<p>SAIT, UNAIS; k v, Gokul Lal; Prajapati, Sunny; Bhaumik, Rahul; Kumar, Tarun; S, Sanjana; Bhalla , Kriti (2020), “Curated Dataset for COVID-19 Posterior-Anterior Chest Radiography Images (X-Rays).”, Mendeley Data, V1, doi: 10.17632/9xkhgts2s6.1 http://dx.doi.org/10.17632/9xkhgts2s6.1</p>

***:heavy_exclamation_mark:For a faster method of replication, you may download the already prepared dataset used in this work by clicking the link below.*** 

<a href="https://drive.google.com/drive/u/1/folders/1wg6uiF-Y-qQobruR0_nv7XqzkvB7ubVj">CLICK ME FOR THE PREPARED DATASET</a>

# How to use:
***:heavy_exclamation_mark:If training the model, the dependencies included a `tensorflow-gpu`. You may change the `tensorflow-gpu` to `tensorflow` if no GPU is to be used. However, the results from the paper were produced using a GPU (GTX 1070) and Python 3.5x***

Dependencies included in the `requirements.txt`: 
- jupyter==1.0.0
- keras==2.2.5
- matplotlib
- numpy==1.16.2
- opencv-python==4.4.0.42
- pandas==0.25.3
- Pillow==7.2.0
- scikit-learn
- scikit-image
- scikit-plot
- scipy
- tensorflow-gpu==1.14.0 (Note: This is optional and can train even with just a CPU or tensorflow non-gpu variant)

***:heavy_exclamation_mark: START HERE*** You may clone using git or download the repository and extract the files manually:
- Once cloned, CD into the folder and enter `pip install -r requirements.txt`. 
- After installation of the dependecies, there are two options to evaluate or use the model.

**First (easier):**
- Clone this repository or download as zip.
- Install the requirements on a newly created environment to prevent issues with other existing ones.
- Open the jupyter-notebooks and proceed with either training or validation.
**The weight size of the truncatedmodels are very small 😄 the follow are located in the `/weights/` folder.**
**For the full weighst of the full-length models you may use the link below to download as they are to large for Github**

<a href="https://drive.google.com/drive/u/1/folders/1wg6uiF-Y-qQobruR0_nv7XqzkvB7ubVj">CLICK ME FOR THE WEIGHTS OF THE FULL-LENGTH MODELS</a>



