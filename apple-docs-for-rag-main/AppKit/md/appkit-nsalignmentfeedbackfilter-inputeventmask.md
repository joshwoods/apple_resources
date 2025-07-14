

- AppKit
- NSAlignmentFeedbackFilter
-  inputEventMask 

Type Property

# inputEventMask

Retrieves the event types the filter accepts.

macOS 10.11+

``` source
class var inputEventMask: NSEvent.EventTypeMask { get }
```

## Discussion

This method retrieves the event types that the filter accepts. This information may be used by an event tracking loop to watch for events that can be passed to the filter.

## See Also

### Related Documentation

class NSEvent

An object that contains information about an input action, such as a mouse click or a key press.

