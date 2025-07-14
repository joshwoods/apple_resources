

- UIKit
- NSTextSelectionNavigation
-  allowsNonContiguousRanges 

Instance Property

# allowsNonContiguousRanges

Determines if the instance could produce selections with multiple noncontiguous selections.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var allowsNonContiguousRanges: Bool { get set }
```

## See Also

### Selection characteristics

var rotatesCoordinateSystemForLayoutOrientation: Bool

Determines if the framework rotates the coordinate system to match the layout orientation.

struct Modifier

Values that describe how the framework handles different kinds of selection modifiers.

enum Destination

Values that affect how the framework handles navigation across different textual boundaries during a selection.

enum Direction

Values that describe the direction of a selection.

func textSelection(for: NSTextSelection.Granularity, enclosing: CGPoint, inContainerAt: any NSTextLocation) -> NSTextSelection?

Returns a text selection that expands to the nearest boundaries for selection granularity and an enclosing point you specify.

