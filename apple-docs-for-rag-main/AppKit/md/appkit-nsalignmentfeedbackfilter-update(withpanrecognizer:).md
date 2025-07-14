

- AppKit
- NSAlignmentFeedbackFilter
-  update(withPanRecognizer:) 

Instance Method

# update(withPanRecognizer:)

Informs the feedback filter about a new pan (drag) gesture recognizer event.

macOS 10.11+

``` source
func update(withPanRecognizer panRecognizer: NSPanGestureRecognizer)
```

## Parameters 

`panRecognizer`  

The gesture recognizer (NSPanGestureRecognizer) that produced the event.

## Discussion

This method informs the feedback filter about a new pan (drag) gesture recognizer event. Call this method instead of update(with:) if your event tracking uses gesture recognizers.

## See Also

### Related Documentation

class NSGestureRecognizer

An object that monitors events and calls its action method when a predefined sequence of events occur.

class NSPanGestureRecognizer

A continuous gesture recognizer for panning gestures.

### Informing the Filter About Events

func update(with: NSEvent)

Informs the feedback filter about a new event.

