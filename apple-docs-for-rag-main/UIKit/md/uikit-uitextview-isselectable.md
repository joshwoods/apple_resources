

- UIKit
- UITextView
-  isSelectable 

Instance Property

# isSelectable

A Boolean value that indicates whether the text view is selectable.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isSelectable: Bool { get set }
```

## Discussion

This property controls the ability of the user to select content and interact with URLs and text attachments. The default value is true.

## See Also

### Working with the selection

var selectedRange: NSRange

The current selection range of the text view.

func scrollRangeToVisible(NSRange)

Scrolls the text view until the text in the specified range is visible.

var clearsOnInsertion: Bool

A Boolean value that indicates whether inserting text replaces the previous contents.

