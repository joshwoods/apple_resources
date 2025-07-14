

- UIKit
- UITextInput
-  setMarkedText(\_:selectedRange:) 

Instance Method

# setMarkedText(\_:selectedRange:)

Inserts the provided text and marks it to indicate that it is part of an active input session.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
func setMarkedText(
    _ markedText: String?,
    selectedRange: NSRange
)
```

**Required**

## Parameters 

`markedText`  

The text to be marked.

`selectedRange`  

A range within `markedText` that indicates the current selection. This range is always relative to `markedText`.

## Discussion

Setting marked text either replaces the existing marked text or, if none is present, inserts it in place of the current selection.

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

func setAttributedMarkedText(NSAttributedString?, selectedRange: NSRange)

Inserts the provided styled text and marks it to indicate that it is part of an active input session.

func unmarkText()

Unmarks the currently marked text.

**Required**

var selectionAffinity: UITextStorageDirection

The desired location for the insertion point.

