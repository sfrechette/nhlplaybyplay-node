# nhlplaybyplay-node
Fetch NHL Play by Play game data in JSON file format

## Purpose
Application built using Node.js that provides the means for accessing, fetching NHL Schedule and Play by Play game data in JSON format. 

**Hope your familiar with this…**

2016-2017 NHL Season Schedule -> 
http://live.nhl.com/GameData/SeasonSchedule-20162017.json

Play by Play for game 2016020031 ->
http://live.nhl.com/GameData/20162017/2016020031/PlayByPlay.json

*Note: Schedule and Play by Play data only available from the 2011-2012 NHL Season and onward…*

## Installation
Install the dependencies with the following command:
```
npm install
```

Create a `data` directory:
```
mkdir data
```

**Before using you will need to create a specific directory for each of the seasons you will be fetching data for.**

i.e. To fetch data from the 2012-2013 NHL season you need to create the following folder `20122013` under the `data` directory. 

## Usage
node fetch.js *season* *[game]*

To fetch all games for a specific season:
```
node fetch.js 20152016
```

To fetch specific game from a specific season
```
node fetch.js 20162017 2016020001
```

Will be adding parsing functionallity in the near future...
Enjoy!