

- AppKit
- NSTextFinderClient
-  firstSelectedRange 

Instance Property

# firstSelectedRange

Returns the currently selected range.

macOS

``` source
optional var firstSelectedRange: NSRange { get }
```

## Discussion

This property is required for the next match, previous match, replace, replace and find and set search string actions. The client should return its first selected range, or {index, 0} to indicate the location of the insertion point if there is no selection.

## See Also

### Selection Information

var isSelectable: Bool

Returns whether the text is selectable.

var allowsMultipleSelection: Bool

Returns whether multiple items can be selected.

var selectedRanges: [NSValue]

Returns an array of selected ranges.

