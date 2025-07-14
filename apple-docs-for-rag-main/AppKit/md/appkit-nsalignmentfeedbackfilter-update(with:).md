

- AppKit
- NSAlignmentFeedbackFilter
-  update(with:) 

Instance Method

# update(with:)

Informs the feedback filter about a new event.

macOS 10.11+

``` source
func update(with event: NSEvent)
```

## Parameters 

`event`  

An event (NSEvent) to be filtered, which matches an event type returned by the inputEventMask method.

## Discussion

This method informs the feedback filter about a new event to be filtered, which matches an event type returned by the inputEventMask method. Call the `updateWithEvent:` method instead of update(withPanRecognizer:) if you are using a tracking loop controller for event tracking.

## See Also

### Related Documentation

class var inputEventMask: NSEvent.EventTypeMask

Retrieves the event types the filter accepts.

### Informing the Filter About Events

func update(withPanRecognizer: NSPanGestureRecognizer)

Informs the feedback filter about a new pan (drag) gesture recognizer event.

