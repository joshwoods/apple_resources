

- MapKit JS
- mapkit.Map
-  annotationForMapFeature 

Instance Method

# annotationForMapFeature

The method MapKit JS calls when the framework creates a map feature annotation.

MapKit JS 5.74+

``` source
void annotationForMapFeature(
 mapkit.MapFeatureAnnotation mapFeatureAnnotation
);
```

## Discussion

You can choose to return the annotation the method provides with modified properties, or provide a new annotation to represent the map feature. If an annotation doesn’t return, MapKit JS uses the default annotation.

## See Also

### Selecting map features

selectableMapFeatures

An array of map features that users can select from the map.

selectableMapFeatureSelectionAccessory

An accessory for displaying place information when a person selects a map feature.

