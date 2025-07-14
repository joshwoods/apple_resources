

- MapKit JS
- mapkit.Annotation
-  collisionMode 

Instance Property

# collisionMode

A mode that determines the shape of the collision frame.

MapKit JS 5.0+

``` source
attribute string collisionMode;
```

## Discussion

The collision mode indicates whether the annotation collides, and, if so, the shape of an annotation’s collision frame:

Rectangle  
Indicates the bounding box of the annotation.

Circle  
Indicates a circle within the bounding box.

None  
Indicates the annotation doesn’t collide with other annotations.

The default value is Rectangle.

## See Also

### Managing clustering

memberAnnotations

An array of annotations that the framework groups together in a cluster.

clusteringIdentifier

An identifier for grouping annotations into the same cluster.

mapkit.Annotation.CollisionMode

Constants that indicate whether an annotation collides and how to interpret the collision-frame rectangle of an annotation view.

