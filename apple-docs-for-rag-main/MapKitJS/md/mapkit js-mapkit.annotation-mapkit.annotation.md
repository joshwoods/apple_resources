

- MapKit JS
- mapkit.Annotation
-  mapkit.Annotation 

Initializer

# mapkit.Annotation

Creates a new annotation given its location and initialization options.

MapKit JS 5.0+

``` source
new mapkit.Annotation(
 mapkit.Coordinate|Place location,
 function factory,
 optional AnnotationConstructorOptions options
);
```

## Parameters 

`location`  

The coordinate where the annotation appears.

`factory`  

A factory function that returns a DOM element that represents the annotation.

`options`  

A hash of properties MapKit JS uses to initialize the annotation.

## Return Value

A mapkit.Annotation instance.

## Discussion

The `factory` function returns a DOM element to represent the annotation. It can be a single element or a containing element with subelements. MapKit JS calls this function with the following two arguments:

- `coordinate` (mapkit.Coordinate) — The annotation’s coordinate.

- `options` (AnnotationConstructorOptions) — You can use options you pass to the annotation constructor to add context to the custom annotation.

The `options` include `title` and `subtitle`, which appear in a callout if they’re present.

## Relationships

### Inherits From

- mapkit.ImageAnnotation
- mapkit.MarkerAnnotation

## See Also

### Creating an annotation

AnnotationConstructorOptions

An object that contains options for creating annotation features.

mapkit.Annotation.CollisionMode

Constants that indicate whether an annotation collides and how to interpret the collision-frame rectangle of an annotation view.

mapkit.Annotation.DisplayPriority

Constant values that provide a hint the map uses to prioritize displaying annotations.

addEventListener

Adds an event listener to handle events that user interactions with annotations trigger.

removeEventListener

Removes an event listener.

