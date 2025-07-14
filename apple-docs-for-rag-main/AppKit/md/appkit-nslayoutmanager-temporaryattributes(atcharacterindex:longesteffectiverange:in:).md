

- AppKit
- NSLayoutManager
-  temporaryAttributes(atCharacterIndex:longestEffectiveRange:in:) 

Instance Method

# temporaryAttributes(atCharacterIndex:longestEffectiveRange:in:)

Returns the temporary attributes for a character, and the maximum range they apply to.

macOS 10.5+

``` source
func temporaryAttributes(
    atCharacterIndex location: Int,
    longestEffectiveRange range: NSRangePointer?,
    in rangeLimit: NSRange
) -> [NSAttributedString.Key : Any]
```

## Parameters 

`location`  

The index for which to return attributes. This value must not exceed the bounds of the receiver.

`range`  

If not `NULL`, on output, contains the maximum range over which the attributes and values are the same as those at `location`, clipped to `rangeLimit`.

`rangeLimit`  

The range over which to search for continuous presence of the attributes at `location`. This value must not exceed the bounds of the receiver.

## Return Value

The attributes for the character at `location`.

## Discussion

If you don’t need the longest effective range, it’s far more efficient to use the temporaryAttributes(atCharacterIndex:effectiveRange:) method to retrieve the attribute value.

## See Also

### Managing temporary attribute support

func addTemporaryAttributes([NSAttributedString.Key : Any], forCharacterRange: NSRange)

Appends one or more temporary attributes to the attributes dictionary of the specified character range.

func addTemporaryAttribute(NSAttributedString.Key, value: Any, forCharacterRange: NSRange)

Adds a temporary attribute to the characters in the specified range.

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

