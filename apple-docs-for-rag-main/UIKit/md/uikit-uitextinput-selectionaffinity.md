

- UIKit
- UITextInput
-  selectionAffinity 

Instance Property

# selectionAffinity

The desired location for the insertion point.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
optional var selectionAffinity: UITextStorageDirection { get set }
```

## Discussion

For text selections that wrap across line boundaries, this property determines whether the insertion point appears after the last character on the line or before the first character on the following line. The selection affinity is set in response to the user navigating via the keyboard (for example, command-right-arrow). The text input system checks this property when it moves the insertion point around in a document.

In the default implementation, if the selection is not at the end of the line, or if the selection is at the start of a paragraph for an empty line, a forward direction is assumed (UITextStorageDirection.forward); otherwise, a backward direction UITextStorageDirection.backward is assumed.

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

func unmarkText()

Unmarks the currently marked text.

**Required**

