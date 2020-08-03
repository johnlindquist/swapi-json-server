## Endpoint documentation

All endpoints will be documented here. All endpoints will respond with a status code of 200 on a successful request unless otherwise indicated. Likewise, all requests will respond with a 400 indicating a bad request unless otherwise indicated. Lastly, a 500 status code will be used when there is an internal server fault.

For pagination and filtering refer to these docs. [https://www.npmjs.com/package/json-server](https://www.npmjs.com/package/json-server)

## Table of Contents

- [Films](#films)
- [People](#people)
- [Planets](#planets)
- [Species](#species)
- [Starships](#starships)
- [Transport](#transport)
- [Vehicles](#vehicles)
- [Meta](#meta)

### Films

Base URL: `/films`

Success Response

```json
[
  {
    "starships": [2, 3, 5, 9, 10, 11, 12, 13],
    "edited": "2014-12-20T19:49:45.256Z",
    "vehicles": [4, 6, 7, 8],
    "planets": [1, 2, 3],
    "producer": "Gary Kurtz, Rick McCallum",
    "title": "A New Hope",
    "created": "2014-12-10T14:23:31.880Z",
    "episode_id": 4,
    "director": "George Lucas",
    "release_date": "1977-05-25",
    "opening_crawl": "It is a period of civil war.\r\nRebel spaceships, striking\r\nfrom a hidden base, have won\r\ntheir first victory against\r\nthe evil Galactic Empire.\r\n\r\nDuring the battle, Rebel\r\nspies managed to steal secret\r\nplans to the Empire's\r\nultimate weapon, the DEATH\r\nSTAR, an armored space\r\nstation with enough power\r\nto destroy an entire planet.\r\n\r\nPursued by the Empire's\r\nsinister agents, Princess\r\nLeia races home aboard her\r\nstarship, custodian of the\r\nstolen plans that can save her\r\npeople and restore\r\nfreedom to the galaxy....",
    "characters": [
      1,
      2,
      3,
      4,
      5,
      6,
      7,
      8,
      9,
      10,
      12,
      13,
      14,
      15,
      16,
      18,
      19,
      81
    ],
    "species": [1, 2, 3, 4, 5],
    "id": 1
  },
  ...
]
```

#### Get film by Id

URL: `/films/:id`

Success Response

```json
{
  "starships": [2, 3, 5, 9, 10, 11, 12, 13],
  "edited": "2014-12-20T19:49:45.256Z",
  "vehicles": [4, 6, 7, 8],
  "planets": [1, 2, 3],
  "producer": "Gary Kurtz, Rick McCallum",
  "title": "A New Hope",
  "created": "2014-12-10T14:23:31.880Z",
  "episode_id": 4,
  "director": "George Lucas",
  "release_date": "1977-05-25",
  "opening_crawl": "It is a period of civil war.\r\nRebel spaceships, striking\r\nfrom a hidden base, have won\r\ntheir first victory against\r\nthe evil Galactic Empire.\r\n\r\nDuring the battle, Rebel\r\nspies managed to steal secret\r\nplans to the Empire's\r\nultimate weapon, the DEATH\r\nSTAR, an armored space\r\nstation with enough power\r\nto destroy an entire planet.\r\n\r\nPursued by the Empire's\r\nsinister agents, Princess\r\nLeia races home aboard her\r\nstarship, custodian of the\r\nstolen plans that can save her\r\npeople and restore\r\nfreedom to the galaxy....",
  "characters": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 12, 13, 14, 15, 16, 18, 19, 81],
  "species": [1, 2, 3, 4, 5],
  "id": 1
}
```

### People

Base URL: `/people`

Success Response

```json
[
  {
    "edited": "2014-12-20T21:17:56.891Z",
    "name": "Luke Skywalker",
    "created": "2014-12-09T13:50:51.644Z",
    "gender": "male",
    "skin_color": "fair",
    "hair_color": "blond",
    "height": "172",
    "eye_color": "blue",
    "mass": "77",
    "homeworld": 1,
    "birth_year": "19BBY",
    "image": "luke_skywalker.jpg",
    "id": 1,
    "vehicles": [
      14,
      30
    ],
    "starships": [
      12,
      22
    ],
    "films": [
      1,
      2,
      3,
      6
    ]
  },
  {
    "edited": "2014-12-20T21:17:50.309Z",
    "name": "C-3PO",
    "created": "2014-12-10T15:10:51.357Z",
    "gender": "n/a",
    "skin_color": "gold",
    "hair_color": "n/a",
    "height": "167",
    "eye_color": "yellow",
    "mass": "75",
    "homeworld": 1,
    "birth_year": "112BBY",
    "image": "c-3po.jpg",
    "id": 2,
    "vehicles": [],
    "starships": [],
    "films": [
      1,
      2,
      3,
      4,
      5,
      6
    ]
  },
  ...
]
```

#### Get person by Id

URL: `/people/:id`

Success Response

```json
{
  "edited": "2014-12-20T21:17:56.891Z",
  "name": "Luke Skywalker",
  "created": "2014-12-09T13:50:51.644Z",
  "gender": "male",
  "skin_color": "fair",
  "hair_color": "blond",
  "height": "172",
  "eye_color": "blue",
  "mass": "77",
  "homeworld": 1,
  "birth_year": "19BBY",
  "image": "luke_skywalker.jpg",
  "id": 1,
  "vehicles": [14, 30],
  "starships": [12, 22],
  "films": [1, 2, 3, 6]
}
```

### Planets

Base URL: `/planets`

Success Response

```json
[
  {
    "edited": "2014-12-20T20:58:18.411Z",
    "climate": "arid",
    "surface_water": "1",
    "name": "Tatooine",
    "diameter": "10465",
    "rotation_period": "23",
    "created": "2014-12-09T13:50:49.641Z",
    "terrain": "desert",
    "gravity": "1 standard",
    "orbital_period": "304",
    "population": "200000",
    "id": 1,
    "residents": [
      1,
      2,
      4,
      6,
      7,
      8,
      9,
      11,
      43,
      62
    ],
    "films": [
      1,
      3,
      4,
      5,
      6
    ]
  },
  {
    "edited": "2014-12-20T20:58:18.420Z",
    "climate": "temperate",
    "surface_water": "40",
    "name": "Alderaan",
    "diameter": "12500",
    "rotation_period": "24",
    "created": "2014-12-10T11:35:48.479Z",
    "terrain": "grasslands, mountains",
    "gravity": "1 standard",
    "orbital_period": "364",
    "population": "2000000000",
    "id": 2,
    "residents": [
      5,
      68,
      81
    ],
    "films": [
      1,
      6
    ]
  },
  ...
]
```

#### Get planet by Id

URL: `/planets/:id`

Success Response

```json
{
  "edited": "2014-12-20T20:58:18.411Z",
  "climate": "arid",
  "surface_water": "1",
  "name": "Tatooine",
  "diameter": "10465",
  "rotation_period": "23",
  "created": "2014-12-09T13:50:49.641Z",
  "terrain": "desert",
  "gravity": "1 standard",
  "orbital_period": "304",
  "population": "200000",
  "id": 1,
  "residents": [1, 2, 4, 6, 7, 8, 9, 11, 43, 62],
  "films": [1, 3, 4, 5, 6]
}
```

### Species

Base URL: `/species`

Success Response

```json
[
  {
    "edited": "2014-12-20T21:36:42.136Z",
    "classification": "mammal",
    "name": "Human",
    "designation": "sentient",
    "created": "2014-12-10T13:52:11.567Z",
    "eye_colors": "brown, blue, green, hazel, grey, amber",
    "people": [
      66,
      67,
      68,
      74
    ],
    "skin_colors": "caucasian, black, asian, hispanic",
    "language": "Galactic Basic",
    "hair_colors": "blonde, brown, black, red",
    "homeworld": 9,
    "average_lifespan": "120",
    "average_height": "180",
    "id": 1
  },
  {
    "edited": "2014-12-20T21:36:42.139Z",
    "classification": "artificial",
    "name": "Droid",
    "designation": "sentient",
    "created": "2014-12-10T15:16:16.259Z",
    "eye_colors": "n/a",
    "people": [
      2,
      3,
      8,
      23
    ],
    "skin_colors": "n/a",
    "language": "n/a",
    "hair_colors": "n/a",
    "homeworld": null,
    "average_lifespan": "indefinite",
    "average_height": "n/a",
    "id": 2
  },
  ...
]
```

#### Get species by Id

URL: `/species/:id`

Success Response

```json
{
  "edited": "2014-12-20T21:36:42.136Z",
  "classification": "mammal",
  "name": "Human",
  "designation": "sentient",
  "created": "2014-12-10T13:52:11.567Z",
  "eye_colors": "brown, blue, green, hazel, grey, amber",
  "people": [66, 67, 68, 74],
  "skin_colors": "caucasian, black, asian, hispanic",
  "language": "Galactic Basic",
  "hair_colors": "blonde, brown, black, red",
  "homeworld": 9,
  "average_lifespan": "120",
  "average_height": "180",
  "id": 1
}
```

### Starships

Base URL: `/starships`

Success Response

```json
[
  {
    "pilots": [],
    "MGLT": "60",
    "starship_class": "corvette",
    "hyperdrive_rating": "2.0",
    "id": 2,
    "edited": "2014-12-20T21:23:49.867Z",
    "consumables": "1 year",
    "name": "CR90 corvette",
    "created": "2014-12-10T14:20:33.369Z",
    "cargo_capacity": "3000000",
    "passengers": "600",
    "max_atmosphering_speed": "950",
    "crew": "30-165",
    "length": "150",
    "model": "CR90 corvette",
    "cost_in_credits": "3500000",
    "manufacturer": "Corellian Engineering Corporation",
    "image": "cr90_corvette.jpg",
    "films": [
      1,
      3,
      6
    ]
  },
  {
    "pilots": [],
    "MGLT": "60",
    "starship_class": "Star Destroyer",
    "hyperdrive_rating": "2.0",
    "id": 3,
    "edited": "2014-12-20T21:23:49.870Z",
    "consumables": "2 years",
    "name": "Star Destroyer",
    "created": "2014-12-10T15:08:19.848Z",
    "cargo_capacity": "36000000",
    "passengers": "n/a",
    "max_atmosphering_speed": "975",
    "crew": "47,060",
    "length": "1,600",
    "model": "Imperial I-class Star Destroyer",
    "cost_in_credits": "150000000",
    "manufacturer": "Kuat Drive Yards",
    "image": "star_destroyer.jpg",
    "films": [
      1,
      2,
      3
    ]
  },
  ...
]
```

#### Get starship by Id

URL: `/starships/:id`

Success Response

```json
{
  "pilots": [],
  "MGLT": "60",
  "starship_class": "corvette",
  "hyperdrive_rating": "2.0",
  "id": 2,
  "edited": "2014-12-20T21:23:49.867Z",
  "consumables": "1 year",
  "name": "CR90 corvette",
  "created": "2014-12-10T14:20:33.369Z",
  "cargo_capacity": "3000000",
  "passengers": "600",
  "max_atmosphering_speed": "950",
  "crew": "30-165",
  "length": "150",
  "model": "CR90 corvette",
  "cost_in_credits": "3500000",
  "manufacturer": "Corellian Engineering Corporation",
  "image": "cr90_corvette.jpg",
  "films": [1, 3, 6]
}
```

### Transport

Base URL: `/transport`

Success Response

```json
[
  {
    "edited": "2014-12-20T21:23:49.867Z",
    "consumables": "1 year",
    "name": "CR90 corvette",
    "created": "2014-12-10T14:20:33.369Z",
    "cargo_capacity": "3000000",
    "passengers": "600",
    "max_atmosphering_speed": "950",
    "crew": "30-165",
    "length": "150",
    "model": "CR90 corvette",
    "cost_in_credits": "3500000",
    "manufacturer": "Corellian Engineering Corporation",
    "image": "cr90_corvette.jpg",
    "id": 2
  },
  {
    "edited": "2014-12-20T21:23:49.870Z",
    "consumables": "2 years",
    "name": "Star Destroyer",
    "created": "2014-12-10T15:08:19.848Z",
    "cargo_capacity": "36000000",
    "passengers": "n/a",
    "max_atmosphering_speed": "975",
    "crew": "47,060",
    "length": "1,600",
    "model": "Imperial I-class Star Destroyer",
    "cost_in_credits": "150000000",
    "manufacturer": "Kuat Drive Yards",
    "image": "star_destroyer.jpg",
    "id": 3
  },
  ...
]
```

#### Get transport by Id

URL: `/transport/:id`

Success Response

```json
{
  "edited": "2014-12-20T21:23:49.867Z",
  "consumables": "1 year",
  "name": "CR90 corvette",
  "created": "2014-12-10T14:20:33.369Z",
  "cargo_capacity": "3000000",
  "passengers": "600",
  "max_atmosphering_speed": "950",
  "crew": "30-165",
  "length": "150",
  "model": "CR90 corvette",
  "cost_in_credits": "3500000",
  "manufacturer": "Corellian Engineering Corporation",
  "image": "cr90_corvette.jpg",
  "id": 2
}
```

### Vehicles

Base URL: `/vehicles`

Success Response

```json
[
  {
    "vehicle_class": "wheeled",
    "pilots": [],
    "id": 4,
    "edited": "2014-12-20T21:30:21.661Z",
    "consumables": "2 months",
    "name": "Sand Crawler",
    "created": "2014-12-10T15:36:25.724Z",
    "cargo_capacity": "50000",
    "passengers": "30",
    "max_atmosphering_speed": "30",
    "crew": "46",
    "length": "36.8 ",
    "model": "Digger Crawler",
    "cost_in_credits": "150000",
    "manufacturer": "Corellia Mining Corporation",
    "image": "sand_crawler.jpg"
  },
  {
    "vehicle_class": "repulsorcraft",
    "pilots": [],
    "id": 6,
    "edited": "2014-12-20T21:30:21.665Z",
    "consumables": "0",
    "name": "T-16 skyhopper",
    "created": "2014-12-10T16:01:52.434Z",
    "cargo_capacity": "50",
    "passengers": "1",
    "max_atmosphering_speed": "1200",
    "crew": "1",
    "length": "10.4 ",
    "model": "T-16 skyhopper",
    "cost_in_credits": "14500",
    "manufacturer": "Incom Corporation",
    "image": "t-16_skyhopper.jpg"
  },
  ...
]
```

#### Get vehicle by Id

URL: `/vehicles/:id`

Success Response

```json
{
  "vehicle_class": "wheeled",
  "pilots": [],
  "id": 4,
  "edited": "2014-12-20T21:30:21.661Z",
  "consumables": "2 months",
  "name": "Sand Crawler",
  "created": "2014-12-10T15:36:25.724Z",
  "cargo_capacity": "50000",
  "passengers": "30",
  "max_atmosphering_speed": "30",
  "crew": "46",
  "length": "36.8 ",
  "model": "Digger Crawler",
  "cost_in_credits": "150000",
  "manufacturer": "Corellia Mining Corporation",
  "image": "sand_crawler.jpg"
}
```

### Meta

Base URL: `/meta`

#### Get server uptime

URL: `/meta/runtime`

Query Strings Accepted: `?measurement=value`

Valid measurement values accepted are shown below. If non-valid or no measurement is passed, it will default to seconds.

```
const validMeasurmements = [
    'days',
    'years',
    'months',
    'weeks',
    'days',
    'hours',
    'minutes',
    'seconds',
  ]
```

Success Response

```json
{
  "timeSinceLastReboot": "6 seconds"
}
```
