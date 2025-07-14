

- AppKit
- NSTextSelectionNavigation
-  resolvedInsertionLocation(for:writingDirection:) 

Instance Method

# resolvedInsertionLocation(for:writingDirection:)

Returns the location for inserting the next input depending on the state of the current and secondary selections.

macOS 12.0+

``` source
func resolvedInsertionLocation(
    for textSelection: NSTextSelection,
    writingDirection: NSTextSelectionNavigation.WritingDirection
) -> (any NSTextLocation)?
```

## Parameters 

`textSelection`  

The text selection.

`writingDirection`  

The NSTextSelectionNavigation.WritingDirection direction.

## Return Value

Returns an `NSTextLocation` when the `textSelection.isLogical = false AND` `secondarySelectionLocation != nil`. Otherwise, returns nil.

