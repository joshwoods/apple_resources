

- MapKit JS
- mapkit.Map
-  selectedAnnotation 

Instance Property

# selectedAnnotation

The selected annotation.

MapKit JS 5.0+

``` source
attribute mapkit.Annotation selectedAnnotation;
```

## Discussion

The value of selectedAnnotation is either a mapkit.Annotation object, if the user selects one, or `null` if there aren’t any selected annotations.

An annotation is in a selected state if its selected property is `true`. To deselect all annotations, set this attribute to `null`.

To select an annotation that’s already part of the map, set this attribute to the desired annotation.

When MapKit JS removes the selected annotation from the map (as an effect of removeAnnotation, removeAnnotations, or setting a new set of annotations with the annotations property), MapKit JS deselects it before removing it.

## See Also

### Annotating the map

annotations

An array of all the annotations on the map.

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

