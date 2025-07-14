

- AppKit
- NSLayoutManager
-  temporaryAttribute(\_:atCharacterIndex:effectiveRange:) 

Instance Method

# temporaryAttribute(\_:atCharacterIndex:effectiveRange:)

Returns the value for the temporary attribute of a character, and the range it applies to.

macOS 10.5+

``` source
func temporaryAttribute(
    _ attrName: NSAttributedString.Key,
    atCharacterIndex location: Int,
    effectiveRange range: NSRangePointer?
) -> Any?
```

## Parameters 

`attrName`  

The name of a temporary attribute.

`location`  

The index for which to return attributes. This value must not exceed the bounds of the receiver.

`range`  

If non-`NULL`:

- If the named attribute exists at `location`, on output, contains the range over which the named attribute’s value applies.

- If the named attribute does not exist at `location`, on output, contains the range over which the attribute does not exist.

The range isn’t necessarily the maximum range covered by `attrName`, and its extent is implementation-dependent. If you need the maximum range, use temporaryAttribute(_:atCharacterIndex:longestEffectiveRange:in:). If you don’t need this value, pass `NULL`.

## Return Value

The value for the temporary attribute named `attrName` of the character at index `location`, or `nil` if there is no such attribute.

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

func temporaryAttribute(NSAttributedString.Key, atCharacterIndex: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> Any?

Returns the value for the temporary attribute of a character, and the maximum range it applies to.

func temporaryAttributes(atCharacterIndex: Int, effectiveRange: NSRangePointer?) -> [NSAttributedString.Key : Any]

Returns the dictionary of temporary attributes for the specified character range.

func temporaryAttributes(atCharacterIndex: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> [NSAttributedString.Key : Any]

Returns the temporary attributes for a character, and the maximum range they apply to.

