

- MapKit JS
- mapkit.Map
-  removeAnnotations 

Instance Method

# removeAnnotations

Removes multiple annotations from the map.

MapKit JS 5.0+

``` source
mapkit.Annotation[] removeAnnotations(
 mapkit.Annotation[] annotations
);
```

## Parameters 

`annotations`  

An array of annotations to remove.

## Return Value

Returns the array of annotations.

## See Also

### Annotating the map

annotations

An array of all the annotations on the map.

selectedAnnotation

The selected annotation.

annotationForCluster

A delegate method for modifying an annotation that represents a group of annotations that the framework combines into a cluster.

annotationsInMapRect

Returns the list of annotation objects within the specified map rectangle.

addAnnotation

Adds an annotation to the map.

addAnnotations

Adds an array of annotations to the map.

removeAnnotation

Removes an annotation from the map.

