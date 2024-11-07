1. List All Films:

```Query
{
  allFilms {
    films {
      title
    }
  }
}
```

```Response
{
  "data": {
    "allFilms": {
      "films": [
        {
          "title": "A New Hope"
        },
        {
          "title": "The Empire Strikes Back"
        },
        {
          "title": "Return of the Jedi"
        },
        {
          "title": "The Phantom Menace"
        },
        {
          "title": "Attack of the Clones"
        },
        {
          "title": "Revenge of the Sith"
        }
      ]
    }
  }
}
```

2.Fetch a Specific Character:`

```Query
{
  person(id: "cGVvcGxlOjEz"){
    name
  }
}
```

```Response
{
  "data": {
    "person": {
      "name": "Chewbacca"
    }
  }
}
```

3.Explore Planets:

```Query
{
  allPlanets(first: 5) {
    planets {
      name
    }
  }
}
```

```Response
{
  "data": {
    "allPlanets": {
      "planets": [
        {
          "name": "Tatooine"
        },
        {
          "name": "Alderaan"
        },
        {
          "name": "Yavin IV"
        },
        {
          "name": "Hoth"
        },
        {
          "name": "Dagobah"
        }
      ]
    }
  }
}
```

4.Starships Information:

```Query
{
  allStarships(first: 3) {
    starships {
      name
      model
    }
  }
}
```

```Response
{
  "data": {
    "allStarships": {
      "starships": [
        {
          "name": "CR90 corvette",
          "model": "CR90 corvette"
        },
        {
          "name": "Star Destroyer",
          "model": "Imperial I-class Star Destroyer"
        },
        {
          "name": "Sentinel-class landing craft",
          "model": "Sentinel-class landing craft"
        }
      ]
    }
  }
}
```

5.Character and Their Starships:

```Query
{
  allPeople(first: 5) {
    people {
      name
      starshipConnection {
        starships {
          name
        }
      }
    }
  }
}
```

```Response
{
  "data": {
    "allPeople": {
      "people": [
        {
          "name": "Luke Skywalker",
          "starshipConnection": {
            "starships": [
              {
                "name": "X-wing"
              },
              {
                "name": "Imperial shuttle"
              }
            ]
          }
        },
        {
          "name": "C-3PO",
          "starshipConnection": {
            "starships": []
          }
        },
        {
          "name": "R2-D2",
          "starshipConnection": {
            "starships": []
          }
        },
        {
          "name": "Darth Vader",
          "starshipConnection": {
            "starships": [
              {
                "name": "TIE Advanced x1"
              }
            ]
          }
        },
        {
          "name": "Leia Organa",
          "starshipConnection": {
            "starships": []
          }
        }
      ]
    }
  }
}
```

6.Species and Their Languages:

```Query
{
  allSpecies(first: 5) {
    species {
      name
      language
    }
  }
}
```

```Response
{
  "data": {
    "allSpecies": {
      "species": [
        {
          "name": "Human",
          "language": "Galactic Basic"
        },
        {
          "name": "Droid",
          "language": "n/a"
        },
        {
          "name": "Wookie",
          "language": "Shyriiwook"
        },
        {
          "name": "Rodian",
          "language": "Galatic Basic"
        },
        {
          "name": "Hutt",
          "language": "Huttese"
        }
      ]
    }
  }
}
```

7.Planets and Their Climates:

```Query
{
  allPlanets(first:5) {
    planets {
      name
      climates
    }
  }
}
```

```Response
{
  "data": {
    "allPlanets": {
      "planets": [
        {
          "name": "Tatooine",
          "climates": [
            "arid"
          ]
        },
        {
          "name": "Alderaan",
          "climates": [
            "temperate"
          ]
        },
        {
          "name": "Yavin IV",
          "climates": [
            "temperate",
            "tropical"
          ]
        },
        {
          "name": "Hoth",
          "climates": [
            "frozen"
          ]
        },
        {
          "name": "Dagobah",
          "climates": [
            "murky"
          ]
        }
      ]
    }
  }
}
```

8.Vehicles and Their Costs:

```Query
{
  allVehicles(first: 3) {
    vehicles {
      name
      costInCredits
    }
  }
}
```

```Response
{
  "data": {
    "allVehicles": {
      "vehicles": [
        {
          "name": "Sand Crawler",
          "costInCredits": 150000
        },
        {
          "name": "T-16 skyhopper",
          "costInCredits": 14500
        },
        {
          "name": "X-34 landspeeder",
          "costInCredits": 10550
        }
      ]
    }
  }
}
```
