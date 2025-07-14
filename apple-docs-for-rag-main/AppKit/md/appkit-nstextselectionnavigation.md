

- AppKit
-  NSTextSelectionNavigation 

Class

# NSTextSelectionNavigation

An interface you use to expose methods for obtaining results from actions performed on text selections.

macOS 12.0+

``` source
class NSTextSelectionNavigation
```

## Topics

### Creating a selection navigation

init(dataSource: any NSTextSelectionDataSource)

Creates a new object using the text selection data source you provide.

### Selection characteristics

var allowsNonContiguousRanges: Bool

Determines if the instance could produce selections with multiple noncontiguous selections.

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

### Accessing the data source

var textSelectionDataSource: (any NSTextSelectionDataSource)?

The data source associated with this selection navigation.

protocol NSTextSelectionDataSource

A set of methods that objects implement to provide data for, and manage text selections.

### Working with text selections

func textSelection(for: NSTextSelection.Granularity, enclosing: NSTextSelection) -> NSTextSelection

Returns a text selection expanded to the nearest boundaries for the selection granularity and enclosing text selection text ranges you specify.

func textSelections(interactingAt: CGPoint, inContainerAt: any NSTextLocation, anchors: [NSTextSelection], modifiers: NSTextSelectionNavigation.Modifier, selecting: Bool, bounds: CGRect) -> [NSTextSelection]

Returns an array of text selections produced by a tap or click at the point you specify.

func destinationSelection(for: NSTextSelection, direction: NSTextSelectionNavigation.Direction, destination: NSTextSelectionNavigation.Destination, extending: Bool, confined: Bool) -> NSTextSelection?

Returns a new selection that results from applying the navigation operations you specify to the text selection you provide.

### Controlling cache behavior

func flushLayoutCache()

Flushes cached layout information.

### Finding the insertion point

func resolvedInsertionLocation(for: NSTextSelection, writingDirection: NSTextSelectionNavigation.WritingDirection) -> (any NSTextLocation)?

Returns the location for inserting the next input depending on the state of the current and secondary selections.

### Specifying deletion ranges

func deletionRanges(for: NSTextSelection, direction: NSTextSelectionNavigation.Direction, destination: NSTextSelectionNavigation.Destination, allowsDecomposition: Bool) -> [NSTextRange]

Returns the ranges for deleting the text based on the current selection and movement arguments.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Location and selection

class NSTextRange

A class that represents a contiguous range between two locations inside document contents.

class NSTextSelection

A class that represents a single logical selection context that corresponds to an insertion point.

protocol NSTextLocation

An interface you implement that represents an abstract location inside your document’s content.

