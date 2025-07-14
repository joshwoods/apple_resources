

- UIKit
- NSTextSelectionNavigation
-  NSTextSelectionNavigation.Direction 

Enumeration

# NSTextSelectionNavigation.Direction

Values that describe the direction of a selection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
enum Direction
```

## Topics

### Navigation directions

case forward

The value that represents a logical forward selection based on the flow of text stored in the document.

case backward

The value that represents a backward selection based on the flow of text stored in the document.

case left

The value that represents a selection in the left direction along the current line.

case right

The value that represents a selection in the right direction along the current line.

case up

The value that represents a selection in the up direction, above the current line.

case down

The value that represents a selection in the down direction, below the current line.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Selection characteristics

var allowsNonContiguousRanges: Bool

Determines if the instance could produce selections with multiple noncontiguous selections.

var rotatesCoordinateSystemForLayoutOrientation: Bool

Determines if the framework rotates the coordinate system to match the layout orientation.

struct Modifier

Values that describe how the framework handles different kinds of selection modifiers.

enum Destination

Values that affect how the framework handles navigation across different textual boundaries during a selection.

func textSelection(for: NSTextSelection.Granularity, enclosing: CGPoint, inContainerAt: any NSTextLocation) -> NSTextSelection?

Returns a text selection that expands to the nearest boundaries for selection granularity and an enclosing point you specify.

