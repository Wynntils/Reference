# Reference
High-quality data storage for Artemis, based on automatic extraction from external, reliable sources

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

* `locations/combat.json`: This file is based on the same raw data outlined for services.json above.
However, it includes names pertinent to the type of combat location, such as "The Nameless Anomaly"
name field for an entrance in the type "Raids".

* `locations/hotspots.json`: This file is based on data collected from the Wynncraft API, via the
script found at https://github.com/Wynntils/Data-Storage/blob/master/scripts/update-wynn-locations.sh.
This API can get outdated fast and there is no other good way to get this data since these are defined on otherwise
abstract locations. However, both types of POI (Caves and Grind Spots) found in this file can be cross-referenced
using the Wynncraft Map.

* `locations/spirits.json`: This file is based off the coordinates for lost spirits in the bonfire/spirit event.
Collection involves checking the wiki for the current year (2022) at
[Festival of the Bonfire](https://wynncraft.fandom.com/wiki/Festival_of_the_Bonfire_(2022))
and preferably verifying the validity of the data. The wiki itself is not parsed due to potential for griefs as
well as technical limitations.

* `materials/materials.json`: This file is a modified version of https://raw.githubusercontent.com/PrismarineJS/minecraft-data/master/data/pc/1.12/items.json. It is used to convert old material ids to the new material name system in Artemis.


* `lootruns/lootrun_tasks.json`: The data for this file can be collected with `LootrunBeaconLocationCollectorFeature` in Artemis. Data is processed by the script found at `https://github.com/Wynntils/Data-Storage/blob/master/scripts/merge_lootrun_data.py`.
