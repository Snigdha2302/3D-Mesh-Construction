# 3D-Mesh-Construction
Installation 

uses Python 3.6, pytorch 1.1.0, cudatoolkit 9.1.0. 
we used conda to install packages - https://docs.anaconda.com/anaconda/packages/oldpkglists/

Installed with conda 
conda env create -f environment.yml
conda activate Total3D

Before executing demo files, for downloading pre trained model
https://livebournemouthac-my.sharepoint.com/personal/ynie_bournemouth_ac_uk/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fynie%5Fbournemouth%5Fac%5Fuk%2FDocuments%2FTotal3D%2Fpretrained%5Fmodel%2Epth&parent=%2Fpersonal%2Fynie%5Fbournemouth%5Fac%5Fuk%2FDocuments%2FTotal3D&originalPath=aHR0cHM6Ly9saXZlYm91cm5lbW91dGhhYy1teS5zaGFyZXBvaW50LmNvbS86dTovZy9wZXJzb25hbC95bmllX2JvdXJuZW1vdXRoX2FjX3VrL0VXdXlRWGVtQjI1R3E1c3NPWmZGS3lRQkE3dzJVUlhSM0hMdmpKaUtrQ2hhaUE_cnRpbWU9NU11RXRodVkyRWc
 
 and mesh generation net 
 
 https://livebournemouthac-my.sharepoint.com/personal/ynie_bournemouth_ac_uk/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fynie%5Fbournemouth%5Fac%5Fuk%2FDocuments%2FTotal3D%2Fmeshnet%5Fmodel%2Epth&parent=%2Fpersonal%2Fynie%5Fbournemouth%5Fac%5Fuk%2FDocuments%2FTotal3D&originalPath=aHR0cHM6Ly9saXZlYm91cm5lbW91dGhhYy1teS5zaGFyZXBvaW50LmNvbS86dTovZy9wZXJzb25hbC95bmllX2JvdXJuZW1vdXRoX2FjX3VrL0VjYndwVmlNRlFOQ2x1SHpXRjhQNS1nQkZqVldqbHFwOXYzYUs0QkU0MU0zR3c_cnRpbWU9VFBhY2ZSeVkyRWc
 
 1st Observation now, cd 3D-Mesh_Construction
 and python main.py configs/total3d.yaml --mode demo --demo_path demo/inputs/custom
 

 for preprocessed training/testing SUN RGB-D data set into data/sunrgbd/sunrgbd_train_test_data
 https://livebournemouthac-my.sharepoint.com/personal/ynie_bournemouth_ac_uk/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fynie%5Fbournemouth%5Fac%5Fuk%2FDocuments%2FTotal3D%2Fsunrgbd%5Ftrain%5Ftest%5Fdata%2Etar%2Egz&parent=%2Fpersonal%2Fynie%5Fbournemouth%5Fac%5Fuk%2FDocuments%2FTotal3D&originalPath=aHR0cHM6Ly9saXZlYm91cm5lbW91dGhhYy1teS5zaGFyZXBvaW50LmNvbS86dTovZy9wZXJzb25hbC95bmllX2JvdXJuZW1vdXRoX2FjX3VrL0VjQTY2TmIxYUkxS2l0elg3YXZiRTEwQmlIR3pvdmYzcnFRZWJlSkhtRkI0UUE_cnRpbWU9NDZzeEtCMlkyRWc
 
 then python utils/generate_data.py
 
 Preprocessed Pix3D
 Download pix3D dataset( http://pix3d.csail.mit.edu/ ) to data/pix3d/metadata 
 then Run python utils/preprocess_pix3d.py
 
 
 
