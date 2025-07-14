

- UIKit
- UITextInput
-  markedTextRange 

Instance Property

# markedTextRange

The range of currently marked text in a document.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var markedTextRange: UITextRange? { get }
```

**Required**

## Discussion

If there is no marked text, the value of the property is `nil`. Marked text is provisionally inserted text that requires user confirmation; it occurs in multistage text input. The current selection, which can be a caret or an extended range, always occurs within the marked text.

## See Also

### Working with marked and selected text

var selectedTextRange: UITextRange?

The range of selected text in a document.

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

