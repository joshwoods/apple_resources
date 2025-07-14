

- AppKit
- NSTextSelectionNavigation
-  rotatesCoordinateSystemForLayoutOrientation 

Instance Property

# rotatesCoordinateSystemForLayoutOrientation

Determines if the framework rotates the coordinate system to match the layout orientation.

macOS 12.0+

``` source
var rotatesCoordinateSystemForLayoutOrientation: Bool { get set }
```

## Discussion

If set to `true`, the framework rotates the coordinate system for arguments passed to the navigation methods such as textSelections(interactingAt:inContainerAt:anchors:modifiers:selecting:bounds:): based on the text container layout orientation. Defaults to `false`.

## See Also

### Selection characteristics

var allowsNonContiguousRanges: Bool

Determines if the instance could produce selections with multiple noncontiguous selections.

struct Modifier

Values that describe how the framework handles different kinds of selection modifiers.

enum Destination

Values that affect how the framework handles navigation across different textual boundaries during a selection.

enum Direction

Values that describe the direction of a selection.

func textSelection(for: NSTextSelection.Granularity, enclosing: CGPoint, inContainerAt: any NSTextLocation) -> NSTextSelection?

Returns a text selection that expands to the nearest boundaries for selection granularity and an enclosing point you specify.

