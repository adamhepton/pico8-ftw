# FTW: Flood the World
## A "Learn by doing" Pico-8 game

Name: FTW - Flood the World

![BBS Cart](http://www.lexaloffle.com/bbs/cposts/3/31579.p8.png)

_If you save this image, you have a copy of the game._
 
![Latest Screenshot](https://adamhepton.github.io/pico8-ftw/screenshots/latest.png)

_Latest Screenshot_

[Play the Game in-browser](http://www.lexaloffle.com/bbs/?pid=31580)

Concept: You get three seconds to pick somewhere to unleash a storm.  You get a score based on how big a flood you make.

Each tile on the map has a randomly-assigned amount of “slope” which determines how much accumulated water is needed to spread to neighbouring tiles.  Each tile also has an amount of water within it, which accumulates as the flood spreads.

Progress:
Procedurally generated map with two bits of data per tile - one for slope, one for collectable water.  Map being represented by sprites depicting how much/little hill and water there is per-tile, but at the moment just flat top-bottom hills existing, need to do neighbour recognition to form river-type shapes that join up properly.

Map can be sized dynamically and seeded according to how much impenetrable hill is placed (fully dark tiles) vs spreadable hill (any tile with beige on it).  Map is scrollable, currently set at 150x150 because that seems like the biggest it will feasibly go, at least the way I’m storing it right now ;)

Next:
Make joined river graphics make sense to the human eye.

Any feedback welcomed, either conceptually, about how I'm misusing Pico-8 or anything else.  This is the first time I've really spent more than an hour on anything with Pico-8 so I'm very much learning as I go.
