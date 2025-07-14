

- MapKit JS
- GeoJSONDelegate
-  itemForPolygon 

Instance Method

# itemForPolygon

Overrides a polygon.

MapKit JS 5.0+

``` source
optional(mapkit.Annotation|mapkit.Overlay|(mapkit.Annotation|mapkit.Overlay)[]) itemForPolygon(
 mapkit.PolygonOverlay overlay,
 Object geoJSON
);
```

## Parameters 

`overlay`  

You can customize the provided overlay before returning it, or you can completely replace the overlay.

`geoJSON`  

The original GeoJSON object for the polygon.

## Return Value

A map item or an array of map items.

## Discussion

MapKit JS calls this method for each individual `polygon` geometry object. The framework breaks `MultiPolygon` geometry types into individual polygon types.

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

itemForMultiPolygon

Overrides a multipolygon.

styleForOverlay

Overrides the style of overlays.

