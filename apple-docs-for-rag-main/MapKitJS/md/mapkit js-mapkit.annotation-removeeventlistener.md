

- MapKit JS
- mapkit.Annotation
-  removeEventListener 

Instance Method

# removeEventListener

Removes an event listener.

MapKit JS 5.0+

``` source
void removeEventListener(
 string type,
 function listener,
 optional Object thisObject
);
```

## Parameters 

`type`  

The event type of interest (such as `“select”`).

`listener`  

The callback function to remove.

`thisObject`  

An object MapKit JS sets as the `this` keyword on the `listener` function.

## Return Value

This method doesn’t return a value.

## Discussion

Removes `listener` as a callback for an event of `type`.

## See Also

### Creating an annotation

mapkit.Annotation

Creates a new annotation given its location and initialization options.

AnnotationConstructorOptions

An object that contains options for creating annotation features.

mapkit.Annotation.CollisionMode

Constants that indicate whether an annotation collides and how to interpret the collision-frame rectangle of an annotation view.

mapkit.Annotation.DisplayPriority

Constant values that provide a hint the map uses to prioritize displaying annotations.

addEventListener

Adds an event listener to handle events that user interactions with annotations trigger.

