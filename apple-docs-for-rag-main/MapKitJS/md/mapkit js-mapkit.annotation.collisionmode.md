

- MapKit JS
-  mapkit.Annotation.CollisionMode 

Enumeration

# mapkit.Annotation.CollisionMode

Constants that indicate whether an annotation collides and how to interpret the collision-frame rectangle of an annotation view.

MapKit JS 5.0+

``` source
interface mapkit.Annotation.CollisionMode {
 const string Rectangle;
 const string Circle;
 const String None;
};
```

## Topics

### Collision modes

Rectangle

A constant indicating that the map should use a full collision rectangle for detecting collisions.

Circle

A constant indicating that the map should use a circle inscribed in the collision frame rectangle to determine collisions.

None

A constant that indicates the annotation doesn’t collide with other annotations.

## See Also

### Annotations

Clustering annotations

Combine multiple annotations into a single clustered annotation.

mapkit.Annotation

The base annotation object for creating custom annotations.

AnnotationCalloutDelegate

Methods for customizing the behavior and appearance of an annotation callout.

mapkit.PlaceAnnotation

An annotation for a place.

mapkit.MapFeatureAnnotation

An object that represents a map feature that the user selects.

mapkit.Annotation.DisplayPriority

Constant values that provide a hint the map uses to prioritize displaying annotations.

