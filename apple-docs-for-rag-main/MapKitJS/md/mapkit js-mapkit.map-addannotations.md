

- MapKit JS
- mapkit.Map
-  addAnnotations 

Instance Method

# addAnnotations

Adds an array of annotations to the map.

MapKit JS 5.0+

``` source
mapkit.Annotation[] addAnnotations(
 mapkit.Annotation[] annotations
);
```

## Parameters 

`annotations`  

An array of annotations to add.

## Return Value

Returns the array of annotations.

## Discussion

The map shows annotations that have their animates property set to `true` in a staggered manner, in order of latitude.

Note

MapKitJS immediately adds the annotations to the annotations array, then visually displays them on the map.

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

removeAnnotation

Removes an annotation from the map.

removeAnnotations

Removes multiple annotations from the map.

