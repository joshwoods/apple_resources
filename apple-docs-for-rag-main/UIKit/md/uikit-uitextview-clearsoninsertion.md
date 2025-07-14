

- UIKit
- UITextView
-  clearsOnInsertion 

Instance Property

# clearsOnInsertion

A Boolean value that indicates whether inserting text replaces the previous contents.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var clearsOnInsertion: Bool { get set }
```

## Discussion

The default value of this property is false. When the value of this property is true and the text view is in editing mode, the selection UI is hidden and inserting new text clears the contents of the text view and sets the value of this property back to false.

## See Also

### Working with the selection

var selectedRange: NSRange

The current selection range of the text view.

func scrollRangeToVisible(NSRange)

Scrolls the text view until the text in the specified range is visible.

var isSelectable: Bool

A Boolean value that indicates whether the text view is selectable.

