

- AppKit
- NSScroller
-  trackScrollButtons(with:) Deprecated

Instance Method

# trackScrollButtons(with:)

Tracks the scroll buttons and sends action messages to the receiver’s target.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func trackScrollButtons(with event: NSEvent)
```

Deprecated

Not invoked since 10.7

## Discussion

This method is invoked automatically when the receiver receives `theEvent` mouse-down event in a scroll button; you should not invoke this method directly.

### Special Considerations

This method is not invoked in macOS 10.7 and later.

## See Also

### Event Handling

var hitPart: NSScroller.Part

A part code indicating the manner in which the scrolling should be performed.

func trackKnob(with: NSEvent)

Tracks the knob and sends action messages to the receiver’s target.

