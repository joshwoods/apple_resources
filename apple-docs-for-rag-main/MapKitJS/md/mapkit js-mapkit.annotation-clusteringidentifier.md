

- MapKit JS
- mapkit.Annotation
-  clusteringIdentifier 

Instance Property

# clusteringIdentifier

An identifier for grouping annotations into the same cluster.

MapKit JS 5.0+

``` source
attribute string clusteringIdentifier;
```

## Mentioned in 

Clustering annotations

MapKit JS 5

## Discussion

For MapKit JS to cluster annotations, an annotation needs a `clusteringIdentifie`r. When annotations collide and have the same `clusteringIdentifier`, MapKit JS clusters them together.

The default value is `null`.

For more details, see Clustering annotations.

## See Also

### Managing clustering

memberAnnotations

An array of annotations that the framework groups together in a cluster.

collisionMode

A mode that determines the shape of the collision frame.

mapkit.Annotation.CollisionMode

Constants that indicate whether an annotation collides and how to interpret the collision-frame rectangle of an annotation view.

