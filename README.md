# proj4m
proj4 minimal/maptalks

## supported projection
- Normal
    - EPSG:3857, `+proj=merc +a=6378137 +b=6378137 +lat_ts=0.0 +lon_0=0.0 +x_0=0.0 +y_0=0 +k=1.0 +units=m +nadgrids=@null +wktext  +no_defs`
    - EPSG:4326, `+proj=longlat +datum=WGS84 +no_defs`
- GCJ02
    - GCJ02, `+proj=longlat +dataum=GCJ02`
    - Projected GCJ02, `+proj=merc +datum=GCJ02`
- BD09
    - BD09LL, `+proj=longlat +datum=BD09`
    - BD09MC, `+proj=bmerc +datum=BD09`

## TODO
Add alias for these projectons, then can be used like:
```
Proj4 proj = new Proj4("+proj=bmerc +datum=BD09", "EPSG:3857");
```
