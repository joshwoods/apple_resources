

- UIKit
- UITextInput
-  unmarkText() 

Instance Method

# unmarkText()

Unmarks the currently marked text.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func unmarkText()
```

**Required**

## Discussion

After this method is called, the value of markedTextRange is `nil`.

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

func setAttributedMarkedText(NSAttributedString?, selectedRange: NSRange)

Inserts the provided styled text and marks it to indicate that it is part of an active input session.

var selectionAffinity: UITextStorageDirection

The desired location for the insertion point.

