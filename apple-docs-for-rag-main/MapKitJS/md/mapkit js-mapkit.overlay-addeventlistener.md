

- MapKit JS
- mapkit.Overlay
-  addEventListener 

Instance Method

# addEventListener

Starts listening for the specified type of event.

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

A required string that represents the event type, such as `select`.

`listener`  

The required event listener (function or object that implements the `EventListener` interface) to invoke.

`thisObject`  

An optional object set as the `this` keyword on the `listener` function.

## Discussion

Adds `listener` as an event listener for an event of `type`. Throws an error if `type` is invalid.

| **Event type** | **Summary**                                   |
|----------------|-----------------------------------------------|
| `select`       | The overlay’s `selected` property is `true`.  |
| `deselect`     | The overlay’s `selected` property is `false`. |

## See Also

### Registering event listeners

removeEventListener

Stops listening for the specified type of event.

