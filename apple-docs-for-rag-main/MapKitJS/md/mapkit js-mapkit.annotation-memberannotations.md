

- MapKit JS
- mapkit.Annotation
-  memberAnnotations 

Instance Property

# memberAnnotations

An array of annotations that the framework groups together in a cluster.

MapKit JS 5.0+

``` source
attribute mapkit.Annotation[] memberAnnotations;
```

## Mentioned in 

Clustering annotations

## Discussion

The memberAnnotations array contains all of the annotations that MapKit JS groups together in a cluster. This is a flat array. If there are multiple clusters of annotations, this array contains all of the individual annotations within those clusters; it doesn’t contain any cluster annotations.

## See Also

### Managing clustering

clusteringIdentifier

An identifier for grouping annotations into the same cluster.

collisionMode

A mode that determines the shape of the collision frame.

mapkit.Annotation.CollisionMode

Constants that indicate whether an annotation collides and how to interpret the collision-frame rectangle of an annotation view.

