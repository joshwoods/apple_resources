

- UIKit
- UITextView
-  scrollRangeToVisible(\_:) 

Instance Method

# scrollRangeToVisible(\_:)

Scrolls the text view until the text in the specified range is visible.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func scrollRangeToVisible(_ range: NSRange)
```

## Parameters 

`range`  

The range of text to scroll into view.

## See Also

### Working with the selection

var selectedRange: NSRange

The current selection range of the text view.

var clearsOnInsertion: Bool

A Boolean value that indicates whether inserting text replaces the previous contents.

var isSelectable: Bool

A Boolean value that indicates whether the text view is selectable.

