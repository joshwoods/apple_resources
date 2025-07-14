

- Swift
- Character
-  isWhitespace 

Instance Property

# isWhitespace

A Boolean value indicating whether this character represents whitespace, including newlines.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isWhitespace: Bool { get }
```

## Discussion

For example, the following characters all represent whitespace:

- “\t” (U+0009 CHARACTER TABULATION)

- “ “ (U+0020 SPACE)

- U+2029 PARAGRAPH SEPARATOR

- U+3000 IDEOGRAPHIC SPACE

## See Also

### Inspecting a Character

var isLetter: Bool

A Boolean value indicating whether this character is a letter.

var isPunctuation: Bool

A Boolean value indicating whether this character represents punctuation.

var isNewline: Bool

A Boolean value indicating whether this character represents a newline.

var isSymbol: Bool

A Boolean value indicating whether this character represents a symbol.

var isMathSymbol: Bool

A Boolean value indicating whether this character represents a symbol that naturally appears in mathematical contexts.

var isCurrencySymbol: Bool

A Boolean value indicating whether this character represents a currency symbol.

