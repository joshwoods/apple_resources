

- AppKit
- NSTextFinderClient
-  selectedRanges 

Instance Property

# selectedRanges

Returns an array of selected ranges.

macOS

``` source
optional var selectedRanges: [NSValue] { get set }
```

## Discussion

This property is required for the replace all in selection, select all, and select all in selection actions. The returned `NSArray` object should contain `NSRanges` wrapped by `NSValues`.

## See Also

### Selection Information

var isSelectable: Bool

Returns whether the text is selectable.

var allowsMultipleSelection: Bool

Returns whether multiple items can be selected.

var firstSelectedRange: NSRange

Returns the currently selected range.

