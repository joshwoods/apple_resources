

- AppKit
- NSScroller
-  usableParts 

Instance Property

# usableParts

A value that indicates which parts of the receiver are displayed and usable.

macOS

``` source
@MainActor
var usableParts: NSScroller.UsableParts { get }
```

## Discussion

See NSScroller.UsableParts for a list of possible values.

## See Also

### Related Documentation

var arrowsPosition: NSScroller.ArrowPosition

The location of the scroll buttons within the scroller, as described in NSScroller.ArrowPosition.

Deprecated

### Calculating Layout

func rect(for: NSScroller.Part) -> NSRect

Returns the rectangle occupied by `aPart`, which for this method is interpreted literally rather than as an indicator of scrolling direction.

func testPart(NSPoint) -> NSScroller.Part

Returns the part that would be hit by a mouse-down event at `aPoint` (expressed in the window’s coordinate system).

func checkSpaceForParts()

Checks to see if there is enough room in the receiver to display the knob and buttons.

