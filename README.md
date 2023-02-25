# Malware detectors on CTU-50

This repo contains the code and experiments to detect malware on CTU-50 dataset

# Data

In the folder `ctu-50-features` are the folders with the data. The data are preprocessed features for the TLS connections of the CTU-50 dataset.

The folders are:

        ├── Client1 (benign)
        │   ├── Day1
        │   │   └── comb_features.csv
        │   ├── Day2
        │   │   └── comb_features.csv
        │   ├── Day3
        │   │   └── comb_features.csv
        │   ├── Day4
        │   │   └── comb_features.csv
        │   └── Day5
        │       └── comb_features.csv
        ├── Client10 (benign)
        │   ├── Day1
        │   │   └── comb_features.csv
        │   ├── Day2
        │   │   └── comb_features.csv
        │   ├── Day3
        │   │   └── comb_features.csv
        │   ├── Day4
        │   │   └── comb_features.csv
        │   └── Day5
        │       └── comb_features.csv
        ├── Client2 (benign)
        │   ├── Day1
        │   │   └── comb_features.csv
        │   ├── Day2
        │   │   └── comb_features.csv
        │   ├── Day3
        │   │   └── comb_features.csv
        │   ├── Day4
        │   │   └── comb_features.csv
        │   └── Day5
        │       └── comb_features.csv
        ├── Client3 (benign)
        │   ├── Day1
        │   │   └── comb_features.csv
        │   ├── Day2
        │   │   └── comb_features.csv
        │   ├── Day3
        │   │   └── comb_features.csv
        │   ├── Day4
        │   │   └── comb_features.csv
        │   └── Day5
        │       └── comb_features.csv
        ├── Client4 (benign)
        │   ├── Day1
        │   │   └── comb_features.csv
        │   ├── Day2
        │   │   └── comb_features.csv
        │   ├── Day3
        │   │   └── comb_features.csv
        │   ├── Day4
        │   │   └── comb_features.csv
        │   └── Day5
        │       └── comb_features.csv
        ├── Client5 (benign)
        │   ├── Day1
        │   │   └── comb_features.csv
        │   ├── Day2
        │   │   └── comb_features.csv
        │   ├── Day3
        │   │   └── comb_features.csv
        │   ├── Day4
        │   │   └── comb_features.csv
        │   └── Day5
        │       └── comb_features.csv
        ├── Client6 (benign)
        │   ├── Day1
        │   │   └── comb_features.csv
        │   ├── Day2
        │   │   └── comb_features.csv
        │   ├── Day3
        │   │   └── comb_features.csv
        │   ├── Day4
        │   │   └── comb_features.csv
        │   └── Day5
        │       └── comb_features.csv
        ├── Client7 (benign)
        │   ├── Day1
        │   │   └── comb_features.csv
        │   ├── Day2
        │   │   └── comb_features.csv
        │   ├── Day3
        │   │   └── comb_features.csv
        │   ├── Day4
        │   │   └── comb_features.csv
        │   └── Day5
        │       └── comb_features.csv
        ├── Client8 (benign)
        │   ├── Day1
        │   │   └── comb_features.csv
        │   ├── Day2
        │   │   └── comb_features.csv
        │   ├── Day3
        │   │   └── comb_features.csv
        │   ├── Day4
        │   │   └── comb_features.csv
        │   └── Day5
        │       └── comb_features.csv
        ├── Client9 (benign)
        │   ├── Day1
        │   │   └── comb_features.csv
        │   ├── Day2
        │   │   └── comb_features.csv
        │   ├── Day3
        │   │   └── comb_features.csv
        │   ├── Day4
        │   │   └── comb_features.csv
        │   └── Day5
        │       └── comb_features.csv
        └── Malware
            ├── CTU-Malware-Capture-Botnet-219-2
            │   ├── Day1
            │   │   └── comb_features.csv
            │   ├── Day2
            │   ├── Day3
            │   ├── Day4
            │   └── Day5
            ├── CTU-Malware-Capture-Botnet-230-1
            │   ├── Day1
            │   │   └── comb_features.csv
            │   ├── Day2
            │   ├── Day3
            │   ├── Day4
            │   └── Day5
            ├── CTU-Malware-Capture-Botnet-246-1
            │   ├── Day1
            │   │   └── comb_features.csv
            │   ├── Day2
            │   │   └── comb_features.csv
            │   ├── Day3
            │   │   └── comb_features.csv
            │   ├── Day4
            │   │   └── comb_features.csv
            │   └── Day5
            │       └── comb_features.csv
            ├── CTU-Malware-Capture-Botnet-327-2
            │   ├── Day1
            │   │   └── comb_features.csv
            │   ├── Day2
            │   │   └── comb_features.csv
            │   ├── Day3
            │   │   └── comb_features.csv
            │   ├── Day4
            │   │   └── comb_features.csv
            │   └── Day5
            │       └── comb_features.csv
            ├── CTU-Malware-Capture-Botnet-346-1
            │   ├── Day1
            │   │   └── comb_features.csv
            │   ├── Day2
            │   │   └── comb_features.csv
            │   ├── Day3
            │   │   └── comb_features.csv
            │   ├── Day4
            │   │   └── comb_features.csv
            │   └── Day5
            │       └── comb_features.csv
            └── CTU-Malware-Capture-Botnet-67-1
                ├── Day1
                │   └── comb_features.csv
                ├── Day2
                │   └── comb_features.csv
                ├── Day3
                │   └── comb_features.csv
                ├── Day4
                │   └── comb_features.csv
                └── Day5
                    └── comb_features.csv

If some day does not have a CSV file is because there was not malware during that day.

## Explanation of which malware and users are in the dataset
![Explanation of ctu-50-dataset](ctu-50-features/ctu-50-features.png)


## Explanation of the data

Each row/sample in the `comb_fatures.csv` files is an aggregation of many TLS flows. The idea is to put together the flow that go to the same service so to model the behavior of the user/malware respect to the same service (for example https://mail.google.com).

The aggregation works as follows:
1. Take all the TLS flows that *share* the same **source IP**, **destination IP**, **destination port**, and **protocol**.
2. Compute some features on these aggregated flows, such as for example the amount of flows.

The complete list of features was originally created by František Střasák [here](https://dspace.cvut.cz/bitstream/handle/10467/68528/F3-BP-2017-Strasak-Frantisek-strasak_thesis_2017.pdf) and adapted by Pavel Janata [here]().

