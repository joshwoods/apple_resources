

- AppKit
- NSTextInputClient
-  markedRange() 

Instance Method

# markedRange()

Returns the range of the marked text.

macOS

``` source
func markedRange() -> NSRange
```

**Required**

## Return Value

The range of marked text or `{NSNotFound, 0}` if there is no marked range.

## Discussion

The returned range measures from the start of the receiver’s text storage. The return value’s `location` is `NSNotFound` and its `length` is 0 if and only if hasMarkedText() returns false.

## See Also

### Handling marked text

func hasMarkedText() -> Bool

Returns a Boolean value indicating whether the receiver has marked text.

**Required**

func selectedRange() -> NSRange

Returns the range of selected text.

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

