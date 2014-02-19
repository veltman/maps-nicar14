# Creating maps: principles, mistakes, and potential #

## Making a map ##

Should you be making a map?
* What are maps for, anyway? Orienting self, locating one's own place quickly, showing a geographic trend, service journalism for things happening in physical space.
* Map as interface vs. map as story
* But pretty much everything happens in physical space. It doesn't all belong on a map.
* DON'T MAKE POPULATION MAPS.
* Tradeoffs of different types of map, bar charts - ease of locating, ease of comparing two places, ease of highlighting regional trends, ease of identifying extremes, ease of identifying distribution.  WaPo Senate map as example.

Everyone gerrymanders.
* If your data is grouped, you're skewing the results no matter what level of detail you map it at.  What is the proper atomic unit?  Is the real story state vs. state, urban vs. rural, east vs. west? Should you be using political units, or arbitrary units of equal area?

Making a map doesn't mean making a map James Cook could navigate with.
* All maps are opinionated. Embrace it. Tell the story you want to tell, mindfully.  Think about transit maps: sacrificing some geographic fidelity in favor of ability to parse the system.

Building a map, the basics:
* Anatomy of a tilemap, advantages and limitations.
* Non-tilemap alternatives, advantages and limitations.

Map design issues:
* Centroid disease - assigning things to center point of a place.  Especially large problem if you have data with mixed precision (some street level, some city level)
* Explosion at the map marker factory - impenetrable thicket of markers makes a map pretty useless, esp. if they don't scale with zoom.  What is the actual need you're trying to meet with them?  Can you bin them, or exclude some, or only show one subcategory at a time?
* Projections (not sure how much we should actually talk about this, it seems beaten to death)
* Not thinking about zoom - if your map is zoomable, every zoom level is a separate feature.  Things should scale and show/hide gracefully based on zoom level. Restrict zoom level to the useful range if zooming out too far or too close would discombobulate.
* Overcrowded map with defaults - esp. true with base layers full of streets, parks, etc. I'm looking at you, Google Maps API. Lots of noise obscuring your data. Easy solutions include MapBox or Gmaps styling wizard.
* Overcrowded map with data - Don't expect people to hold a whole map with multiple data dimensions in working memory.  Focus attention, leave things out.
* Showing giant maps on tiny screens - esp. true with tilemaps, where the same swipe-to-scroll event might get captured by browser, might get captured by map instead.
* Colors and maps - Color is one of the primary tools for showing data with a map.  But how well people perceive scale, contrast, depends a lot on your colors.  Do you scale continuously or in intervals? Do you show winner-take-all or gradient? How many categorical colors is too many?

## Geographic data ##

### What does geographic data look like? ###
* Pretty much everything is a list of latitudes and longitudes. If you speak lat/lng you speak map.
* Intro to formats: shapefiles, GeoJSON, TopoJSON, KML
* Touch on OpenStreetMap

### Geographic data issues ###
* Precision - Large files are large.  Simplification can drop things altogether if you're not careful.
* CRS - sometimes things don't come in lat/lng.
* Real-world geography is messy - How many countries are there? Is Greenland part of Denmark? Is Puerto Rico part of the US? Census tracts can include parks, harbors, etc. Is Belgium one country or Flanders+Wallonia? Pakistan election map - how to deal with Kashmir? And boundaries change.

## Data to put on a map ##

### Data issues ###
* Data join problems: name mismatches, sovereignty mismatches. South Korea vs. Korea vs. Republic of Korea vs. S. Korea.  How many different names can you come up with for Hong Kong?  The UN has 4.
Outlying islands, etc. that skew results.
* Ignoring confounding variables (like all journalism) - e.g., a crime map where the hotspot has a lot of car theft and violent crime is elsewhere.
* Geocoding issues: if your geographic data consists of addresses, not unique IDs or lat/lngs, proceed very carefully.

## Tipsheet ##

### Tools ###
QGIS  
Matt Bloch's Mapshaper  
ADC4GIS ogr2ogr converter  
MapBox suite  
Leaflet  
Google Maps API  
D3  
MapStack  
CartoDB  
Kartograph.js  
OpenStreetMap ecosystem  
Google Maps API, Geocoder  
Gmaps styling wizard

### Tutorials ###
Mapschool  
MapBox docs  
ForJournalism mapping session  
Bostock's Let's Make a Map  

### Data sources ###
US census  
Natural Earth  
OSM  
Wikimedia SVGs  