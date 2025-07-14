

- MapKit JS
- GeoJSONDelegate
-  itemForMultiLineString 

Instance Method

# itemForMultiLineString

Overrides a multiline string.

MapKit JS 5.0+

``` source
optional(mapkit.Annotation|mapkit.Overlay|(mapkit.Annotation|mapkit.Overlay)[]) itemForMultiLineString(
 ItemCollection itemCollection,
 Object geoJSON
);
```

## Parameters 

`itemCollection`  

An item collection containing associated overlays.

`geoJSON`  

The original GeoJSON object for the `MultiLineString`. This contains an array of geometries.

## Return Value

A map item or an array of map items.

## Discussion

MapKit JS calls this method for every `MultiLineString` object. The framework also calls this method after constructing subitems and calling their delegate functions.

## See Also

### Overriding items

itemForFeature

Overrides a feature.

itemForFeatureCollection

Overrides a feature collection.

itemForLineString

Overrides a line string.

itemForPoint

Overrides a point.

itemForMultiPoint

Overrides a multipoint object.

itemForPolygon

Overrides a polygon.

itemForMultiPolygon

Overrides a multipolygon.

styleForOverlay

Overrides the style of overlays.

