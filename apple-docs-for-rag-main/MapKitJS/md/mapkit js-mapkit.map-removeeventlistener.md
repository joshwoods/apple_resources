

- MapKit JS
- mapkit.Map
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

The type of event to remove.

`listener`  

The callback function removed.

`thisObject`  

An object set as `this` keyword on the `listener` function.

## Return Value

This method does not return a value.

## Discussion

removeEventListener removes `listener` as a callback for the specified event type. See Handling map events for a list of event types.

## See Also

### Handling map events

Handling map events

Register an event lister for events that a map object dispatches.

addEventListener

Adds an event listener to handle events that user interactions and the framework trigger.

