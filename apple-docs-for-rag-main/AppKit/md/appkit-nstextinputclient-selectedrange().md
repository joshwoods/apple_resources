

- AppKit
- NSTextInputClient
-  selectedRange() 

Instance Method

# selectedRange()

Returns the range of selected text.

macOS

``` source
func selectedRange() -> NSRange
```

**Required**

## Return Value

The range of selected text or `{NSNotFound, 0}` if there is no selection.

## Discussion

The returned range measures from the start of the receiver’s text storage, that is, from 0 to the document length.

## See Also

### Handling marked text

func hasMarkedText() -> Bool

Returns a Boolean value indicating whether the receiver has marked text.

**Required**

func markedRange() -> NSRange

Returns the range of the marked text.

**Required**

func setMarkedText(Any, selectedRange: NSRange, replacementRange: NSRange)

Replaces a specified range in the receiver’s text storage with the given string and sets the selection.

**Required**

func unmarkText()

Unmarks the marked text.

**Required**

func validAttributesForMarkedText() -> [NSAttributedString.Key]

Returns an array of attribute names recognized by the receiver.

**Required**

