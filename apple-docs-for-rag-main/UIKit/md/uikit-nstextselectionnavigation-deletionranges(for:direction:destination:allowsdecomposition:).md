

- UIKit
- NSTextSelectionNavigation
-  deletionRanges(for:direction:destination:allowsDecomposition:) 

Instance Method

# deletionRanges(for:direction:destination:allowsDecomposition:)

Returns the ranges for deleting the text based on the current selection and movement arguments.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
func deletionRanges(
    for textSelection: NSTextSelection,
    direction: NSTextSelectionNavigation.Direction,
    destination: NSTextSelectionNavigation.Destination,
    allowsDecomposition: Bool
) -> [NSTextRange]
```

## Parameters 

`textSelection`  

The text selection.

`direction`  

The NSTextSelectionNavigation.Direction to consider when calculating the deletion ranges.

`destination`  

The NSTextSelectionNavigation.Destination that describes the scope of the text selection to consider when calculating the deletion ranges.

`allowsDecomposition`  

A Boolean value that determines if this method operates on composite characters which may be present depending on the characteristics of the script used by `textSelection`.

## Return Value

An array of text ranges to delete.

## Discussion

The selection after deletion contains a zero-length range starting at the location of the first range returned. The framework ignores the destination when `textSelection` has a non-empty selection. The `allowsDecomposition` parameter only applies to the NSTextSelectionNavigation.Direction.backward direction and NSTextSelectionNavigation.Destination.character with a zero-length selection.

