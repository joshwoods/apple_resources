

- MapKit JS
- AnnotationConstructorOptions
-  clusteringIdentifier 

Instance Property

# clusteringIdentifier

An identifier for grouping annotations into the same cluster.

MapKit JS 5.0+

``` source
attribute string clusteringIdentifier;
```

## Discussion

When zooming out on a map that contains many annotations, MapKit JS groups the colliding annotations based on a clustering identifier value.

The default value is `null`.

For more information, see Clustering annotations.

## See Also

### Grouping annotations

collisionMode

A mode that determines the shape of the collision frame.

id

A Place ID that uniquely identifies a feature.

