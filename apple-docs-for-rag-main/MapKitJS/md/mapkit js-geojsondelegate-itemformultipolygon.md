

- MapKit JS
- GeoJSONDelegate
-  itemForMultiPolygon 

Instance Method

# itemForMultiPolygon

Overrides a multipolygon.

MapKit JS 5.0+

``` source
optional(mapkit.Annotation|mapkit.Overlay|(mapkit.Annotation|mapkit.Overlay)[]) itemForMultiPolygon(
 ItemCollection itemCollection,
 Object geoJSON
);
```

## Parameters 

`itemCollection`  

A collection containing associated overlays.

`geoJSON`  

The original GeoJSON object for the `MultiPolygon`. It contains an array of geometries.

## Return Value

A map item or an array of map items.

## Discussion

MapKit JS calls this method for every `MultiPolygon` object. The framework also calls this method after constructing subitems, and calling their delegate functions.

## See Also

### Overriding items

itemForFeature

Overrides a feature.

itemForFeatureCollection

Overrides a feature collection.

itemForLineString

Overrides a line string.

itemForMultiLineString

Overrides a multiline string.

itemForPoint

Overrides a point.

itemForMultiPoint

Overrides a multipoint object.

itemForPolygon

Overrides a polygon.

styleForOverlay

Overrides the style of overlays.

