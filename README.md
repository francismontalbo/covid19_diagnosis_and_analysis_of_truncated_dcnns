<p> Author: Francis Jesmar P. Montalbo </p>
<p> Affiliation: Batangas State University </p>
<p> Email: francismontalbo@ieee.org </p>
<p><a href="https://francismontalbo.github.io">Personal Webpage</a></p>
***PLEASE CONTANCT ME IF YOU ARE HAVING TROUBLE. I CAN OFFER ASSITANCE***
  
***:heavy_exclamation_mark:This GitHub repository serves as the source code for a published paper.*** 
<p>CITATION</p>

# Paper

# Please Consider Citing. Thank you! 

<p>F. J. P. Montalbo, "Truncating Fined-Tuned Vision-Based Models to Lightweight Deployable Diagnostic Tools for SARS-CoV-2 Infected Chest X-Rays and CT-Scans," Multimedia Tools and Applications, 2022. doi: 10.1007/s11042-022-12484-0.</p>

<img src="/image/truncation_covid_preview.png" alt="covid_truncation_dcnn_montalbo_graphical_abstract_2022" width="1000">

# Dataset: 
## CT SCAN
<h3>Citation</h3>
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
***:heavy_exclamation_mark:If training the model, the dependencies included a `tensorflow-gpu`. You may change the `tensorflow-gpu` to `tensorflow` if no GPU is to be used. However, the results from the paper were produced using a GPU (GTX 1070) and Python 3.5x because of the baseline full-length models.***

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
- tensorflow-gpu==1.14.0 (Note: This is optional if training the truncated versions. However, training the full-length models may require a GPU)

***:heavy_exclamation_mark: START HERE*** You may clone using git or download the repository and extract the files manually:
- Once cloned, CD into the folder and enter `pip install -r requirements.txt`. 
- After installation of the dependecies, there are two options to evaluate or use the model.

**First (easier):**
- Clone this repository or download as zip.
- Install the requirements on a newly created environment to prevent issues with other existing ones.
- Open the jupyter-notebooks and proceed with either training or validation.
**The weight size of the truncated models are very small 😄 the following are located in the `/weights/` folder and can be used immediately.**
**For the baseline weights of the full-length models you may use the link below to download as they are too large for Github**
**REMEMBER! Re-producing the baseline results may take large computing resources, long hours, and a GPU. It is advised to just download the weights and load it on the corresponding notebooks*

<a href="https://drive.google.com/drive/u/1/folders/1wg6uiF-Y-qQobruR0_nv7XqzkvB7ubVj">CLICK ME FOR THE WEIGHTS OF THE FULL-LENGTH MODELS</a>


<!-- ## Performance Results and Specifications of the Truncated Models

<table style="width:100%", "text-align: center">
  <tr>
    <th>Model</th>
    <th>Accuracy <i>(%)</i></th> 
    <th>Precision <i>(%)</i></th>
    <th>Recall <i>(%)</i></th>
    <th>F1-Score <i>(%)</i></th>
    <th>Weight Size <i>(KB)</i></th>
  </tr>
  <tr>
    <td>Truncated InceptionResNetV2</td>
    <td><strong>97.41%</strong></td>
    <td><strong>97.59%</strong></td>
    <td><strong>97.52%</strong></td>
    <td><strong>97.55%</strong></td>
    <td>5,338</td>
  </tr>
  <tr>
    <td>Truncated InceptionV3</td>
    <td>97.36%</td>
    <td>97.46%</td>
    <td>97.40%</td>
    <td>97.43%</td>
    <td>5,188</td>
  </tr>
   <tr>
    <td>Truncated ResNet50V2</td>
    <td>86.12%</td>
    <td>87.77%</td>
    <td>86.78%</td>
    <td>87.25%</td>
    <td>1,081</td>
  </tr>
   <tr>
    <td>Truncated EfficientNetB0</td>
    <td>86.03%</td>
    <td>88.44%</td>
    <td>86.45%</td>
    <td>87.34%</td>
    <td>405</td>
  </tr>
   <tr>
    <td>Truncated DenseNet121</td>
    <td>77.98%</td>
    <td>80.86%</td>
    <td>76.72%</td>
    <td>78.25%</td>
    <td>714</td>
  </tr>
   <tr>
    <td>Truncated Xception</td>
    <td>78.82%</td>
    <td>81.11%</td>
    <td>80.43%</td>
    <td>80.25%</td>
    <td>739</td>
  </tr>
</table> -->

## Major credits to 
<p>https://github.com/totti0223/gradcamplusplus for the grad-cam implementations</p>
<p>Yosuke Toda, Ph.D (Agriculture)</p>
<p>tyosuke@aquaseerser.com</p>
<p>JST PRESTO ITbM, Nagoya University, Japan</p>

<p>https://github.com/lutzroeder/netron for the Netron model viewer</p>



## Citation :black_nib:

<p>F. J. P. Montalbo, "Truncating Fined-Tuned Vision-Based Models to Lightweight Deployable Diagnostic Tools for SARS-CoV-2 Infected Chest X-Rays and CT-Scans," Multimedia Tools and Applications, 2022. doi: 10.1007/s11042-022-12484-0.</p>

[Author Profile](https://scholar.google.com/citations?user=PV8dJDkAAAAJ&hl=en&oi=ao)



