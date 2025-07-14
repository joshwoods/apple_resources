

- AppKit
- NSTextInputClient
-  setMarkedText(\_:selectedRange:replacementRange:) 

Instance Method

# setMarkedText(\_:selectedRange:replacementRange:)

Replaces a specified range in the receiver’s text storage with the given string and sets the selection.

macOS

``` source
func setMarkedText(
    _ string: Any,
    selectedRange: NSRange,
    replacementRange: NSRange
)
```

**Required**

## Parameters 

`string`  

The string to insert. Can be either an `NSString` or `NSAttributedString` instance.

`selectedRange`  

The range to set as the selection, computed from the beginning of the inserted string.

`replacementRange`  

The range to replace, computed from the beginning of the marked text.

## Discussion

If there is no marked text, the current selection is replaced. If there is no selection, the string is inserted at the insertion point.

When `aString` is an `NSString` object, the receiver is expected to render the marked text with distinguishing appearance (for example, `NSTextView` renders with markedTextAttributes).

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

func unmarkText()

Unmarks the marked text.

**Required**

func validAttributesForMarkedText() -> [NSAttributedString.Key]

Returns an array of attribute names recognized by the receiver.

**Required**

