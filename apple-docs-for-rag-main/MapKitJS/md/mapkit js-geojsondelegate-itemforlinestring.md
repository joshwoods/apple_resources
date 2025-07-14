

- MapKit JS
- GeoJSONDelegate
-  itemForLineString 

Instance Method

# itemForLineString

Overrides a line string.

MapKit JS 5.0+

``` source
optional(mapkit.Annotation|mapkit.Overlay|(mapkit.Annotation|mapkit.Overlay)[]) itemForLineString(
 mapkit.PolylineOverlay overlay,
 Object geoJSON
);
```

## Parameters 

`overlay`  

A mapkit.PolylineOverlay object.

`geoJSON`  

The original GeoJSON object for the `LineString` object.

## Return Value

A map item or an array of map items.

## Discussion

MapKit JS calls this method for each individual `LineString` geometry object. You can customize or completely replace the provided overlay before returning it.

## See Also

### Overriding items

itemForFeature

Overrides a feature.

itemForFeatureCollection

Overrides a feature collection.

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

