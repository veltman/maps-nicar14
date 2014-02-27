It's pretty easy to make maps now. Choropleths and Google Maps marker forests are everywhere.  But with that ease comes a temptation to repeat yourself (or someone else) unthinkingly. [re: Mad Libs quote.]

There is rarely one obvious right answer.  My own #1 principle:

* Mindfulness.
Do things for a reason.
Do things for a reason besides "that's how we did it before."

---

Mapmaking mistakes

---

Making a map instead of a bar chart.

[WaPo gun deaths chart]

Bar charts are still popular for a reason. They're great for comparing values. It's easy to identify extremes, easy to identify the overall distribution.  People are pretty good at seeing scale when it's the length of a bar. It's not biased by the fact that Nevada is bigger than Delaware.  There are downsides: it's harder to locate your own place.  It obscures geographic trends, if there are meaningful ones (be careful: there may be fake ones).

---

Making a map instead of writing a sentence.

If the lede of your map is one sentence, why are you making a map?  If all you want to show is that California is off the charts compared to everywhere else, just say that and save yourself the aggravation.

---

Not mapping what you think you're mapping.

"The Fusion Tables map gets halfway around the world before the truth gets its pants on." -Mark Twain, probably

[Hate tweets]

[NY crime maps]

Data on maps is no different than data you're hearing about in every other NICAR session.  It's easy to miss the real story.  There are lots of confounding variables when it comes to human geography.  It's easy to conflate two things or accidentally map a different variable.  Tom mentioned population.  Don't make population maps. BREAKING: lots of people live in cities.

Be careful with rates too.  Results can get VERY skewed in sparsely-populated places.

FlowingData as case study.
Lesson in mindfulness about data, but also about openness.  It's OK for your data to be imperfect.  It's OK to use proxies.

"You go to journalism with the data you have, not the data you want." -Donald Rumsfeld, probably

But you should wear those warts on your sleeves.  Explain where the data is from, what it means, what it doesn't mean, and what you don't know.  This is better for your audience, but it's also better for you.  Going through that thought process will probably wake you up to some questions you should be asking as you go.

"Find a rabbi." -Ben Welsh

Talk to subject experts. Get their smell test. They probably know the obscured patterns better than you.

---

Gerrymandering.

[Everybody gerrymanders book cover]

If your data is grouped, you're skewing the results no matter what level of detail you map it at. There's no way around that. But you can mitigate it in your choose of units.  What is the proper atomic unit?  Is the real story state vs. state, urban vs. rural, east vs. west? Should you be using political units, or arbitrary units of equal area? How precise do you want to get? Binning.

---

Overstuffing.

[Monty Python's Meaning of Life]

Trying to tell three stories at once with a map means you wind up telling zero. You're in the business of focusing attention, so don't compete against yourself. You don't want a million labels and points and and shapes and colors all screaming for a user's attention. If your map looks like an explosion at the data factory consider paring things down, binning them, or categorizing them.

---

One size fits all?

You're probably designing your map on a beautiful cinema display, but half or more of your users will be using tiny screens.  You don't have much real estate to get your point across.  And if you make people play Operation with their thumb trying to click on things, they will hate you.  Also, don't make tilemaps that take up the whole screen with additional content.

---

Ignoring zoom.

This is a very map-centric problem. The world-level view and the street-level view of the same data-driven map can be wildly different. Treat different zoom levels as different maps when you're testing it out. Consider limiting zoom levels to the useful range.  If the map looks dumb or useless or confusing at a given zoom level, why do you want them to get there? It's easy to get discombobulated on a tilemap.

---

Color blindness.

Color is one of the primary tools for showing data with a map.  But how well people perceive scale, contrast, depends a lot on your colors.  Do you scale continuously or in intervals? Quantiles, equal intervals, natural breaks?  Do you show winner-take-all or a gradient? How many categorical colors is too many? Use things like Colorbrewer to help with color ramps.  Don't go color crazy. Colorblindness: significant problem, especially red/green.  Colors that look vivid and high-contrast on your cinema display might look like crap on someone's Cheap Dell Monitor (TM) or phone.

---

Geography is an asshole.

There's a good chance if you're making a map you're going to end up doing some sort of data join. You've got a spreadsheet of data about unemployment rates, GDP, favorite baseball team, etc. and then you need to join it to the map shapes. This can go very wrong.

How many countries are there? UN: 193/206, ISO: 249, FIFA: 209. According to whom (e.g. Kashmir)? With US data you might get Puerto Rico, Guam, American Samoa, Northern Mariana Islands. Is Greenland in Denmark? And boundaries change. Districts gonna redistrict. 

Boundaries can also include water, parks, etc. As a general rule: the more geographically precise the data is, the more susceptible it is to weird quirks, like a place nobody lives or a prison or a hospital.

---

People entering data are assholes.

South Korea, Korea, Republic of Korea, S. Korea, (in Korean).

The LA traffic citation system has 49 ways to spell Cahuenga (Cahaunga, Caheinga, Cahenga, Caheunga, Cahienga, Cahlenga, Cahoengia, Cahu, Cahubnga and Cahue).

Things get especially sticky if you have to geocode data (physical address -> geographic point): false positives, false negatives, the dreaded centroid disease.

Avoiding data join problems: review your data carefully. Make sure n = n. AB(S)C. Always Be Spot Checking.

---