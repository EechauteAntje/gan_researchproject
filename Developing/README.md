# How to train the models
## Train a musegan model

The dataset that were used are the weimar jazz database and Jazz ML ready midi dataset og Kaggle. Download the midifiles from this link: [Weimar](https://jazzomat.hfm-weimar.de/download/downloads/RELEASE2.0_mid_unquant.zip) , [Kaggle](https://www.kaggle.com/datasets/saikayala/jazz-ml-ready-midi/download?datasetVersionNumber=2)

place the midi files in a folder called 'data'.

### Anaconda

- Create a new environment in anaconda.

    ``` cmd
    conda create -n gan python=3.6
    ```

    ``` cmd
    conda activate gan 
    ```

- Install the packages

    ``` cmd
    conda install -c anaconda cudatoolkit
    ```

    ``` cmd
    conda install -c conda-forge cudnn
    ```

    ``` cmd
    pip install tensorflow==2.5
    ```

    ``` cmd
    pip install music21
    ```

    ``` cmd
    pip install imageio
    ```

    ``` cmd
    conda install matplotlib
    ```

    ``` cmd
    pip install scikit-learn 
    ```


### Notebook

Go to the file 'musegan.ipynb'. Follow the notebook with explanations and make melodies.

## Train the magenta model

Magenta has a number of different models. In this project, the GANSynth model will be used. With this model, we are going to create a sound. I did this in Azure so that I could run the other model locally.

### Azure 

1. Create a new resource group.
2. Create a machine learning service.
3. Open the azure machine learning studio.
4. Create a compute instance.
5. Then go to Notebooks.

first install Magenta and tensorflow_gan
```cmd
> pip install magenta
> pip install tensorflow_gan
```
The files you need can be found in the github repository in the folder 'magenta'.

Place the folders and files in Azure.
The structure in azure will then look like this:

![](https://i.imgur.com/v24mkmX.png)


> In the 'data' folder, you can put your own samples of sounds that you like. Place them in '.wav' format and they must not be longer than 4 seconds. The model responds best to sounds that are constant.

Open the 'GAN.ipynb' fileand follow the notebook with explanation.

If everything went smoothly, the stucture in Azure should look like this:

![](https://i.imgur.com/B6mljaR.png)

In the 'Generated' folder, you will find your generated sounds or song.
