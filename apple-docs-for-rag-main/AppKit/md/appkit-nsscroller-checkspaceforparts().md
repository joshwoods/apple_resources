

- AppKit
- NSScroller
-  checkSpaceForParts() 

Instance Method

# checkSpaceForParts()

Checks to see if there is enough room in the receiver to display the knob and buttons.

macOS

``` source
@MainActor
func checkSpaceForParts()
```

## Discussion

The usableParts property contains the state calculated by this method. You should never need to invoke this method; it’s invoked automatically whenever the scroller’s size changes.

## See Also

### Calculating Layout

func rect(for: NSScroller.Part) -> NSRect

Returns the rectangle occupied by `aPart`, which for this method is interpreted literally rather than as an indicator of scrolling direction.

func testPart(NSPoint) -> NSScroller.Part

Returns the part that would be hit by a mouse-down event at `aPoint` (expressed in the window’s coordinate system).

var usableParts: NSScroller.UsableParts

A value that indicates which parts of the receiver are displayed and usable.

