![alt tag](https://stephanefrechette.com/blog/wp-content/uploads/2017/04/hockey-rink.png)

# nhlplaybyplay-node
Fetch and Convert NHL Play by Play game data 

## Purpose
Application built using Node.js that provides the means for accessing, fetching NHL Schedule and Play by Play game data in JSON format and
converting the output to CSV.

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

*Before using you will need to create a specific directory for each of the seasons you will be fetching data for.*

i.e. To fetch data from the 2012-2013 NHL season you need to create the following folder `20122013` under the `data` directory. 

## Usage
**Fetch Play by Play JSON**  
node fetch.js *season* *[game]*

To fetch all games for a specific season:
```
node fetch.js 20152016
```

To fetch a specific game from a specific season
```
node fetch.js 20162017 2016020001
```

**Convert Play by Play JSON to CSV**   
node convert.js *season* *[game]*

To convert all games for a specific season:
```
node convert.js 20152016
```

To convert a specific game from a specific season
```
node convert.js 20162017 2016020001
```

