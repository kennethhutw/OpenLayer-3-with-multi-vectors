OpenLayers 3
----

Create three features and put into an array.
```code

  var iconFeatures=[];
  var iconFeature = new ol.Feature({
						  geometry: new ol.geom.Point(ol.proj.transform([103.6080804,1.3571318], 'EPSG:4326',     
						  'EPSG:3857')),
						  name: 'Null Island',
						  population: 4000,
						  rainfall: 500
						});
  var iconFeature1 = new ol.Feature({
						  geometry: new ol.geom.Point(ol.proj.transform([103.9080804,1.5571318], 'EPSG:4326',     
						  'EPSG:3857')),
						  name: 'Null Island',
						  population: 4000,
						  rainfall: 500
						});

  var iconFeature2 = new ol.Feature({
						  geometry: new ol.geom.Point(ol.proj.transform([103.8080804,1.3571318], 'EPSG:4326',     
						  'EPSG:3857')),
						  name: 'Null Island',
						  population: 4000,
						  rainfall: 500
						});

var iconStyle = new ol.style.Style({
  image: new ol.style.Icon(/** @type {olx.style.IconOptions} */ ({
    anchor: [0.5, 46],
    anchorXUnits: 'fraction',
    anchorYUnits: 'pixels',
    opacity: 0.75,
    src: 'http://openlayers.org/en/v3.0.0/examples/data/icon.png'
  }))
});

iconFeature.setStyle(iconStyle);
iconFeature1.setStyle(iconStyle);
iconFeature2.setStyle(iconStyle);
iconFeatures.push(iconFeature);
iconFeatures.push(iconFeature1);
iconFeatures.push(iconFeature2);

```

