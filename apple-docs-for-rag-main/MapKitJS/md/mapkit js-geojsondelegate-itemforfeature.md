

- MapKit JS
- GeoJSONDelegate
-  itemForFeature 

Instance Method

# itemForFeature

Overrides a feature.

MapKit JS 5.0+

``` source
optional(mapkit.Annotation|mapkit.Overlay|(mapkit.Annotation|mapkit.Overlay)[]) itemForFeature();
```

## Parameters 

`item`  

An item the system creates for the geometry of the feature, or `null` for features with `null` geometry.

`geoJSON`  

The original GeoJSON object for the `feature`.

## Return Value

A map item for the `feature`.

## Discussion

MapKit JS calls this method for every GeoJSON `feature`.

## See Also

### Overriding items

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

itemForMultiPolygon

Overrides a multipolygon.

styleForOverlay

Overrides the style of overlays.

