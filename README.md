# FPCUP - Working Group Africa

# Training: 
# Detecting plastic pollution and events of marine debris pollution using Sentinel -2

Emanuel Castanho (AIR Centre)

25 OCTOBER 2023

<hr>

### Setup on Docker (recommended):
1- Download Docker based on your operating system [here](https://www.docker.com/get-started/);

2- After installation using the recommended settings, start Docker without signing in and fill some information;

3- Download this repository, click on *<> Code* and select *Download ZIP*;

4- Unzip the downloaded file and move the *fpcup\_africa\_marine-debris-main* folder to your Desktop or other path (keep the path simple);

5- Open a terminal window inside the folder *fpcup\_africa\_marine-debris-main* and run the following commands: 

`docker build -t fpcup_africa_marine-debris-main .` (wait until it finishes the building)

`docker run -it -p 8888:8888 -v .:/home/jovyan/fpcup_africa_marine-debris-main fpcup_africa_marine-debris-main` (do this on the same terminal window)

6- The previous command will start Jupyter, open the server url (try the third url) on your browser; 

7- Download *data.zip* from [here](https://drive.google.com/drive/folders/1nd9JHQhgqmZi98GicBAgNLFDESFjtq0Z?usp=sharing), unzip it and replace inside *fpcup\_africa\_marine-debris-main*;

8- You are ready to run the notebook *fpcup\_africa\_marine-debris.ipynb*

### Setup on Conda (optional):
5- If you do not want to use Docker, try Miniconda. After step 4, open a terminal window inside the folder *fpcup\_africa\_marine-debris-main* and run the following commands:

`conda create -n fpcup_africa_marine-debris-env python=3.9`

`conda activate fpcup_africa_marine-debris-env`

`conda install -c conda-forge gdal=3.7.2`

`pip install notebook==7.0.6 localtileserver==0.7.2 geopandas==0.14.0 leafmap==0.27.0 scikit-learn==1.1.1 pyarrow==13.0.0`

6- On the same terminal window, run `jupyter notebook` to start.








