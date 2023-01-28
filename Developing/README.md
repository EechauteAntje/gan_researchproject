## Trainen van het musegan model

De dataset die wordt gebruikt is de weimar jazz database. Download de midifiles via deze link: [download](https://jazzomat.hfm-weimar.de/download/downloads/RELEASE2.0_mid_unquant.zip) 
plaats de midi files in een map met de naam 'data'

### Anaconda

- Maak een nieuw environment in anaconda.

    ``` cmd
    conda create -n gan python=3.6
    ```

    ``` cmd
    conda activate gan 
    ```

- Installeer de packages

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

Clone deze github link: [download](https://github.com/EechauteAntje/researchproject.git)

### Notebook

Ga naar de file ‘musegan.ipynb’. Volg the notebook met uitleg and maak melodieën.

## Trainen van het magenta model

Magenta het aantal verschillende modellen. Bij dit project wordt het GANSynth model gebruikt. Met dit model gaan we een sound creëeren. Ik heb dit gedaan in Azure zodat ik andere model lokaal kon runnen.

### Azure 

1. Maak een nieuwe resource group.
2. Maak een machine learning service aan.
3. Open de azure machine learning studio.
4. Maak een compute instance.
5. Ga dan naar Notebooks.

Installeer eerst Magente en tensorflow_gan
```cmd
> pip install magenta
> pip install tensorflow_gan
```
De files die je nodig hebt vind je in de github repository in de map 'magenta'.

Plaats de folders en files in Azure.
De structuur in azure ziet er dan als volgt uit:
![](https://i.imgur.com/v24mkmX.png)


> In de map 'data' kan je jouw eigen samples plaatsen van leuke sounds. Plaats ze in '.wav' format en niet langer dan 4 seconden. Het model reageert het beste op sounds die constant zijn.

Open de 'GAN.ipynb' file en volg de notebook met uitleg.

Als alles vlot is verlopen moet de stuctuur in Azure er als volgt uitzien:
![](https://i.imgur.com/B6mljaR.png)

In de map 'Generated' vind je jouw gegenereerde sounds of song.
