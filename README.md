# Robert-Koch Institut API (Data & Images)

With this JSON API you can get the data of corona cases for every state and every district in Germany.
You have also access to the latest images of maps.

Data Sources:

https://npgeo-corona-npgeo-de.hub.arcgis.com/datasets/917fc37a709542548cc3be077a786c17_0?geometry=-21.159%2C46.211%2C43.177%2C55.839

https://npgeo-corona-npgeo-de.hub.arcgis.com/datasets/ef4b445a53c1406892257fe63129a8ea_0?geometry=-24.040%2C46.270%2C40.296%2C55.886

## Endpoints

### `https://rki-covid-api.now.sh/api/states`

#### Data Structure

```json
{
  "lastUpdate": 1603317600000,
  "states": [
    {
      "name": "Baden-Württemberg",
      "count": 58653,
      "weekIncidence": 42,
      "casesPer100k": 343.099136209832,
      "deaths": 1927,
      "code": "BW"
    },
    {
      "name": "Bayern",
      "count": 77904,
      "weekIncidence": 39,
      "casesPer100k": 123.099136209832,
      "deaths": 2714,
      "code": "BY"
    },
    ...
    {
      "name": "Schleswig-Holstein",
      "count": 5600,
      "weekIncidence": 13,
      "casesPer100k": 121.099136209832,
      "deaths": 163,
      "code": "SH"
    },
    {
      "name": "Thüringen",
      "count": 4793,
      "weekIncidence": 18,
      "casesPer100k": 324.099136209832,
      "deaths": 198,
      "code": "TH"
    }
  ]
}
```

### `https://rki-covid-api.now.sh/api/states-map`

You receive a PNG image:

<img src="media/states-map.png" alt="states-map" width="300"/>

### `https://rki-covid-api.now.sh/api/districts`

#### Data Structure

```json
{
  "lastUpdate": "26.10.2020, 00:00 Uhr",
  "districts": [
    {
      "name": "Flensburg",
      "count": 182,
      "deaths": 3,
      "weekIncidence": 34.3817931768777,
      "casesPer100k": 201.854398651346,
      "casesPerPopulation": 0.201854398651346
    },
    {
      "name": "Kiel",
      "count": 582,
      "deaths": 12,
      "weekIncidence": 27.5533440845401,
      "casesPer100k": 235.824209664741,
      "casesPerPopulation": 0.235824209664741
    },
    ...
    {
      "name": "Berlin Friedrichshain-Kreuzberg",
      "count": 2622,
      "deaths": 11,
      "weekIncidence": 172.304376034801,
      "casesPer100k": 929.592744780347,
      "casesPerPopulation": 0.929592744780347
    },
    {
      "name": "Berlin Tempelhof-Schöneberg",
      "count": 2760,
      "deaths": 28,
      "weekIncidence": 164.729702842831,
      "casesPer100k": 807.555914469295,
      "casesPerPopulation": 0.807555914469295
    }
  ]
}
```

### `https://rki-covid-api.now.sh/api/districts-map`

You receive a PNG image:

<img src="media/districts-map.png" alt="districts-map" width="300"/>


## Project Showcase (project using this API)

[Add your project by openening an issue with your project details!](https://github.com/marlon360/rki-covid-api/issues/new)

- https://coronafallzahlen.de



## Donation

[Buy me a coffee](https://ko-fi.com/marlon360)
