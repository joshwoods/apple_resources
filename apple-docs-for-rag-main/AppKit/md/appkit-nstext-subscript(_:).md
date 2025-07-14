

- AppKit
- NSText
-  subscript(\_:) 

Instance Method

# subscript(\_:)

This action method applies a subscript attribute to selected text (or all text if the receiver is a plain text object), lowering its baseline offset by a predefined amount.

macOS

``` source
@MainActor
func `subscript`(_ sender: Any?)
```

## See Also

### Related Documentation

func lowerBaseline(Any?)

Lowers the baseline offset of selected text by 1 point, or of all text if the receiver is a plain text view.

### Setting superscripting and subscripting

func superscript(Any?)

This action method applies a superscript attribute to selected text (or all text if the receiver is a plain text object), raising its baseline offset by a predefined amount.

func unscript(Any?)

This action method removes any superscripting or subscripting from selected text (or all text if the receiver is a plain text object).

