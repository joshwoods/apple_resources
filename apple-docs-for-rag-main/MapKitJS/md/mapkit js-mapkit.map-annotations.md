

- MapKit JS
- mapkit.Map
-  annotations 

Instance Property

# annotations

An array of all the annotations on the map.

MapKit JS 5.0+

``` source
attribute mapkit.Annotation[] annotations;
```

## Mentioned in 

Clustering annotations

MapKit JS 5

## Discussion

You can set this attribute to a new (possibly empty) array of annotations, which updates all the annotations on the map.

## See Also

### Annotating the map

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

removeAnnotations

Removes multiple annotations from the map.

