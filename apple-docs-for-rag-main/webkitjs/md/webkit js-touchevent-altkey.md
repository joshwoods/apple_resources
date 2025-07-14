

- WebKit JS
- TouchEvent
-  altKey 

Instance Property

# altKey

A Boolean value indicating whether the alt key is pressed.

Safari Desktop 10.1+Safari Mobile 2.0+

``` source
readonly attribute boolean altKey;
```

## Discussion

If `true`, the alt key is pressed; otherwise, it is not. If there is no keyboard, this value is `false`.

## See Also

### Accessing Properties

ctrlKey

A Boolean value indicating whether the control key is pressed.

metaKey

A Boolean value indicating whether the meta key is pressed.

shiftKey

A Boolean value indicating whether the shift key is pressed.

changedTouches

A collection of Touch objects representing all touches that changed in this event.

targetTouches

A collection of Touch objects representing all touches associated with this target.

touches

A collection of Touch objects representing all touches associated with this event.

rotation

The delta rotation since the start of an event in degrees where clockwise is positive and counter-clockwise is negative.

scale

The distance between two fingers since the start of an event as a multiplier of the initial distance.

### Related Documentation

Safari Web Content Guide

