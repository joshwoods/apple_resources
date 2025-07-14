

- AppKit
- NSText
-  unscript(\_:) 

Instance Method

# unscript(\_:)

This action method removes any superscripting or subscripting from selected text (or all text if the receiver is a plain text object).

macOS

``` source
@MainActor
func unscript(_ sender: Any?)
```

## See Also

### Related Documentation

func lowerBaseline(Any?)

Lowers the baseline offset of selected text by 1 point, or of all text if the receiver is a plain text view.

func raiseBaseline(Any?)

Raises the baseline offset of selected text by 1 point, or of all text if the receiver is a plain text view.

### Setting superscripting and subscripting

func superscript(Any?)

This action method applies a superscript attribute to selected text (or all text if the receiver is a plain text object), raising its baseline offset by a predefined amount.

func `subscript`(Any?)

This action method applies a subscript attribute to selected text (or all text if the receiver is a plain text object), lowering its baseline offset by a predefined amount.

