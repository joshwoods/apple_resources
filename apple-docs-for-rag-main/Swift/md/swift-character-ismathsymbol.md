

- Swift
- Character
-  isMathSymbol 

Instance Property

# isMathSymbol

A Boolean value indicating whether this character represents a symbol that naturally appears in mathematical contexts.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isMathSymbol: Bool { get }
```

## Discussion

For example, the following characters all represent math symbols:

- “+” (U+002B PLUS SIGN)

- “∫” (U+222B INTEGRAL)

- “ϰ” (U+03F0 GREEK KAPPA SYMBOL)

The set of characters that have an `isMathSymbol` value of `true` is not a strict subset of those for which `isSymbol` is `true`. This includes characters used both as letters and commonly in mathematical formulas. For example, “ϰ” (U+03F0 GREEK KAPPA SYMBOL) is considered both a mathematical symbol and a letter.

This property corresponds to the “Math” property in the Unicode Standard.

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

var isSymbol: Bool

A Boolean value indicating whether this character represents a symbol.

var isCurrencySymbol: Bool

A Boolean value indicating whether this character represents a currency symbol.

