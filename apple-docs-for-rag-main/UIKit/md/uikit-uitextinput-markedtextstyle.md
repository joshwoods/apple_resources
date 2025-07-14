

- UIKit
- UITextInput
-  markedTextStyle 

Instance Property

# markedTextStyle

A dictionary of attributes that describes how to draw marked text.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var markedTextStyle: [NSAttributedString.Key : Any]? { get set }
```

**Required**

## Discussion

Marked text requires a unique visual treatment when displayed to users. See Style dictionary keys for descriptions of the valid keys and values for this dictionary.

## See Also

### Working with marked and selected text

var selectedTextRange: UITextRange?

The range of selected text in a document.

**Required**

var markedTextRange: UITextRange?

The range of currently marked text in a document.

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

