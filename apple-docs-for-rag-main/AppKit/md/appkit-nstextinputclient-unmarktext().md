

- AppKit
- NSTextInputClient
-  unmarkText() 

Instance Method

# unmarkText()

Unmarks the marked text.

macOS

``` source
func unmarkText()
```

**Required**

## Discussion

The receiver removes any marking from pending input text and disposes of the marked text as it wishes. The text view should accept the marked text as if it had been inserted normally. If there is no marked text, the invocation of this method has no effect.

## See Also

### Handling marked text

func hasMarkedText() -> Bool

Returns a Boolean value indicating whether the receiver has marked text.

**Required**

func markedRange() -> NSRange

Returns the range of the marked text.

**Required**

func selectedRange() -> NSRange

Returns the range of selected text.

**Required**

func setMarkedText(Any, selectedRange: NSRange, replacementRange: NSRange)

Replaces a specified range in the receiver’s text storage with the given string and sets the selection.

**Required**

func validAttributesForMarkedText() -> [NSAttributedString.Key]

Returns an array of attribute names recognized by the receiver.

**Required**

