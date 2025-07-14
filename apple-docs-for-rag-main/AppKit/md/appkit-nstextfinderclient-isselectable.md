

- AppKit
- NSTextFinderClient
-  isSelectable 

Instance Property

# isSelectable

Returns whether the text is selectable.

macOS

``` source
optional var isSelectable: Bool { get }
```

## Discussion

If this properties is not implemented, the text finder will act as if they returned true.

## See Also

### Selection Information

var allowsMultipleSelection: Bool

Returns whether multiple items can be selected.

var firstSelectedRange: NSRange

Returns the currently selected range.

var selectedRanges: [NSValue]

Returns an array of selected ranges.

