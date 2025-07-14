

- MapKit JS
- mapkit.Annotation
-  addEventListener 

Instance Method

# addEventListener

Adds an event listener to handle events that user interactions with annotations trigger.

MapKit JS 5.0+

``` source
void addEventListener(
 string type,
 function listener,
 optional Object thisObject
);
```

## Parameters 

`type`  

The event type of interest (such as `“select”`).

`listener`  

The callback function to invoke. MapKit JS passes `listener` an annotation event as its sole argument.

`thisObject`  

An object MapKit JS sets as the `this` keyword on the `listener` function.

## Return Value

This method doesn’t return a value.

## Discussion

Adds `listener` as a callback for an event of type `type`. Throws an error if `type` is invalid.

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

removeEventListener

Removes an event listener.

