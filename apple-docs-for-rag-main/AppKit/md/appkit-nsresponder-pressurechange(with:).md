

- AppKit
- NSResponder
-  pressureChange(with:) 

Instance Method

# pressureChange(with:)

Indicates a pressure change as the result of a user input event on a system that supports pressure sensitivity.

macOS 10.10.3+

``` source
@MainActor
func pressureChange(with event: NSEvent)
```

## Parameters 

`event`  

An `NSEvent` object encapsulating information about the event that invoked the change in pressure.

## Discussion

This method is invoked automatically in response to user actions. `event` is the event that initiated the change in pressure.

## See Also

### Related Documentation

class NSEvent

An object that contains information about an input action, such as a mouse click or a key press.

