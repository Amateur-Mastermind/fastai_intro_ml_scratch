# fastai_dl1_scratch


### Local Linux Setup
Reference: https://forums.fast.ai/t/fastai-v0-7-install-issues-thread/24652

The way I plan on organizing it is...


1. Install / update to latest version of `conda` and `pip` 

2. Clone `fastai` repo into ~/src/ and setup a fastai conda environment
```
cd ~/src
git clone https://github.com/fastai/fastai.git
cd fastai
conda env create -f environment.yml
```

3. Use this (`fastai_dl1_scratch`) repo to track my notes/changes when going through the lesson notebooks (and perhaps for playing around with datasets in kaggle). (example for lesson1.ipynb which might already be checked)
```
cd ~/projects
git clone https://github.com/Amateur-Mastermind/fastai_dl1_scratch.git
ln -s ~/src/fastai/old/fastai fastai
cp ~/src/fastai/courses/dl1/lesson1.ipynb scratch-lesson1.ipynb
ln 
# copy dogscats data into scratch repo, also change the PATH variable in the notebook to point to it)
```
Reason for doing this is so that I can keep the fastai repo up to date while also having my notes/fastai projects in version control.

4. Activate conda env and start up Jupyter!
```
source activate fastai
jupyter notebook
```
