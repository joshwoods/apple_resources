

- MapKit JS
- GeoJSONDelegate
-  styleForOverlay 

Instance Method

# styleForOverlay

Overrides the style of overlays.

MapKit JS 5.0+

``` source
mapkit.Style styleForOverlay(
 mapkit.Overlay overlay,
 Object geoJSON
);
```

## Parameters 

`overlay`  

The overlay to style.

`geoJSON`  

The original GeoJSON for the `feature` or `geometry` object`.`

## Return Value

This method returns a mapkit.Style object for the provided overlay.

## Discussion

MapKit JS calls this method for each overlay, and after each call to itemForPoint and itemForPolygon.

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

itemForMultiPolygon

Overrides a multipolygon.

