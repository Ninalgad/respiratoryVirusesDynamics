Analysis of respiratory virus infections in Canada using `SAS` and `saspy`.

# Included Viruses
- `ADENO`: [Adenoviruses](https://www.cdc.gov/adenovirus/index.html)
- `CORON`: [Human Coronaviruses](https://www.cdc.gov/coronavirus/general-information.html)
- `ENTERORHINO`: [Entero Rhinovirus](https://www.cdc.gov/ncird/rhinoviruses-common-cold.html)
- `HMPV`: [Human Metapneumovirus](https://www.cdc.gov/ncird/human-metapneumovirus.html)
- `INFA`: [Influenza A](https://www.cdc.gov/flu/about/viruses/types.htm)
- `INFB`: [Influenza B](https://www.cdc.gov/flu/about/viruses/types.htm)
- `RSV`: [Respiratory Syncitial Virus](https://www.cdc.gov/rsv/index.html)
- `PIV`: [Parainfluenzavirus](https://www.cdc.gov/parainfluenza/index.html)

# Snippet
```sas
TITLE 'Viral Incidence Rates Over Time';
PROC SGPLOT DATA=work.mydata;
    SERIES x=date y=Incidence_pop / GROUP=Virus;
RUN; 
```
![](plot.png)

# Data Citation
Varela-Lasheras I, Perfeito L, Mesquita S, Gonc¸alves-Sa´ J (2023) The effects of weather and mobility on respiratory viruses dynamics before and during the COVID-19 pandemic in the USA and Canada. PLOS Digit Health 2(12): e0000405. https://doi.org/10.1371/journal.pdig.0000405