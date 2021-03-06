# ERA8-Mapping

**Title**: Exome sequencing of bulked segregants identified a novel *TaMKK3-A* allele linked to the wheat *ERA8* ABA-hypersensitive germination phenotype  
**Authors**: Shantel A. Martinez, Oluwayesi Shorinola, Samantha Conselman, Deven See, Daniel Z. Skinner, Cristobal Uauy, and Camille M. Steber  

This repository contains all datasets for the paper, Martinez et al. 2019, and can be used to enable reproducibility of the QTL Mapping and figures created.  
> PLEASE REFER TO THE MATERIALS AND METHODS SECTION FOR REFERENCE  

## Exome Capture  
Post-alignment SNP calls are available upon request.   

## GBS Analysis 
[README and scripts](https://github.com/shantel-martinez/ERA8-Mapping/tree/master/GBS) are available used for alignment and SNP calls in the Louise/ZakERA8 RIL population.  
Data wrangling from raw .csv files to JoinMap format was conducted in excel.   
All SNPs were included in the JoinMap linkage grouping. Raw data prior to linkage grouping is available upon request.    
The final genetic map, GBS genotypes, and dormancy phenotypes of the Louise/ZakERA8 RIL population is available in the [/data/LZ8_SNP1-SNP30_MKK3.csv](https://github.com/shantel-martinez/ERA8-Mapping/blob/master/data/LZ8_GBS_all.csv) file and also in Martinez et al. (2019) SUPPLEMENTAL TABLE 3.   

## QTL Analysis
View the R code, analysis, and figure creation in the [QTL_Mapping_of_ERA8](http://rpubs.com/shantel-martinez/ERA8-Mapping) website.  

### File Descriptions   
Multiple files are included in the data analysis.   


| name       | file_name                        | description                                                  |
| ---------- | -------------------------------- | ------------------------------------------------------------ |
| ZZ8        | ZZ8_SNP1-SNP_30_all.csv          | Fine Mapping Zak/ZaERA8 population                           |
| data5.1    | ZZ8_SNP1-SNP_30_5.1.csv          | Fine Mapping Zak/ZaERA8 population subset of cross 5.1       |
| data5.2a   | ZZ8_SNP1-SNP_30_5.2a.csv         | Fine Mapping Zak/ZaERA8 population subset of cross 5.2a      |
| data5.2b   | ZZ8_SNP1-SNP_30_5.2b.csv         | Fine Mapping Zak/ZaERA8 population subset of cross 5.2b      |
| LZ8        | LZ8_SNP1-SNP30_MKK3.csv          | Fine Mapping Louise/ZaERA8 population                        |
| LZ8GBS     | LZ8_GBS_all.csv                  | Whole genome QTL Mapping of Louise/ZaERA8 population         |
| OZ8        | OZ8_SNP6-SNP29.csv               | Fine Mapping Otis/ZaERA8 population                          |
| uniqpos    | GBS_UniquePos.txt                | Unique variables of positions or graphing ABA trait          |
| uniqposAHH | GBS_UniquePos_ABAHeadHei.txt     | Unique variables of positions or graphing ABA, height, heading traits |
| ATol       | AllTolQTLAlleles.txt             | defined tolerant alleles in the Louise/ZakERA8  population   |
| ParABA     | LZ8ARTC_2014.csv                 | Louise and ERA8 parental after-ripening time course          |
| ZParABA    | ZZ8ARTC_E1.csv                   | Zak and ERA8 parental after-ripening time course             |
| imap       | ZZ8 5.1 5.2 Group Data for R.csv | interval map of the Zak/ZakERA8 population                   |

| name       | file_name                        | obs   | variables | line_no | marker_no | chr  | phenotypes                             |
| ---------- | -------------------------------- | ----- | --------- | ------- | --------- | ---- | -------------------------------------- |
| ZZ8        | ZZ8_SNP1-SNP_30_all.csv          | -     | -         | 424     | 11        | 4A   | GI, PG                                 |
| data5.1    | ZZ8_SNP1-SNP_30_5.1.csv          | -     | -         | 122     | 11        | 4A   | GI, PG                                 |
| data5.2a   | ZZ8_SNP1-SNP_30_5.2a.csv         | -     | -         | 242     | 11        | 4A   | GI, PG                                 |
| data5.2b   | ZZ8_SNP1-SNP_30_5.2b.csv         | -     | -         | 60      | 11        | 4A   | GI, PG                                 |
| LZ8        | LZ8_SNP1-SNP30_MKK3.csv          | -     | -         | 207     | 13        | 4A   | E1-E3:D1-D5, E1-E3:GI, Height, Heading |
| LZ8GBS     | LZ8_GBS_all.csv                  | -     | -         | 209     | 2234      | ALL  | E1-E3:D1-D5, E1-E3:GI, Height, Heading |
| OZ8        | OZ8_SNP6-SNP29.csv               | -     | -         | 108     | 4         | 4A   | PG_d1-d5, GI                           |
| uniqpos    | GBS_UniquePos.txt                | 38520 | 6         | -       | -         | ALL  | -                                      |
| uniqposAHH | GBS_UniquePos_ABAHeadHei.txt     | 42800 | 6         | -       | -         | ALL  | -                                      |
| ATol       | AllTolQTLAlleles.txt             | 207   | 33        | -       | -         | -    | -                                      |
| ParABA     | LZ8ARTC_2014.csv                 | 78    | 9         | -       | -         | -    | -                                      |
| ZParABA    | ZZ8ARTC_E1.csv                   | 55    | 8         | -       | -         | -    | -                                      |
| imap       | ZZ8 5.1 5.2 Group Data for R.csv | 128   | 28        | -       | -         | 4A   | -                                      |


### Reproducing the QTL Analysis
Linked in the [QTL_Mapping_of_ERA8](http://rpubs.com/shantel-martinez/ERA8-Mapping) website under the header `Load All Data`, you can download all of the data files (listed above) as an `ERA8-Mapping-Data.RData` file for this analysis.   

Run 
```
load("PATH/ERA8-Mapping-Data.RData")
```
in your R workspace with the correct PATH directory to the downloaded file.  


