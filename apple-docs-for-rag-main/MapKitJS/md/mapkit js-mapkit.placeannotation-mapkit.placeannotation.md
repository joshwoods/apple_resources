

- MapKit JS
- mapkit.PlaceAnnotation
-  mapkit.PlaceAnnotation 

Initializer

# mapkit.PlaceAnnotation

Creates a new place annotation.

MapKit JS 5.78.1+

``` source
new mapkit.PlaceAnnotation(
 mapkit.Coordinate|Place location,
 optional MarkerAnnotationConstructorOptions options
);
```

## Discussion

You’re required to provide a Place object, either by passing it as the first argument or setting place. If you don’t provide the required object, the call throws an error.

## Relationships

### Inherits From

- mapkit.MapFeatureAnnotation

