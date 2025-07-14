

- UIKit
- UITextInput
-  selectedTextRange 

Instance Property

# selectedTextRange

The range of selected text in a document.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@NSCopying @MainActor
var selectedTextRange: UITextRange? { get set }
```

**Required**

## Discussion

If the text range has a length, it indicates the currently selected text. If it has zero length, it indicates the caret (insertion point). If the text-range object is `nil`, it indicates that there is no current selection.

## See Also

### Related Documentation

var isEmpty: Bool

A Boolean value that indicates whether the range of text represented by the receiver is zero-length.

### Working with marked and selected text

var markedTextRange: UITextRange?

The range of currently marked text in a document.

**Required**

var markedTextStyle: [NSAttributedString.Key : Any]?

A dictionary of attributes that describes how to draw marked text.

**Required**

func setMarkedText(String?, selectedRange: NSRange)

Inserts the provided text and marks it to indicate that it is part of an active input session.

**Required**

func setAttributedMarkedText(NSAttributedString?, selectedRange: NSRange)

Inserts the provided styled text and marks it to indicate that it is part of an active input session.

func unmarkText()

Unmarks the currently marked text.

**Required**

var selectionAffinity: UITextStorageDirection

The desired location for the insertion point.

