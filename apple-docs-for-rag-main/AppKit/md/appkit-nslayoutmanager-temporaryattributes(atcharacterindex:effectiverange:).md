

- AppKit
- NSLayoutManager
-  temporaryAttributes(atCharacterIndex:effectiveRange:) 

Instance Method

# temporaryAttributes(atCharacterIndex:effectiveRange:)

Returns the dictionary of temporary attributes for the specified character range.

macOS 10.7+

``` source
func temporaryAttributes(
    atCharacterIndex charIndex: Int,
    effectiveRange effectiveCharRange: NSRangePointer?
) -> [NSAttributedString.Key : Any]
```

## Return Value

The dictionary of temporary attributes for the character range specified in `effectiveCharRange` at character index `charIndex`.

## Discussion

Temporary attributes are used only for onscreen drawing and are not persistent in any way. `NSTextView` uses them to color misspelled words when continuous spell checking is enabled. Currently the only temporary attributes recognized are those that do not affect layout (colors, underlines, and so on).

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

func temporaryAttributes(atCharacterIndex: Int, longestEffectiveRange: NSRangePointer?, in: NSRange) -> [NSAttributedString.Key : Any]

Returns the temporary attributes for a character, and the maximum range they apply to.

