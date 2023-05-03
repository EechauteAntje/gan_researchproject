# Generate music with this GAN model

Download the models from this link: [download](https://drive.google.com/drive/folders/10-S0SNllrL2Fub-Zz8szH9hTkeFeLZGL?usp=sharing).

Place the .h5 files in the map ‘files’.

## Anaconda

- Make a new environment in anaconda.

    ``` cmd
    conda create -n gan python=3.6
    ```

    ``` cmd
    conda activate gan 
    ```

- Install packages

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

## Notebook

Go to the file ‘Generator.ipynb’. Follow the notebook with explanations and create new music.
