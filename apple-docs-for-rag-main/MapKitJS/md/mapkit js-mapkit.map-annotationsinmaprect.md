

- MapKit JS
- mapkit.Map
-  annotationsInMapRect 

Instance Method

# annotationsInMapRect

Returns the list of annotation objects within the specified map rectangle.

MapKit JS 5.0+

``` source
mapkit.Annotation[] annotationsInMapRect(
 mapkit.MapRect mapRect
);
```

## Parameters 

`mapRect`  

The portion of the map in which to look for annotations.

## Return Value

Returns an array of annotations that fall inside `mapRect`.

## Mentioned in 

MapKit JS 5

## See Also

### Annotating the map

annotations

An array of all the annotations on the map.

selectedAnnotation

The selected annotation.

annotationForCluster

A delegate method for modifying an annotation that represents a group of annotations that the framework combines into a cluster.

addAnnotation

Adds an annotation to the map.

addAnnotations

Adds an array of annotations to the map.

removeAnnotation

Removes an annotation from the map.

removeAnnotations

Removes multiple annotations from the map.

