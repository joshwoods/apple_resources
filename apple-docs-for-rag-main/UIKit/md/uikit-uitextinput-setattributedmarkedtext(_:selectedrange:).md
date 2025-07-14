

- UIKit
- UITextInput
-  setAttributedMarkedText(\_:selectedRange:) 

Instance Method

# setAttributedMarkedText(\_:selectedRange:)

Inserts the provided styled text and marks it to indicate that it is part of an active input session.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional func setAttributedMarkedText(
    _ markedText: NSAttributedString?,
    selectedRange: NSRange
)
```

## See Also

### Working with marked and selected text

var selectedTextRange: UITextRange?

The range of selected text in a document.

**Required**

var markedTextRange: UITextRange?

The range of currently marked text in a document.

**Required**

var markedTextStyle: [NSAttributedString.Key : Any]?

A dictionary of attributes that describes how to draw marked text.

**Required**

func setMarkedText(String?, selectedRange: NSRange)

Inserts the provided text and marks it to indicate that it is part of an active input session.

**Required**

func unmarkText()

Unmarks the currently marked text.

**Required**

var selectionAffinity: UITextStorageDirection

The desired location for the insertion point.

