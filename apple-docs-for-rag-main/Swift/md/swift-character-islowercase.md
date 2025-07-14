

- Swift
- Character
-  isLowercase 

Instance Property

# isLowercase

A Boolean value indicating whether this character is considered lowercase.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isLowercase: Bool { get }
```

## Discussion

Lowercase characters change when converted to uppercase, but not when converted to lowercase. The following characters are all lowercase:

- “é” (U+0065 LATIN SMALL LETTER E, U+0301 COMBINING ACUTE ACCENT)

- “и” (U+0438 CYRILLIC SMALL LETTER I)

- “π” (U+03C0 GREEK SMALL LETTER PI)

## See Also

### Checking a Character’s Case

var isCased: Bool

A Boolean value indicating whether this character changes under any form of case conversion.

var isUppercase: Bool

A Boolean value indicating whether this character is considered uppercase.

func uppercased() -> String

Returns an uppercased version of this character.

func lowercased() -> String

Returns a lowercased version of this character.

