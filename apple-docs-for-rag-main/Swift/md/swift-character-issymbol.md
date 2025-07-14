

- Swift
- Character
-  isSymbol 

Instance Property

# isSymbol

A Boolean value indicating whether this character represents a symbol.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isSymbol: Bool { get }
```

## Discussion

This property is `true` only for characters composed of scalars in the “Math_Symbol”, “Currency_Symbol”, “Modifier_Symbol”, or “Other_Symbol” categories in the Unicode Standard.

For example, the following characters all represent symbols:

- “®” (U+00AE REGISTERED SIGN)

- “⌹” (U+2339 APL FUNCTIONAL SYMBOL QUAD DIVIDE)

- “⡆” (U+2846 BRAILLE PATTERN DOTS-237)

## See Also

### Inspecting a Character

var isLetter: Bool

A Boolean value indicating whether this character is a letter.

var isPunctuation: Bool

A Boolean value indicating whether this character represents punctuation.

var isNewline: Bool

A Boolean value indicating whether this character represents a newline.

var isWhitespace: Bool

A Boolean value indicating whether this character represents whitespace, including newlines.

var isMathSymbol: Bool

A Boolean value indicating whether this character represents a symbol that naturally appears in mathematical contexts.

var isCurrencySymbol: Bool

A Boolean value indicating whether this character represents a currency symbol.

