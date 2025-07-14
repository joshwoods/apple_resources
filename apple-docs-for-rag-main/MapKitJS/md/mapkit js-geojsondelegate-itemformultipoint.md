

- MapKit JS
- GeoJSONDelegate
-  itemForMultiPoint 

Instance Method

# itemForMultiPoint

Overrides a multipoint object.

MapKit JS 5.0+

``` source
optional(mapkit.Annotation|mapkit.Overlay|(mapkit.Annotation|mapkit.Overlay)[]) itemForMultiPoint(
 ItemCollection itemCollection,
 Object geoJSON
);
```

## Parameters 

`itemCollection`  

A collection containing associated annotations.

`geoJSON`  

The original GeoJSON object for the `MultiPoint`. This contains an array of geometries.

## Return Value

A map item or an array of map items.

## Discussion

MapKit JS calls this method for every `MultiPoint` object. The framework also calls this method after constructing subitems, and calling their delegate functions.

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

itemForPolygon

Overrides a polygon.

itemForMultiPolygon

Overrides a multipolygon.

styleForOverlay

Overrides the style of overlays.

