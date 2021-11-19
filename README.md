# Runescape_projects
Runescape is a hobby of mine, and these are my adventures

This repository is for various runescape projects that I have

1. Archeology Web Scrape
This project came about as I saw potential to add something to the Runescape Wikipedia page. There are lists of artefacts and materials that are used in the skill.
However, I like to be prepared, and frequently frustrated by not having enough of the required materials. While the number of materials needed for each individual artefact is easily accesible, along with the number of artefacts required, no one had joined these two together, to produce a definitive materials list.
This is further complicated since materials are used across multiple artefacts, each artefact uses a different amount of materials, and each artefact is required a different number of times.
The number of artefacts was determined to be the minimum number required to complete all the in game collections and mysteries (see https://runescape.wiki/w/Archaeology)
I initially opted to build this list for personal use.
So i used beautiful soup, alongside requests, to pull the web page I needed. Then parsed out the tables required, and extracted the needed information about each artefact and the materials needed.

It's a very duct tape job, but it works

Then I complied the materials into dictionaries the value being what was needed for that artefact.
The looped through all the artefacts, noted how many are required and incremented each material count by the product of the material needed for that artefact and the number of artefacts required.

Further to this I edited the wiki page, to reflect my knowledge and help others. Experience with the Lua language.

While the first iteration worked out okay (after two tries) I am currently forgoing visual editing, which I did to get familar, and am now editing at the code level for better clarity, and so that the variables are linked.
This is because it is not unlikely that new content may be added to the game, as a result, the values would have to be recomputed and re edited, however, if the table is able to perform the calculations internally, this would be better as there will be less to change, and no longer rely upon the webscraping, as all the information needed is contained on the same page
