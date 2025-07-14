

- MapKit JS
- mapkit.TileOverlay
-  removeEventListener 

Instance Method

# removeEventListener

Stops listening for events of the specified type.

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

The required event type, such as `tile-error`.

`listener`  

The required event listener function or delegate object to invoke.

`thisObject`  

An optional object set as the `this` keyword on the listener function.

## Discussion

Removes `listener` as a callback for an event of `type`.

| **Event type** | **Summary** |
|----|----|
| `tile-error` | For each tile load failure, MapKit JS dispatches a `tile-error` event with two properties:  • `tileOverlay`: the tile overlay containing the failing tile.  • `tileUrl`: the specific tile URL string that failed. |

## See Also

### Registering event listeners

addEventListener

Listens for events of the specified type.

