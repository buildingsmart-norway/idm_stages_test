# Testprosjekt for maskinlesbar publikasjon av fasebetegnelser


Fasedefinisjonene er hentet fra [definisjonene gitt av arbeidet med bSN Guiden](https://github.com/buildingsmart-norway/bsn-guiden/tree/master/definisjoner), som er basert på IDM standarden ISO 29481-1:2010 Building information modelling.

Målet med denne testen er å lage maskinlesbar ontologi av fasebetegnelsen fra bSN Guiden, samt lage linkset av mappingene som er definert i [bSNG Faser FN POW](definitions/bsng_faser_fn_pow.xlsx).

## EUROTL Modelling and Linking

Prosjektet EUROTL utviklet en kjerneontologi, og et sett linker til andre ontologier, for å kunne integrere og skape interoperabilitet mellom de europeiske objekttype katalogene (slik som norske NVDB) mulig. Les mer om [EUROTL ontologiene her](https://www.roadotl.eu/static/eurotl-ontologies/index.html).

En av konseptene i kjerneontologien er [LifecyclePhase](https://eurotl.laces-viewer.tech/#/view?uri=http%3A%2F%2Fwww.roadotl.eu%2Fdef%2FLifecyclePhase). 

I dette prosjektet skal vi lage ontologi av fase definisjonene som er buildingSMART nettverket har blitt enige om, og tildigere utgitt som excell fil på nett (se [definitions mappen](/definitions). Her defineres fasebetegnelsene og koblingen (linkene) til neste steg og RiBA Plan of Works. 

## Resultater fra testen 

Resultatet fra testen er fire filer [her](filer): 

1. Fasebetegnelsene fra bSN Guiden, basert på Information Delivery Methodology (idm) standarden (ISO 29481-1:2010), som er kalt for ```idm_stages.ttl```
2. Fasebetegnelsene fra Neste Steg (fasenormen), som er kalt ```neste_steg.ttl```
3. Fasebetegnelsene fra RIBA Plan of work, som er kalt ```plan_of_work```
4. Siste filen er inneholder koblingene (linkene) mellom bSN Guiden fasebetegnelsene med Neste Steg og Plan of Work, iht. definisjonene fra buildingSMART nettverket, og kalles ```idm_stages_alignment.ttl```

## Bidra og/eller kommetere
Alle oppfordres til å bidra og/eller kommentere gjennom å engasjere seg i buildingSMART Norge, og/eller lage en "issue" i dette repositoriet på github. Man kan også bidra ved å clone innholdet og gjøre endringer og sende inn en "pull" forespørsel. 

Filene kan vises og endres i f.eks. [Protegé som er nedlastbar her](https://protege.stanford.edu/)

## How to use the code in the Repository

This project uses python 3 and jupyter notebooks. For accessing bSDD the request library is used, and for working with the ontology the RDFLib library is used.

The [environment.yml](environment.yml). Install anaconda on your machine [create environment from this file](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file). After you can activate it by source activate {name of environment} and start the notebooks by ```jupyter notebook``` in the repo root.

## How to contribute
Please add an issue with ideas or comments, and feel free to add pull requests with alterations. 
