# gan_researchproject

Download de modellen via deze link: https://drive.google.com/file/d/1WQqJB9r9KGWD4Pn9iRvs3ZRyY8sJFdIv/view?usp=share_link 
Plaats de .h5 files in de map ‘files’.

### Anaconda

- Maak een nieuwe environment in anaconda.

``` 
conda create -n gan python=3.6
conda activate gan 
```

- Installeer volgende packages

``` 
conda install -c anaconda cudatoolkit
conda install -c conda-forge cudnn
pip install tensorflow==2.5
pip install music21
pip install imageio
conda install matplotlib
pip install scikit-learn 
```

### Notebook

Ga naar de file ‘Generator.ipynb’ volg de notebook met uitleg en creëer nieuwe muziek.
