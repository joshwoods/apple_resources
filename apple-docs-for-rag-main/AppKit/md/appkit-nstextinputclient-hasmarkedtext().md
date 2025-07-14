

- AppKit
- NSTextInputClient
-  hasMarkedText() 

Instance Method

# hasMarkedText()

Returns a Boolean value indicating whether the receiver has marked text.

macOS

``` source
func hasMarkedText() -> Bool
```

**Required**

## Return Value

true if the receiver has marked text; otherwise false.

## Discussion

The text view itself may call this method to determine whether there currently is marked text. `NSTextView`, for example, disables the Edit \> Copy menu item when this method returns true.

## See Also

### Handling marked text

func markedRange() -> NSRange

Returns the range of the marked text.

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

