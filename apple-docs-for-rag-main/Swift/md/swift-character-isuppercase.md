

- Swift
- Character
-  isUppercase 

Instance Property

# isUppercase

A Boolean value indicating whether this character is considered uppercase.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isUppercase: Bool { get }
```

## Discussion

Uppercase characters vary under case-conversion to lowercase, but not when converted to uppercase. The following characters are all uppercase:

- “É” (U+0045 LATIN CAPITAL LETTER E, U+0301 COMBINING ACUTE ACCENT)

- “И” (U+0418 CYRILLIC CAPITAL LETTER I)

- “Π” (U+03A0 GREEK CAPITAL LETTER PI)

## See Also

### Checking a Character’s Case

var isCased: Bool

A Boolean value indicating whether this character changes under any form of case conversion.

func uppercased() -> String

Returns an uppercased version of this character.

var isLowercase: Bool

A Boolean value indicating whether this character is considered lowercase.

func lowercased() -> String

Returns a lowercased version of this character.

