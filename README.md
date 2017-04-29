## Thesis App
This repository contains updates and notes for the visualiztion app

## Key files

#### [parser.js](https://github.com/neuralism/thesis-app/blob/master/parser.js)
- Parses log file based on specificed ruleset into JSON file
- Checks one-word names against list of monsters with one-word names
- Requests item names from [NotAion API](http://api.notaion.com/) as they are not in the log file (once per 0.5 seconds)

#### [monster.js](https://github.com/neuralism/thesis-app/blob/master/monster.js)
- Generates a file containing a list of monsters with one-word names from on list containing [all monsters]() scraped from [aiondatabase.net](http://aiondatabase.net)

#### [insert.js](https://github.com/neuralism/thesis-app/blob/master/insert.js)
- Inserts processed log file into Mongo database

#### [server.js]((https://github.com/neuralism/thesis-app/blob/master/server.js)
- Listens for requests and queries database for a slice of the data
- Transforms requested data and sends it over to the client

