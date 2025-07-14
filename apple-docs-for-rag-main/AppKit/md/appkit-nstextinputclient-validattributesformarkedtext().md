

- AppKit
- NSTextInputClient
-  validAttributesForMarkedText() 

Instance Method

# validAttributesForMarkedText()

Returns an array of attribute names recognized by the receiver.

macOS 10.0+

``` source
func validAttributesForMarkedText() -> [NSAttributedString.Key]
```

**Required**

## Return Value

An array of `NSString` objects representing names for the supported attributes.

## Discussion

Returns an empty array if no attributes are supported. See NSAttributedString Application Kit Additions Reference for the set of string constants representing standard attributes.

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

func unmarkText()

Unmarks the marked text.

**Required**

