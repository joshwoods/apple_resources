

- WebKit JS
- TouchEvent
-  changedTouches 

Instance Property

# changedTouches

A collection of Touch objects representing all touches that changed in this event.

Safari Desktop 10.1+Safari Mobile 2.0+

``` source
readonly attribute TouchList? changedTouches;
```

## Discussion

You manipulate this collection using TouchList methods.

## See Also

### Accessing Properties

altKey

A Boolean value indicating whether the alt key is pressed.

ctrlKey

A Boolean value indicating whether the control key is pressed.

metaKey

A Boolean value indicating whether the meta key is pressed.

shiftKey

A Boolean value indicating whether the shift key is pressed.

targetTouches

A collection of Touch objects representing all touches associated with this target.

touches

A collection of Touch objects representing all touches associated with this event.

rotation

The delta rotation since the start of an event in degrees where clockwise is positive and counter-clockwise is negative.

scale

The distance between two fingers since the start of an event as a multiplier of the initial distance.

