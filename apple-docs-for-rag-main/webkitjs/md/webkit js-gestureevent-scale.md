

- WebKit JS
- GestureEvent
-  scale 

Instance Property

# scale

The distance between two fingers since the start of an event, as a multiplier of the initial distance.

Safari Desktop 10.1+Safari Mobile 2.0+

``` source
readonly attribute float scale;
```

## Discussion

The initial value is `1.0`. If less than `1.0`, the gesture is pinch close (to zoom out). If greater than `1.0`, the gesture is pinch open (to zoom in).

## See Also

### Accessing Properties

altKey

A Boolean value indicating whether the alt key is pressed.

ctrlKey

A Boolean value indicating whether the control key is pressed.

metaKey

A Boolean value indicating whether the meta key is pressed.

rotation

The delta rotation since the start of an event, in degrees, where clockwise is positive and counter-clockwise is negative.

shiftKey

A Boolean value indicating whether the shift key is pressed.

target

The target of this gesture.

