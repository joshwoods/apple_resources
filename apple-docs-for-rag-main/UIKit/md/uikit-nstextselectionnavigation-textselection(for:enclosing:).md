

- UIKit
- NSTextSelectionNavigation
-  textSelection(for:enclosing:) 

Instance Method

# textSelection(for:enclosing:)

Returns a text selection expanded to the nearest boundaries for the selection granularity and enclosing text selection text ranges you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func textSelection(
    for selectionGranularity: NSTextSelection.Granularity,
    enclosing textSelection: NSTextSelection
) -> NSTextSelection
```

## Parameters 

`selectionGranularity`  

One of the available NSTextSelection.Granularity options.

`textSelection`  

The text selection that describes the text range of interest.

## Return Value

A new text selection.

## See Also

### Working with text selections

func textSelections(interactingAt: CGPoint, inContainerAt: any NSTextLocation, anchors: [NSTextSelection], modifiers: NSTextSelectionNavigation.Modifier, selecting: Bool, bounds: CGRect) -> [NSTextSelection]

Returns an array of text selections produced by a tap or click at the point you specify.

func destinationSelection(for: NSTextSelection, direction: NSTextSelectionNavigation.Direction, destination: NSTextSelectionNavigation.Destination, extending: Bool, confined: Bool) -> NSTextSelection?

Returns a new selection that results from applying the navigation operations you specify to the text selection you provide.

