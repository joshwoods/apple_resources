

- MapKit JS
- GeoJSONDelegate
-  itemForFeatureCollection 

Instance Method

# itemForFeatureCollection

Overrides a feature collection.

MapKit JS 5.0+

``` source
optional(mapkit.Annotation|mapkit.Overlay|(mapkit.Annotation|mapkit.Overlay)[]) itemForFeatureCollection(
 ItemCollection itemCollection,
 Object geoJSON
);
```

## Parameters 

`itemCollection`  

A collection containing associated annotations and overlays.

`geoJSON`  

The original GeoJSON object for the `FeatureCollection`. This contains an array of `feature` types.

## Return Value

A map item or an array of map items.

## Discussion

MapKit JS calls this method for every GeoJSON `FeatureCollection` object. The framework also calls this method after constructing subitems and calling their delegate functions.

## See Also

### Overriding items

itemForFeature

Overrides a feature.

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

itemForMultiPolygon

Overrides a multipolygon.

styleForOverlay

Overrides the style of overlays.

