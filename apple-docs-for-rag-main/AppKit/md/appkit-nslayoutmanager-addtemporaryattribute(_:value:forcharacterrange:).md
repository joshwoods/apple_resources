

- AppKit
- NSLayoutManager
-  addTemporaryAttribute(\_:value:forCharacterRange:) 

Instance Method

# addTemporaryAttribute(\_:value:forCharacterRange:)

Adds a temporary attribute to the characters in the specified range.

macOS 10.5+

``` source
func addTemporaryAttribute(
    _ attrName: NSAttributedString.Key,
    value: Any,
    forCharacterRange charRange: NSRange
)
```

## Parameters 

`attrName`  

The name of a temporary attribute.

`value`  

The temporary attribute value associated with `attrName`.

`charRange`  

The range of characters to which the specified attribute-value pair applies.

## Discussion

Raises an invalidArgumentException if `attrName` or `value` is `nil`.

## See Also

### Managing temporary attribute support

func addTemporaryAttributes([NSAttributedString.Key : Any], forCharacterRange: NSRange)

Appends one or more temporary attributes to the attributes dictionary of the specified character range.

func setTemporaryAttributes([NSAttributedString.Key : Any], forCharacterRange: NSRange)

Sets one or more temporary attributes for the specified character range.

func removeTemporaryAttribute(NSAttributedString.Key, forCharacterRange: NSRange)

Removes a temporary attribute from the list of attributes for the specified character range.

func temporaryAttribute(NSAttributedString.Key, atCharacterIndex: Int, effectiveRange: NSRangePointer?) -> Any?

Returns the value for the temporary attribute of a character, and the range it applies to.

func temporaryAttribute(NSAttributedString.Key, atCharacterIndex: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> Any?

Returns the value for the temporary attribute of a character, and the maximum range it applies to.

func temporaryAttributes(atCharacterIndex: Int, effectiveRange: NSRangePointer?) -> [NSAttributedString.Key : Any]

Returns the dictionary of temporary attributes for the specified character range.

func temporaryAttributes(atCharacterIndex: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> [NSAttributedString.Key : Any]

Returns the temporary attributes for a character, and the maximum range they apply to.

