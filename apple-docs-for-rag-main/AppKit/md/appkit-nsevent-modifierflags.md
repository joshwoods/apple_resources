

- AppKit
- NSEvent
-  modifierFlags 

Type Property

# modifierFlags

The currently pressed modifier keys.

macOS 10.6+

``` source
class var modifierFlags: NSEvent.ModifierFlags { get }
```

## Return Value

A mask of the current modifiers using the values in `Modifier Flags`.

## Discussion

This returns the state of devices combined with synthesized events at the moment, independent of which events have been delivered via the event stream.

## See Also

### Getting modifier flags

var modifierFlags: NSEvent.ModifierFlags

An integer bit field that indicates the pressed modifier keys.

struct ModifierFlags

Flags that represent key states in an event object.

