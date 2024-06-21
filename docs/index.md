# Wines API

This API powers the https://github.dev/react-bootcamp reboot for 2024. 

This API is used to manage a toy wines app. You can use it to retrieve wine regions, wines by regions, comments and likes on individual wines. 

<div style="width: 100%; display: flex; justify-content: center; align-items: center;">
  <img src="/docs/winesapp.png" alt="The wine app" width="300" height="auto" class="centered-img">
</div>


This API is open to everyone and is available on [https://${environment.HOST}/api](https://${environment.HOST}/api)

## Fetch all wine regions

If you want to try the API, you can retrieve all wines regions just like that:

```sh
curl -X GET https://${environment.HOST}/api/regions | jq

[
  "Bordeaux",
  "Bourgogne",
  "Champagne",
  "Languedoc",
  "Loire",
  "Normandie"
]
```

## Fetch wines from a region

then you can get all the wines from a specific region like :

```sh
curl -X GET https://${environment.HOST}/api/wines?region=Bordeaux | jq

[
  {
    "id": "chevrol-bel-air",
    "name": "Château Chevrol Bel Air",
    "type": "Rouge",
    "appellation": {
      "name": "Lalande-de-Pomerol",
      "region": "Bordeaux"
    },
    "grapes": [
      "Cabernet Sauvignon",
      "Merlot",
      "Cabernet Franc"
    ]
  },
  ...
]
```