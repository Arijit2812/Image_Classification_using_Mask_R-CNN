# Image_Classification_using_Mask_R-CNN

**Local system**

Clone github repo https://github.com/ahmedfgad/Mask-RCNN-TF2

Create virtual environment (Anaconda prompt)

conda create -n mask-rcnn python=3.7.11

conda activate mask-rcnn

**Install Mask RCNN in the virtual environment**

python -m pip install -r requirements.txt

python setup.py install

Setup video link https://www.youtube.com/watch?v=Fu_km7FXyaU&t=393s

**NeSI system**

cd /nesi/project/agresearch03746/Mask-RCNN-TF2

module purge && module load Python/3.7.3-gimkl-2018b

export PYTHONNOUSERSITE=1

python3 -m venv --system-site-packages venv

venv/bin/pip install -U pip

venv/bin/pip install protobuf==3.20.0

venv/bin/pip install -r requirements.txt

venv/bin/python3 setup.py install

module purge && module load JupyterLab

nesi-add-kernel -v venv mask_rcnn Python/3.7.3-gimkl-2018b cuDNN/7.6.5.32-CUDA-10.0.130

**Slurm batch job script that can be used to run the Python script version of the hoof_test task**
	
 sbatch hoof_test.sl

 **Inference was run for only one image at a time**

 ![image](https://github.com/Arijit2812/Image_Classification_using_Mask_R-CNN/assets/65775311/378cf827-651e-4b9c-b0b4-91f3f1356d6b)

 
**Sample result on Shiny App**

![Shiny3](https://github.com/Arijit2812/Image_Classification_using_Mask_R-CNN/assets/65775311/e755176d-11f6-4973-aaf0-1e43d3282bb6)

