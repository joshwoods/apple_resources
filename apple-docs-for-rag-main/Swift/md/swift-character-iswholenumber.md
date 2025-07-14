

- Swift
- Character
-  isWholeNumber 

Instance Property

# isWholeNumber

A Boolean value indicating whether this character represents a whole number.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isWholeNumber: Bool { get }
```

## Discussion

For example, the following characters all represent whole numbers:

- “1” (U+0031 DIGIT ONE) =\> 1

- “५” (U+096B DEVANAGARI DIGIT FIVE) =\> 5

- “๙” (U+0E59 THAI DIGIT NINE) =\> 9

- “万” (U+4E07 CJK UNIFIED IDEOGRAPH-4E07) =\> 10_000

## See Also

### Checking a Character’s Numeric Properties

var isNumber: Bool

A Boolean value indicating whether this character represents a number.

var wholeNumberValue: Int?

The numeric value this character represents, if it represents a whole number.

var isHexDigit: Bool

A Boolean value indicating whether this character represents a hexadecimal digit.

var hexDigitValue: Int?

The numeric value this character represents, if it is a hexadecimal digit.

