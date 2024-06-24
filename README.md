# spark-map
[Web map](https://huvidragon.github.io/spark-map) template using Leaflet

All data is (c)[OpenStreetMap](https://openstreetmap.org) Contributors

## Helpful Resources:
* [Leaflet](https://www.leafletjs.com)
* [HTML](https://www.w3schools.com/html/)
* [CSS](https://www.w3schools.com/css/)
* [GeoJSON.io](https://www.geojson.io)
* [JavaScript](https://www.w3schools.com/js/default.asp)
* [Overpass API](http://www.overpass-api.de/)

### Overpass Query for User-Created Features
```
[out:json][timeout:25];
// gather results
(
  // query part for: “building”
  way["building"](user:"username1","username2")({{bbox}});
);
// print results
out body;
>;
out skel qt;
```
