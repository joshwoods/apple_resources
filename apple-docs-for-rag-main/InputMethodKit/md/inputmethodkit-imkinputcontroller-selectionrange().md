

- InputMethodKit
- IMKInputController
-  selectionRange() 

Instance Method

# selectionRange()

Returns where the range of the selection that should be placed inside marked text.

macOS 10.5+

``` source
func selectionRange() -> NSRange
```

## Return Value

The range of the selection.

## Discussion

This method is called by updateComposition() to obtain the selection range for marked text. The default implementation sets the selection range at the end of the marked text. You should override this method if your input method provides font or glyph information.

## See Also

### Working with Ranges

func compositionAttributes(at: NSRange) -> NSMutableDictionary!

Returns a dictionary of text attributes.

func replacementRange() -> NSRange

Returns the range in the client document that the text should replace.

func mark(forStyle: Int, at: NSRange) -> [AnyHashable : Any]!

Returns a dictionary of text attributes that can mark a range of an attributed string to send to a client.

