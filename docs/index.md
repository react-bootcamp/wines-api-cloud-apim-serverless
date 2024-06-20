# Wines API

This API powers the https://github.dev/react-bootcamp reboot for 2024. 

This API is open to everyone and is available one ${environment.HOST}

If you want to try the API, you can retrieve all wines regions just like that:

```sh
curl -X GET ${environment.HOST}/api/regions | jq

[
  "Bordeaux",
  "Bourgogne",
  "Champagne",
  "Languedoc",
  "Loire",
  "Normandie"
]
```

then you can get all the wines from a specific region like :

```sh
curl -X GET ${environment.HOST}/api/wines?region=Bordeaux | jq

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