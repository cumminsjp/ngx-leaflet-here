# ngx-leaflet-here
Angular 6 Service for Leaflet and HERE. 

This service wraps  [leaflet-tilelayer-here.js](https://gitlab.com/IvanSanchez/Leaflet.TileLayer.HERE/blob/master/leaflet-tilelayer-here.js) into an injectable service that will return a tile layer.

```
  constructor(private http: HttpClient, private here: LeafletHEREService) {

    var hereTileLayer = here.createTileLayer({
      appId: '<your appId goes here',
      appCode: '<your appCode goes here',
      scheme: 'pedestrian.day.mobile'
    });

```
