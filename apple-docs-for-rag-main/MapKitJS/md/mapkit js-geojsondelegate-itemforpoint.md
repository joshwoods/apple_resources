

- MapKit JS
- GeoJSONDelegate
-  itemForPoint 

Instance Method

# itemForPoint

Overrides a point.

MapKit JS 5.0+

``` source
optional(mapkit.Annotation|mapkit.Overlay|(mapkit.Annotation|mapkit.Overlay)[]) itemForPoint(
 mapkit.Coordinate coordinate,
 Object geoJSON
);
```

## Parameters 

`coordinate`  

A GeoJSON `Point` generates the coordinate. You can use the coordinate to instantiate an item to return.

`geoJSON`  

The original GeoJSON object for the `Point`. This object may be a simple `Point` or a `Feature` with the `Point` geometry type.

## Return Value

An array of map items.

## Discussion

MapKit JS calls this method for every `Point` object. For a `MultiPoint` object or for a `GeometryCollection` of `Points` and `MultiPoints`, the framework calls itemForPoint for each individual `Point` object.

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

itemForMultiPoint

Overrides a multipoint object.

itemForPolygon

Overrides a polygon.

itemForMultiPolygon

Overrides a multipolygon.

styleForOverlay

Overrides the style of overlays.

