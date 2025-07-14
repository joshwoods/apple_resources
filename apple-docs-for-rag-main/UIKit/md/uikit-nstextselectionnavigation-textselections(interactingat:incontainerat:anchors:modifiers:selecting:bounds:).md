

- UIKit
- NSTextSelectionNavigation
-  textSelections(interactingAt:inContainerAt:anchors:modifiers:selecting:bounds:) 

Instance Method

# textSelections(interactingAt:inContainerAt:anchors:modifiers:selecting:bounds:)

Returns an array of text selections produced by a tap or click at the point you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func textSelections(
    interactingAt point: CGPoint,
    inContainerAt containerLocation: any NSTextLocation,
    anchors: [NSTextSelection],
    modifiers: NSTextSelectionNavigation.Modifier,
    selecting: Bool,
    bounds: CGRect
) -> [NSTextSelection]
```

## Parameters 

`point`  

A `CGPoint` that represents the location of the tap or click.

`containerLocation`  

A `NSTextLocation that describes the contasiner location`.

`anchors`  

An array of `NSTextSelection` objects.

`modifiers`  

One or more NSTextSelectionNavigation.Modifier options.

`selecting`  

A Boolean value that indicates if the selection is in drag session.

`bounds`  

A `CGRect` that defines the view area in the container’s coordinate system that can interact with events.

## Return Value

An array of text selections.

## See Also

### Working with text selections

func textSelection(for: NSTextSelection.Granularity, enclosing: NSTextSelection) -> NSTextSelection

Returns a text selection expanded to the nearest boundaries for the selection granularity and enclosing text selection text ranges you specify.

func destinationSelection(for: NSTextSelection, direction: NSTextSelectionNavigation.Direction, destination: NSTextSelectionNavigation.Destination, extending: Bool, confined: Bool) -> NSTextSelection?

Returns a new selection that results from applying the navigation operations you specify to the text selection you provide.

