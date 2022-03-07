# Andre bibliotek

Her er ein guide til korleis du kan installera andre bibliotek (som ikkje ligg i Anaconda-pakken). 

:::{admonition} Pass på!
:class: warning
Ikkje gjer dette om du ikkje har fått beskjed av lærar. Det er kun aktuelt i nokre få fag. 
:::

# Geopandas

**Dokumentasjon:** https://geopandas.org/en/stable/

For å kunna plotta geografiske data i feks. Geofag er bilioteket `GeoPandas` nyttig. Det er eit biliotek som lar oss jobba med datarammer på samme måte som `Pandas` men i tillegg så har det ulike funksjonar for å mogleggjera plotting på kart osv. 

Når me skal installera `GeoPandas` er det beste å laga eit nytt _enviroment_ (miljø på norsk). Dette for å unngå konfliktar mellom dette biblioteket og dei andre biblioteka som ligg inne i Anacondapakken som standard. Me kallar det nye miljøet for `geo_env` for å enkelt forstå seinare at dette handla om geografisk/geofaglege verktøy. 

Installasjon er enklast gjennom terminalen (sjå [](../installasjon.ipynb) for korleis du finn denne). 

```bash
conda create -n geo_env
conda activate geo_env
conda config --env --add channels conda-forge
conda config --env --set channel_priority strict
conda install python=3 geopandas
```

:::{admonition} Viktig
:class: important

Når du skal _bruka_ `GeoPandas` må du bytta til det nye miljøet, `geo_env`.
:::

```{image} img/byttemiljø.gif
:width: 500px
:align: center
```

# Seaborn

**Dokumentasjon:** https://seaborn.pydata.org/

Meir her.