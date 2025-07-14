

- Swift
- Character
-  isPunctuation 

Instance Property

# isPunctuation

A Boolean value indicating whether this character represents punctuation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isPunctuation: Bool { get }
```

## Discussion

For example, the following characters all represent punctuation:

- “!” (U+0021 EXCLAMATION MARK)

- “؟” (U+061F ARABIC QUESTION MARK)

- “…” (U+2026 HORIZONTAL ELLIPSIS)

- “—” (U+2014 EM DASH)

- ““” (U+201C LEFT DOUBLE QUOTATION MARK)

## See Also

### Inspecting a Character

var isLetter: Bool

A Boolean value indicating whether this character is a letter.

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

