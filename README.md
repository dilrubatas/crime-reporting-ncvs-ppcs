# Crime Reporting to Police: NCVS and PPCS Analysis

Analysis of why crime victims do or don't report to police, using the National Crime Victimization Survey (NCVS, 2020–2023), and whether past police violations relate to willingness to contact police, using the Police-Public Contact Survey (PPCS, 2020 and 2022).

All code is in `Crime_reporting_data_analysis.Rmd`. Knitting it produces the HTML report and the figures (`*.png`).

## Data

The raw data are not included in this repository. ICPSR's Terms of Use do not allow redistribution. Download the TSV versions from ICPSR (free account required) and unzip each study into this folder, keeping ICPSR's folder names:

| Study | ICPSR | Files used |
|---|---|---|
| NCVS 2020 | [38090](https://www.icpsr.umich.edu/web/NACJD/studies/38090) | `ICPSR_38090/DS0005/38090-0005-Data.tsv` |
| NCVS 2021 | [38429](https://www.icpsr.umich.edu/web/NACJD/studies/38429) | `ICPSR_38429/DS0005/38429-0005-Data.tsv` |
| NCVS 2022 | [38603](https://www.icpsr.umich.edu/web/NACJD/studies/38603) | `ICPSR_38603/DS0005/38603-0005-Data.tsv` |
| NCVS 2023 | [38962](https://www.icpsr.umich.edu/web/NACJD/studies/38962) | `ICPSR_38962/DS0005/38962-0005-Data.tsv` |
| PPCS 2020 | [38320](https://www.icpsr.umich.edu/web/NACJD/studies/38320) | `ICPSR_38320/DS0001/38320-0001-Data.tsv` |
| PPCS 2022 | [38872](https://www.icpsr.umich.edu/web/NACJD/studies/38872) | `ICPSR_38872/DS0001/38872-0001-Data.tsv` |

## Running

Requires R (tested with 4.5.1) and the packages `tidyverse`, `patchwork`, `survey`, `marginaleffects`, `modelsummary`, `knitr`, and `rmarkdown`.

```r
rmarkdown::render("Crime_reporting_data_analysis.Rmd")
```
