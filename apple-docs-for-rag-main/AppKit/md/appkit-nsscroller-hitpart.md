

- AppKit
- NSScroller
-  hitPart 

Instance Property

# hitPart

A part code indicating the manner in which the scrolling should be performed.

macOS

``` source
@MainActor
var hitPart: NSScroller.Part { get }
```

## Discussion

This method is typically invoked by an NSScrollView object to determine how to scroll its document view when it receives an action message from the scroller.

See NSScroller.Part for a list of part codes. In macOS 10.7 and later, this method no longer returns NSScroller.Part.incrementLine or NSScroller.Part.decrementLine.

## See Also

### Event Handling

func trackKnob(with: NSEvent)

Tracks the knob and sends action messages to the receiver’s target.

func trackScrollButtons(with: NSEvent)

Tracks the scroll buttons and sends action messages to the receiver’s target.

Deprecated

