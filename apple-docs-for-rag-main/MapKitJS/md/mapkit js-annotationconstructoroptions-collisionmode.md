

- MapKit JS
- AnnotationConstructorOptions
-  collisionMode 

Instance Property

# collisionMode

A mode that determines the shape of the collision frame.

MapKit JS 5.0+

``` source
attribute string collisionMode;
```

## Discussion

Use one of the modes available in mapkit.Annotation.CollisionMode:

- `mapkit.Annotation.CollisionMode.Rectangle` — Indicates the bounding box of the annotation.

- `mapkit.Annotation.CollisionMode.Circle` — Indicates a circle within the bounding box.

The default value is `Annotation.CollisionMode.Rectangle`.

## See Also

### Grouping annotations

clusteringIdentifier

An identifier for grouping annotations into the same cluster.

id

A Place ID that uniquely identifies a feature.

