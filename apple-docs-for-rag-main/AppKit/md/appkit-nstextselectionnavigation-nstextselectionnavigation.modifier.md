

- AppKit
- NSTextSelectionNavigation
-  NSTextSelectionNavigation.Modifier 

Structure

# NSTextSelectionNavigation.Modifier

Values that describe how the framework handles different kinds of selection modifiers.

macOS 12.0+

``` source
struct Modifier
```

## Topics

### Creating a navigation modifier

init(rawValue: UInt)

Creates a new navigation modifier using a raw value.

### Navigation modifier characteristics

static var extend: NSTextSelectionNavigation.Modifier

The value that indicates the framework extends the selection by not moving the initial location while in a drag selection.

static var multiple: NSTextSelectionNavigation.Modifier

The value that indicates the framework extends the selection visually inside the rectangular area defined by the anchor and dragged positions.

static var visual: NSTextSelectionNavigation.Modifier

The value that indicates the framework extends the selection visually inside the rectangular area defined by the anchor and drag positions.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Selection characteristics

var allowsNonContiguousRanges: Bool

Determines if the instance could produce selections with multiple noncontiguous selections.

var rotatesCoordinateSystemForLayoutOrientation: Bool

Determines if the framework rotates the coordinate system to match the layout orientation.

enum Destination

Values that affect how the framework handles navigation across different textual boundaries during a selection.

enum Direction

Values that describe the direction of a selection.

func textSelection(for: NSTextSelection.Granularity, enclosing: CGPoint, inContainerAt: any NSTextLocation) -> NSTextSelection?

Returns a text selection that expands to the nearest boundaries for selection granularity and an enclosing point you specify.

