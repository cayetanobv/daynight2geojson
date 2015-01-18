##Description

Get day and night global geometry and dumps to a GeoJSON file.

Output projection: Equirectangular (Cylindrical Equidistant)


##Requirements

- Geojson Python library. https://github.com/frewsxcv/python-geojson
- Shapely Python Library. https://github.com/Toblerity/Shapely
- Matplotlib Basemap Toolkit Python Library. https://github.com/matplotlib/basemap


##Usage

Basic usage:

```
from datetime import datetime
from daynight2geojson import DayNight2Geojson

filepath = '/tmp/day_night.geojson'
input_date = datetime(2015, 1, 15, 12, 00)

dn = DayNight2Geojson(filepath)
dn.getDayNight()
```

Test script:
- lib/bootstrap.py
