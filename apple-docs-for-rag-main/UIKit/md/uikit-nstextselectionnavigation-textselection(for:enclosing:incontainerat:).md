

- UIKit
- NSTextSelectionNavigation
-  textSelection(for:enclosing:inContainerAt:) 

Instance Method

# textSelection(for:enclosing:inContainerAt:)

Returns a text selection that expands to the nearest boundaries for selection granularity and an enclosing point you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func textSelection(
    for selectionGranularity: NSTextSelection.Granularity,
    enclosing point: CGPoint,
    inContainerAt location: any NSTextLocation
) -> NSTextSelection?
```

## Parameters 

`selectionGranularity`  

One of the available NSTextSelection.Granularity options.

`point`  

The point that encloses the text.

`location`  

An NSTextLocation that describes the container.

## Return Value

A new `NSTextSelection`, or `nil` if the text selection is not found.

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

enum Direction

Values that describe the direction of a selection.

