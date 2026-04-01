# shirp_expedition
shirp_expedition


A repo for Shinnecock Bay Restoration Program (ShiRP) 2025 autonomous eDNA expedition and manuscript.

--



Reference databases generated with [RCrux](https://github.com/CalCOFI/rCRUX) 

- [Elas02 databaselink](https://zenodo.org/records/18626068)
- [MiFish databaselink](https://zenodo.org/records/19238536)

CO1 database from [MIDORI2](https://www.reference-midori.info/)

--

Bioinformatics pipeline based on [REVAMP](https://github.com/McAllister-NOAA/REVAMP)

Specification are in config files. To run:

MiFish:

```
revamp.sh -p 01_config_file_MIFish-2024-expedition.txt -f 02_figure_config_file_MiFish-2024-expedition.txt -s 03_sample_metadata_MiFIsh-2024-expedition.txt -r raw_data/2024-MiFish-U-expedition -o results-revamp-2024-MiFish-expedition
```

Elas02:

```
revamp.sh -p 01_config_file_Elas02-2024-expedition.txt -f 02_figure_config_file_Elas02-2024-expedition.txt -s 03_sample_metadata_Elas02-2024-expedition.txt -r raw_data/2024-Elas02-expedition -o results-revamp-2024-Elas02-expedition
```

CO1:

```
revamp.sh -p 01_config_file_CO1_2024-expedition.txt -f 02_figure_config_file_CO1_2024-expedition.txt -s 03_sample_metadata_CO1_2024-expedition.txt  -r raw_data/2024-CO1-all -o results-revamp-2024-CO1
```

--

Notebook to generate maps and plot the CTD output:
`Expedition-CTD-plots.Rmd`

Notebook to filter and quality control REVAMP output:
`Expedition-eDNA-QC-filtering.Rmd`

Notebook to generate plots for manuscript:
