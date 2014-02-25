# Creating maps: principles, mistakes, and potential

By Noah Veltman (@veltman) and Tom MacWright (@tmcw)

## Making a map

---

### Why are you making a map?

---

### Everything happens somewhere.

---

### Maps are good for:
### Telling a story about geography (map as story)
### Orienting yourself (map as interface)

---

### DON'T MAKE POPULATION MAPS.

[BREAKING: lots of people live in cities.]  
[Rates > absolute quantities.]  
[Background: pop map]

---

### Human geography is complicated.

[Are you just mapping a proxy for the real story?]  
[Are you unintentionally conflating multiple things into one?]  
[A geographic pattern can be illuminating to people familiar with the place, misleading to people who aren't]  
[Background: crime map]

---

### Make a bar chart instead.

[Easier to identify extremes, distribution. Not biased by physical space.]  
[Harder to locate your own place.  Much harder to see geographic trends, if they are real.]  
[Background: WaPo shootings bar chart]

---

### Write a sentence instead.

[Not everything is best served by a rich visual. If the story is one sentence long, write that sentence instead.]

---

## Some map design issues ##

### You are not a sea captain.

[All maps are opinionated. Embrace it. Geographic fidelity can be a drawback. Think about transit maps: sacrificing some geographic fidelity in favor of readability.]  
[Background: subway map, WaPo senate block chart.]

---

### Everyone gerrymanders.

[If your data is grouped, you're skewing the results no matter what level of detail you map it at.]  
[What is the proper atomic unit?  Is the real story state vs. state, urban vs. rural, east vs. west? Should you be using political units, or arbitrary units of equal area?]  
[Binning]

---

### Cramming in too much.

[Trying to tell three stories at once with a map means you wind up telling zero.]  
[Don't be afraid of small multiples. They make for better comparisons, and they're especially great for tiny screens.]  
[Also the issue of noise, esp. with default tiles full of labels.  Ruthlessly discard things that don't help the story, or it becomes a stock trading floor, with everything screaming for your attention at once.]  
[Background: that guy from Monty Python's Meaning of Life exploding]

---

### Forgot about zoom.

[Standard map behaviors: zoom, pan; don't toy with them]  
[Different zoom levels tell different stories. Consider them all, and restrict them if appropriate. Don't let a user get stranded in the micro- or macroscope]  
[Background: Zoomed out world with markers clustered]

---

### Explosion at the marker factory.

[Plopping a million markers down on a map is easy and useless.  Consider paring them down, binning them, or categorizing them.]

---

### One size fits all?

[Remember that half or more of your users will be using tiny screens, stabbing with their thumbs.  And tilemaps will capture scroll events.  Don't make tiny Xs.]

---

### Colors.

[Color is one of the primary tools for showing data with a map.  But how well people perceive scale, contrast, depends a lot on your colors.  Do you scale continuously or in intervals? Do you show winner-take-all or   gradient? How many categorical colors is too many?  Use things like Colorbrewer to help with color ramps.  Don't go color crazy.]  
[Colorblindness: significant problem, especially red/green.]  
[Colors that look vivid and high-contrast on your cinema display might look like crap on someone's Cheap Dell Monitor (TM) or phone.]

## Geographic data ##

### It's all lat/lngs.

[If you speak lat/lng you speak map.]

---

### This is a lat/lng.

[Background: point.]

---

### This is three lat/lngs.

[Background: polyline.]

---

### This is four lat/lngs.

[Background: colorado]

---

### Shapefiles, GeoJSON, TopoJSON, KML: aka lists of lat/lngs.

---

## Geographic data issues ##

### Geography trivia lightning round!

---

### How many countries are there?
UN: 193/206
ISO: 249
FIFA: 209

---

### According to whom?

[Background: Kashmir, Taiwan]

---

### Is this in Denmark?

[Background: Greenland]

---

### U-S-A! U-S-A! U-S-A!

[Background: Puerto Rico, Guam, American Samoa, Northern Mariana Islands]

---

### Some low-density census tracts:

[Background: Golden Gate Park, Boston harbor]

---

### Boundaries change.

[Background: side-by-side of congressional districts]

---

### What is this country called?
### South Korea
### Korea
### Republic of Korea
### S. Korea
### (in Korean)

[Background: South Korean flag]  
[Data join problems are one of the biggest gotchas trying to make a map in the newsroom.]

---

### 49 ways to spell Cahuenga.

[Cahaunga, Caheinga, Cahenga, Caheunga, Cahienga, Cahlenga, Cahoengia, Cahu, Cahubnga and Cahue]  
[Background: Cahuenga Boulevard street sign]  
[Ref: http://www.latimes.com/news/opinion/la-oe-smith-lapd-spelling-errors,0,4445429.htmlstory#axzz2uGaL4kMp]

---

### Geocoding

[If your geographic data consists of addresses, not unique IDs or lat/lngs, proceed very carefully.  Hand-entered, unsanitized.]  
[Related: centroid disease: are things that sort into entire state/county being pinned to the exact point in the middle?]

---

### Questions?

---