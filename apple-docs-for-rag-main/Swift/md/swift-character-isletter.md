

- Swift
- Character
-  isLetter 

Instance Property

# isLetter

A Boolean value indicating whether this character is a letter.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isLetter: Bool { get }
```

## Discussion

For example, the following characters are all letters:

- “A” (U+0041 LATIN CAPITAL LETTER A)

- “é” (U+0065 LATIN SMALL LETTER E, U+0301 COMBINING ACUTE ACCENT)

- “ϴ” (U+03F4 GREEK CAPITAL THETA SYMBOL)

- “ڈ” (U+0688 ARABIC LETTER DDAL)

- “日” (U+65E5 CJK UNIFIED IDEOGRAPH-65E5)

- “ᚨ” (U+16A8 RUNIC LETTER ANSUZ A)

## See Also

### Inspecting a Character

var isPunctuation: Bool

A Boolean value indicating whether this character represents punctuation.

var isNewline: Bool

A Boolean value indicating whether this character represents a newline.

var isWhitespace: Bool

A Boolean value indicating whether this character represents whitespace, including newlines.

var isSymbol: Bool

A Boolean value indicating whether this character represents a symbol.

var isMathSymbol: Bool

A Boolean value indicating whether this character represents a symbol that naturally appears in mathematical contexts.

var isCurrencySymbol: Bool

A Boolean value indicating whether this character represents a currency symbol.

