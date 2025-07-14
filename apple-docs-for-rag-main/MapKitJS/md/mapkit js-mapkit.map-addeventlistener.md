

- MapKit JS
- mapkit.Map
-  addEventListener 

Instance Method

# addEventListener

Adds an event listener to handle events that user interactions and the framework trigger.

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

The event type of interest (such as “`select”`).

`listener`  

The callback function that MapKit invokes. MapKit JS passes `listener` to a mapkit.Map event as its sole argument.

`thisObject`  

An object MapKit JS sets as the `this` keyword on the `listener` function.

## Return Value

This method doesn’t return a value.

## Discussion

addEventListener adds `listener` as a callback when an event of type `type` occurs. It throws an error if `type` is invalid. See Handling map events for a list of event types.

The following is an example of adding an event listener for a region change:

```
map.addEventListener("region-change-start", function(event) {
    console.log("Region Change Started");
});
```

## See Also

### Handling map events

Handling map events

Register an event lister for events that a map object dispatches.

removeEventListener

Removes an event listener.

