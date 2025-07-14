

- AppKit
- NSTextSelectionNavigation
-  NSTextSelectionNavigation.Destination 

Enumeration

# NSTextSelectionNavigation.Destination

Values that affect how the framework handles navigation across different textual boundaries during a selection.

macOS 12.0+

``` source
enum Destination
```

## Topics

### Selection destinations

case character

The selection moves to the next extended grapheme cluster boundary.

case word

The selection moves to the next word boundary ignoring punctuation, whitespace, and format characters preceding the next word.

case line

The selection moves to the next line boundary.

case sentence

The selection moves to the next sentence boundary, ignoring punctuation, whitespace, and format characters preceding the next sentence.

case paragraph

The selection moves to the next paragraph boundary, ignoring the end of line elastic characters and paragraph separators.

case container

The selection moves to the next container or page boundary after boundary of the current container, ignoring the end of line elastic characters.

case document

The selection moves to the document boundary.

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

enum Direction

Values that describe the direction of a selection.

func textSelection(for: NSTextSelection.Granularity, enclosing: CGPoint, inContainerAt: any NSTextLocation) -> NSTextSelection?

Returns a text selection that expands to the nearest boundaries for selection granularity and an enclosing point you specify.

