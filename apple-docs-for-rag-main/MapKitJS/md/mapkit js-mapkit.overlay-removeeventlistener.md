

- MapKit JS
- mapkit.Overlay
-  removeEventListener 

Instance Method

# removeEventListener

Stops listening for the specified type of event.

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

A required string that represents the event type, such as `select`.

`listener`  

The required event listener (function or object that implements the `EventListener` interface) to remove.

`thisObject`  

An optional object set as the `this` keyword on the `listener` function.

## Discussion

Removes `listener` as an event listener for an event of `type`.

| **Event type** | **Summary**                                   |
|----------------|-----------------------------------------------|
| `select`       | The overlay’s `selected` property is `true`.  |
| `deselect`     | The overlay’s `selected` property is `false`. |

## See Also

### Registering event listeners

addEventListener

Starts listening for the specified type of event.

