

- AppKit
- NSScroller
-  trackKnob(with:) 

Instance Method

# trackKnob(with:)

Tracks the knob and sends action messages to the receiver’s target.

macOS

``` source
@MainActor
func trackKnob(with event: NSEvent)
```

## Discussion

This method is invoked automatically when the receiver receives `theEvent` mouse-down event in the knob; you should not invoke it directly.

## See Also

### Event Handling

var hitPart: NSScroller.Part

A part code indicating the manner in which the scrolling should be performed.

func trackScrollButtons(with: NSEvent)

Tracks the scroll buttons and sends action messages to the receiver’s target.

Deprecated

