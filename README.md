# Comparing Driving Behavior of Humans and Autonomous Driving in a Professional Racing Simulator

Dataset for the experiments in [Comparing Driving Behavior of Humans and Autonomous Driving in a Professional Racing Simulator]().


## Circuit

From: https://en.wikipedia.org/wiki/Circuit_de_Barcelona-Catalunya

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9c/Formula1_Circuit_Catalunya.svg/1920px-Formula1_Circuit_Catalunya.svg.png">


## Segmentation 
Segments starting with *S* represent straights and segments starting with *C* represent corners. All values are in meters. 

|       | S01 | C01  | C04  | C05  | C07  | C09  | S09  | C10  | C12  | C13  | C14  |
|-------|-----|------|------|------|------|------|------|------|------|------|------|
| Start | 0   | 400  | 1300 | 1725 | 2050 | 2525 | 2840 | 3000 | 3350 | 3650 | 3840 |
| End   | 399 | 1299 | 1724 | 2049 | 2524 | 2839 | 2999 | 3349 | 3649 | 3839 | 4240 |

## Directory structure
    .
    ├── corner_features         # Features extracted from laps at each segment, corner and sector
    ├── data_set_v2             # Time series of the laps for each user including the AI driver
        ├── <for each driver>
            ├── laps            # laps in the time domain
            ├── laps_dist       # laps in the distance domain. 
                                  Where *distance* represents the distance through the racing line.
            lap_times.xlsx      # Summary of the laps
    ├── questionaries           # NASA-TLX and intake questionnaire
    ├── selected_laps           # Resulting laps from the clustering
    └── README.md


## Reference
If you find this code useful in an academic setting, please cite:

```
@article{remonda2020comparing,
  author = {Remonda, Adrian and and Veas, Eduardo and Luzhnica, Granit},
  title = {Comparing Driving Behavior of Humans and Autonomous Driving in a Professional Racing Simulator},
  journal = {PLOS},
  year = {2020}
}
```

