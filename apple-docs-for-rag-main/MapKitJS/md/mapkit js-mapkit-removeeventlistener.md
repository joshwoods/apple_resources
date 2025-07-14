

- MapKit JS
- mapkit
-  removeEventListener 

Instance Method

# removeEventListener

Unsubscribes a listener function from an event type.

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

The type of event (for example, `“configuration-change”`).

`listener`  

The callback function to remove.

`thisObject`  

An object MapKit JS sets as the `this` keyword on the `listener` function.

## Mentioned in 

Adding interactivity to overlays

## See Also

### Initialization

Handling initialization events

Respond to events that trigger when MapKit JS initializes.

init

Initializes MapKit JS by providing an authorization callback function and optional language.

MapKitInitOptions

Initialization options for MapKit JS.

Libraries

The list of available libraries.

loadedLibraries

A string that describes the list of loaded libraries.

load

Tells MapKit JS which libraries to load.

addEventListener

Subscribes a listener function to an event type.

