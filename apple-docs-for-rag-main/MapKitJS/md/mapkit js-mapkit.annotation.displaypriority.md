

- MapKit JS
-  mapkit.Annotation.DisplayPriority 

Enumeration

# mapkit.Annotation.DisplayPriority

Constant values that provide a hint the map uses to prioritize displaying annotations.

MapKit JS 5.0+

``` source
interface mapkit.Annotation.DisplayPriority {
 const number Low;
 const number High;
 const number Required;
};
```

## Topics

### Display priority values

High

A high display priority, with a preset value of 750 out of 1000.

Low

A low display priority, with a preset value of 250 out of 1000.

Required

The highest display priority, with a preset value of 1000 out of 1000.

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

mapkit.Annotation.CollisionMode

Constants that indicate whether an annotation collides and how to interpret the collision-frame rectangle of an annotation view.

