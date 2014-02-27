---

Making a map instead of a bar chart.

Easier to identify extremes, distribution. Not biased by physical space. Harder to locate your own place.  Much harder to see geographic trends, if they are real. Background: WaPo shootings bar chart.

---

Making a map instead of writing a sentence.

---

Not mapping what you think you're mapping.
Population maps, confounding variables, conflating groups together. BREAKING: lots of people live in cities. Hate tweets. FlowingData as case study: lesson is mindfulness about data, but especially being specific about where the data comes from and its limitations.

---

Gerrymandering.

If your data is grouped, you're skewing the results no matter what level of detail you map it at. What is the proper atomic unit?  Is the real story state vs. state, urban vs. rural, east vs. west? Should you be using political units, or arbitrary units of equal area? Binning.

---

Overstuffing.

Trying to tell three stories at once with a map means you wind up telling zero. Also the issue of noise, esp. with default tiles full of labels.  Ruthlessly discard things that don't help the story, or it becomes a stock trading floor, with everything screaming for your attention at once. Explosion at the marker factory: Plopping a million markers down on a map is easy and useless.  Consider paring them down, binning them, or categorizing them.

---

One size fits all?

Remember that half or more of your users will be using tiny screens, stabbing with their thumbs.  And tilemaps will capture scroll events.  Don't make tiny Xs.

---

Ignoring zoom.

Standard map behaviors: zoom, pan; don't toy with them.  Different zoom levels tell different stories. Consider them all, and restrict them if appropriate. Don't let a user get stranded in the micro- or macroscope. Background: Zoomed out world with markers clustered.

---

Color blindness.

Color is one of the primary tools for showing data with a map.  But how well people perceive scale, contrast, depends a lot on your colors.  Do you scale continuously or in intervals? Do you show winner-take-all or   gradient? How many categorical colors is too many?  Use things like Colorbrewer to help with color ramps.  Don't go color crazy. Colorblindness: significant problem, especially red/green.  Colors that look vivid and high-contrast on your cinema display might look like crap on someone's Cheap Dell Monitor (TM) or phone.  Can use equal intervals, quantiles, natural breaks/Jenks.

---

Geography is an asshole.

How many countries are there? UN: 193/206, ISO: 249, FIFA: 209. According to whom? Kashmir, Taiwan. Puerto Rico, Guam, American Samoa, Northern Mariana Islands. Greenland. Changing boundaries. Background: Golden Gate Park, Boston harbor. The more detailed the data, the more susceptible to weird quirks, like a place nobody lives or a prison or a hospital.

---

People entering data are assholes. South Korea, Korea, Republic of Korea, S. Korea, (in Korean).  LA traffic citation system has 50 ways to spell Cahuenga (Cahaunga, Caheinga, Cahenga, Caheunga, Cahienga, Cahlenga, Cahoengia, Cahu, Cahubnga and Cahue).  This is particularly problematic if you have to geocode data (physical address -> geographic point): false positives, false negatives, the dreaded centroid disease.

---