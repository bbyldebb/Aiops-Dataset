# README

### Overview

This Aiops-Dataset is collected from a simulated e-commerce system based on a microservice architecture. The system under study is deployed on a real cloud environment, and its traffic is consistent with the real business traffic. The system comprises 46 system instances, including 40 microservice instances and 6 virtual machines. Each microservice has its corresponding container monitor, and the deployed virtual machines have associated monitoring data. The failure scenarios in this dataset are derived from real system failures and are replayed in batches. To collect the failure records, operators conducted a failure replay in the system for several days in May 2022. The recorded failures were then labeled with their respective real root cause instances.

### Dataset Link
https://mega.nz/file/7UMCWDrD#v-2OJvvTIz4uDL9Qn3Inc_VLNQY-wgdvihVaPdzmD0Q


### Directory Structrue

```
├── Aiops-Dataset/
│   ├── data/
│      ├── 2022-05-01/
│            ├── log/
│            ├── metric/
│            ├── trace/
│      ├── 2022-05-03/
│            ├── ...
│      ├── 2022-05-05/
│            ├── ...
│      ├── 2022-05-07/
│            ├── ...
│      ├── 2022-05-09/
│            ├── ...
│   ├── groundtruth
│      ├── groundtruth-2022-05-01.csv
│      ├── groundtruth-2022-05-03.csv
│      ├── groundtruth-2022-05-05.csv
│      ├── groundtruth-2022-05-07.csv
│      ├── groundtruth-2022-05-09.csv
│      ├── groundtruth-all.csv
└── README.md
```

### Directory Descriptions

- **data/**: This directory contains all the data files, organized in a time-based manner. It provides three types of data for analysis: logs, metrics, and traces.
- **data/**: This directory contains fault injection records, including the time of injection, severity, root cause, and fault category.