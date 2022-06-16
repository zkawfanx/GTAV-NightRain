# GTAV-NightRain: Photometric Realistic Large-scale Dataset for Night-time Rain Streak Removal
This repository contains all related issues of GTAV-NightRain dataset. Updates will be informed here in time.

#### News

- **2022.6.16:** The small version of GTAV-NightRain is uploaded to Google Drive.
- **2022.6.13:** The initial release of GTAV-NightRain is publicly available on Zenodo.


## Dataset

![](figures/examples.png)

The entire dataset consists of 12860 rainy images together with 1286 rain-free ground truths collected in GTA V and is divide into three subsets. The `set1` and `set3` were rendered with the default rain shape while `set2` was rendered with the one we created. 5000/500 rainy/clean images for `set1` and `set2` and 1860/186 rainy/clean images for `set3`. Every 10 rainy images correspond to 1 clean image and they are named as `0000_00.png` to `0000_09.png` and `0000.png`, respectively. The dataset is arranged in the structure as follows:
```shell
GTAV-NightRain (12860 rainy / 1286 clean)
    |
    |--set1/set2
    |   |--Train
    |   |    |--Rainy (5000 images)
    |   |    |--GT    (500  images)
    |   |--Test
    |        |--Rainy (500 images)
    |        |--GT    (50  images)
    |
    |--set3
        |--Rainy      (1860 images)
        |--GT         (186  images)
        |
        |--Test (The subset tested in the paper)
             |--Rainy (186  images)
             |--GT    (186  images)
```

The initial version of GTAV-NightRain dataset is already publicly available on Zenodo and the DOI is: https://zenodo.org/record/6638011. You can get access to the whole dataset on it. 


The size of the entire dataset (47.1 GB) is relatively large and may cause difficulty in access for some researchers interested in our dataset. Thus, we also provide a small version containing only 1 rainy image and 1 clean image for each scene. And you can download it by [Google Drive](https://drive.google.com/drive/folders/1Tsoh_9iCfYc2rtMCHnJACnKW5W_SOheb?usp=sharing) (3.2 GB for `set1` and `set2`, 1.0 GB for `set3`) or [Baidu Yun]()(Coming soon).

## Instructions on Data Collection
We made a series of modifications on GTA V and enabled it to be a good platform for data collection on deraining. The collection is not limited to night-time scenes after some issues get addressed in the game and we focus on night scenes in the initial version of dataset.

The specific tool dependency and modifications provided in `./instructions` folder. Following these instructions, you can collect paired rainy/clean images in GTA V on your own.

* [Tool Dependency](instructions/Tool_dependency.md)
* [Modifications on GTA V](instructions/Modifications.md)


## Contributions
The development of this dataset is still going on and there are still a lot to do in the future. We welcome your suggestions of either the dataset itself, or the procedure of data collection, or modifications on GTA V.

If you have any problems, questions, or suggestions regarding the dataset, please open an issue or contact me via zkawfanx@bit.edu.cn or zkawfanx@gmail.com.

## Problems Found
N/A at the moment.


## To Do
- [] Update Tool_dependency.md
- [] Update Modifications.md
- [] ...

## License
The GTAV-NightRain dataset is licensed by [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). It is made freely available to academic and non-academic entities for non-commercial purposes such as academic research, teaching, scientific publications, or personal experimentation. 