# Reference
Curated data storage for Artemis

# Sources

* `locations/places.json`: This file is based on the labels displayed on [the
  official Wynncraft map](https://map.wynncraft.com/). It is extracted from
  https://map.wynncraft.com/js/labels.js using the script
  https://github.com/Wynntils/Data-Storage/blob/master/scripts/extract_labels.sh.

* `locations/services.json`: This file is based on raw data gathered by playing
Wynncraft with Wynntils, and using the `/detection` command to automatically
find NPCs and other labeled POIs within the game. This raw data is parsed,
cleaned and separated by the script
https://github.com/Wynntils/Data-Storage/blob/master/locations/process-collected-locations.sh.
The latest raw data used is available here:
https://github.com/Wynntils/Data-Storage/blob/master/locations/raw/2022-07-08-by-Pyro.csv

* `locations/spirits.json`: This file is based off the coordinates for lost spirits in the bonfire/spirit event.
Collection involves checking the wiki for the current year (2022) at
[Festival of the Bonfire](https://wynncraft.fandom.com/wiki/Festival_of_the_Bonfire_(2022))
and preferably verifying the validity of the data. The wiki itself is not parsed due to potential for griefs as
well as technical limitations.
