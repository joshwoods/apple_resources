

- AppKit
- NSTextSelectionNavigation
-  destinationSelection(for:direction:destination:extending:confined:) 

Instance Method

# destinationSelection(for:direction:destination:extending:confined:)

Returns a new selection that results from applying the navigation operations you specify to the text selection you provide.

macOS 12.0+

``` source
func destinationSelection(
    for textSelection: NSTextSelection,
    direction: NSTextSelectionNavigation.Direction,
    destination: NSTextSelectionNavigation.Destination,
    extending: Bool,
    confined: Bool
) -> NSTextSelection?
```

## Parameters 

`textSelection`  

The source selection.

`direction`  

One of the available NSTextSelectionNavigation.Direction directions.

`destination`  

One of the available NSTextSelectionNavigation.Destination destinations.

`extending`  

Whether this selection extends an existing selection.

`confined`  

Whether to confine movement to the existing selection.

## Return Value

A new NSTextSelection, or `nil` if the operation doesn’t produce a logically valid result.

## Discussion

If `confined` is `true`, confine any movement to the text element that the selection already lies within.

## See Also

### Working with text selections

func textSelection(for: NSTextSelection.Granularity, enclosing: NSTextSelection) -> NSTextSelection

Returns a text selection expanded to the nearest boundaries for the selection granularity and enclosing text selection text ranges you specify.

func textSelections(interactingAt: CGPoint, inContainerAt: any NSTextLocation, anchors: [NSTextSelection], modifiers: NSTextSelectionNavigation.Modifier, selecting: Bool, bounds: CGRect) -> [NSTextSelection]

Returns an array of text selections produced by a tap or click at the point you specify.

