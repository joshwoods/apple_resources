

- AppKit
- NSTextFinderClient
-  allowsMultipleSelection 

Instance Property

# allowsMultipleSelection

Returns whether multiple items can be selected.

macOS

``` source
optional var allowsMultipleSelection: Bool { get }
```

## Discussion

If this properties is not implemented, the text finder will act as if they returned true.

## See Also

### Selection Information

var isSelectable: Bool

Returns whether the text is selectable.

var firstSelectedRange: NSRange

Returns the currently selected range.

var selectedRanges: [NSValue]

Returns an array of selected ranges.

