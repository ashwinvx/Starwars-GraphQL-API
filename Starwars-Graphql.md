1. List All Films:

### Query
query Films {
  allFilms {
    films {
      title
    }
  }
}
###

### Response
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
###

2.Fetch a Specific Character:

###Query
query Person {
  person(id: "cGVvcGxlOjEz"){
    name
  }
}
###

###Response
{
  "data": {
    "person": {
      "name": "Chewbacca"
    }
  }
}
###

3.Explore Planets:

###Query
query Planets {
  allPlanets(first: 5) {
    planets {
      name
    }
  }
}
###

###Response
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
###

4.Starships Information: 

###Query
query AllStarships {
  allStarships(first: 3) {
    starships {
      name
      model
    }
  }
}
###

###Response
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
###

5.Character and Their Starships:

###Query

###

###Response

###

6.Species and Their Languages:

###Query

###

###Response

###

7.Planets and Their Climates:

###Query

###

###Response

###

8.Vehicles and Their Costs:

###Query

###

###Response

###
