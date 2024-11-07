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

9.Characters in a Specific Film:

```Query
{
  film(id: "ZmlsbXM6Mw==") {
    characterConnection {
      characters {
        name
      }
    }
  }
}
```

```Response
{
  "data": {
    "film": {
      "characterConnection": {
        "characters": [
          {
            "name": "Luke Skywalker"
          },
          {
            "name": "C-3PO"
          },
          {
            "name": "R2-D2"
          },
          {
            "name": "Darth Vader"
          },
          {
            "name": "Leia Organa"
          },
          {
            "name": "Obi-Wan Kenobi"
          },
          {
            "name": "Chewbacca"
          },
          {
            "name": "Han Solo"
          },
          {
            "name": "Jabba Desilijic Tiure"
          },
          {
            "name": "Wedge Antilles"
          },
          {
            "name": "Yoda"
          },
          {
            "name": "Palpatine"
          },
          {
            "name": "Boba Fett"
          },
          {
            "name": "Lando Calrissian"
          },
          {
            "name": "Ackbar"
          },
          {
            "name": "Mon Mothma"
          },
          {
            "name": "Arvel Crynyd"
          },
          {
            "name": "Wicket Systri Warrick"
          },
          {
            "name": "Nien Nunb"
          },
          {
            "name": "Bib Fortuna"
          }
        ]
      }
    }
  }
}
```

10.Multi-Film Characters::

```Query
{
  allPeople {
    people {
      name
      filmConnection{
        totalCount
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
          "filmConnection": {
            "totalCount": 4
          }
        },
        {
          "name": "C-3PO",
          "filmConnection": {
            "totalCount": 6
          }
        },
        {
          "name": "R2-D2",
          "filmConnection": {
            "totalCount": 6
          }
        },
        {
          "name": "Darth Vader",
          "filmConnection": {
            "totalCount": 4
          }
        },
        {
          "name": "Leia Organa",
          "filmConnection": {
            "totalCount": 4
          }
        },
        {
          "name": "Owen Lars",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Beru Whitesun lars",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "R5-D4",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Biggs Darklighter",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Obi-Wan Kenobi",
          "filmConnection": {
            "totalCount": 6
          }
        },
        {
          "name": "Anakin Skywalker",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Wilhuff Tarkin",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Chewbacca",
          "filmConnection": {
            "totalCount": 4
          }
        },
        {
          "name": "Han Solo",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Greedo",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Jabba Desilijic Tiure",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Wedge Antilles",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Jek Tono Porkins",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Yoda",
          "filmConnection": {
            "totalCount": 5
          }
        },
        {
          "name": "Palpatine",
          "filmConnection": {
            "totalCount": 5
          }
        },
        {
          "name": "Boba Fett",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "IG-88",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Bossk",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Lando Calrissian",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Lobot",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Ackbar",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Mon Mothma",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Arvel Crynyd",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Wicket Systri Warrick",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Nien Nunb",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Qui-Gon Jinn",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Nute Gunray",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Finis Valorum",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Padmé Amidala",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Jar Jar Binks",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Roos Tarpals",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Rugor Nass",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Ric Olié",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Watto",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Sebulba",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Quarsh Panaka",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Shmi Skywalker",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Darth Maul",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Bib Fortuna",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Ayla Secura",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Ratts Tyerel",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Dud Bolt",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Gasgano",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Ben Quadinaros",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Mace Windu",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Ki-Adi-Mundi",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Kit Fisto",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Eeth Koth",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Adi Gallia",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Saesee Tiin",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Yarael Poof",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Plo Koon",
          "filmConnection": {
            "totalCount": 3
          }
        },
        {
          "name": "Mas Amedda",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Gregar Typho",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Cordé",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Cliegg Lars",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Poggle the Lesser",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Luminara Unduli",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Barriss Offee",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Dormé",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Dooku",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Bail Prestor Organa",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Jango Fett",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Zam Wesell",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Dexter Jettster",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Lama Su",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Taun We",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Jocasta Nu",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "R4-P17",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Wat Tambor",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "San Hill",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Shaak Ti",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Grievous",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Tarfful",
          "filmConnection": {
            "totalCount": 1
          }
        },
        {
          "name": "Raymus Antilles",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Sly Moore",
          "filmConnection": {
            "totalCount": 2
          }
        },
        {
          "name": "Tion Medon",
          "filmConnection": {
            "totalCount": 1
          }
        }
      ]
    }
  }
}
```

11.Aggregate Film Statistics:

```Query
{
  allPeople {
    totalCount
  }
}
```

```Response
{
  "data": {
    "allPeople": {
      "totalCount": 82
    }
  }
}
```

12.Full Character Profiles:

```Query

```

```Response

```

13.Link Characters with Their Planets: 

```Query

```

```Response

```

14.Vehicles, Their Pilots, and Pilots' Species:

```Query

```

```Response

```

15.Films and Their Associated Entities:

```Query

```

```Response

```