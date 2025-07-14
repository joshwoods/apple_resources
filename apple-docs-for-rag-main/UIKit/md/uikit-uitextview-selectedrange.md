

- UIKit
- UITextView
-  selectedRange 

Instance Property

# selectedRange

The current selection range of the text view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var selectedRange: NSRange { get set }
```

## Discussion

In iOS 2.2 and earlier, the length of the selection range is always 0, indicating that the selection is actually an insertion point. In iOS 3.0 and later, the length of the selection range may be non-zero.

## See Also

### Working with the selection

func scrollRangeToVisible(NSRange)

Scrolls the text view until the text in the specified range is visible.

var clearsOnInsertion: Bool

A Boolean value that indicates whether inserting text replaces the previous contents.

var isSelectable: Bool

A Boolean value that indicates whether the text view is selectable.

