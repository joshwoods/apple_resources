

- AppKit
- NSScroller
-  testPart(\_:) 

Instance Method

# testPart(\_:)

Returns the part that would be hit by a mouse-down event at `aPoint` (expressed in the window’s coordinate system).

macOS

``` source
@MainActor
func testPart(_ point: NSPoint) -> NSScroller.Part
```

## Discussion

See NSScroller.Part for a list of possible return values. In macOS 10.7 and later, this method no longer returns NSScroller.Part.incrementLine or NSScroller.Part.decrementLine.

Note the interpretations of `NSScrollerDecrementPage` and `NSScrollerIncrementPage`. The actual part of a scroller that causes page-by-page scrolling varies, so as a convenience these part codes refer to useful parts different from the scroll buttons.

## See Also

### Related Documentation

var hitPart: NSScroller.Part

A part code indicating the manner in which the scrolling should be performed.

### Calculating Layout

func rect(for: NSScroller.Part) -> NSRect

Returns the rectangle occupied by `aPart`, which for this method is interpreted literally rather than as an indicator of scrolling direction.

func checkSpaceForParts()

Checks to see if there is enough room in the receiver to display the knob and buttons.

var usableParts: NSScroller.UsableParts

A value that indicates which parts of the receiver are displayed and usable.

