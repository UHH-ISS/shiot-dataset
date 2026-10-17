# SHIoT'26 Dataset
Dataset accompanying the paper:
> **SHIoT'26: A Specialized IoT Intrusion Detection Dataset for Smart Home Environments**  
> Tatjana Wingarz, Jeetesh Gupta, Lars Schumacher, Mathias Fischer  
> Nordsec'26 (31st Nordic Conference on Secure IT Systems), 2026

The SHIoT'26 dataset is a network attack dataset focused on smart home networks. It was generated using a realistic testbed containing 17 real IoT devices typically found in smart homes.

## Variants

**Full**: `SHIoT26_full.csv` contains the full, labeled dataset in CSV format. It contains ~3.6 million network flows with 105 features, including label classes. IP addresses have been anonymized while retaining the subnet structure via Crypto-PAn.

**Reduced**: `SHIoT26_reduced_feature_set.csv` contains a subset of 58 features, including label classes.

The exact list of columns for the full and the reduced feature set can be found in [`docs/full_features.txt`](docs/full_features.txt) and [`docs/reduced_features.txt`](docs/reduced_features.txt), respectively.

## Download

The data files are attached to the GitHub release [`v1.0.0`](https://github.com/UHH-ISS/shiot-dataset/releases/v1.0.0) and are not stored in the git history.

| Variant           | File                              | Size (zip)    | SHA-256 (zip) |
|---                |---                                |---            |---            |
| Full              | `SHIoT26_full.zip`                | ~134 MB       | `aa40ed463367b2e5c808d892095cdd0c14864b0c74235838d814a1fe50157acc` |
| Reduced features  | `SHIoT26_reduced_feature_set.zip` | ~44 MB        | `df6c3c5073d57c1ab0d0e9e04458a9598eadf1b69185b0de718cce7efdb494c8` |

The hashes above refer to the downloaded ZIP archives. Since re-packing a CSV file can produce a different archive, the hashes of the extracted CSV files are given below. They identify the content independently of how it is packed.

| Variant           | File                              | Size (csv)    | SHA-256 (csv) |
|---                |---                                |---            |---            |
| Full              | `SHIoT26_full.csv`                | ~1.5 GB       | `b6adf206094525283aabf68696b096e846ebbabcbe453395839b106e4bae75c8` |
| Reduced features  | `SHIoT26_reduced_feature_set.csv` | ~793 MB       | `8631c25e11e3ef4c00189201063f354077bbc0b6ecd228319d46a93da4d5813c` |

## Repository structure

```
.
|-- README.md
|-- LICENSE
|-- docs/
    |-- full_features.txt
    |-- reduced_features.txt
```