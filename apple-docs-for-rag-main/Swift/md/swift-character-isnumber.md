

- Swift
- Character
-  isNumber 

Instance Property

# isNumber

A Boolean value indicating whether this character represents a number.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isNumber: Bool { get }
```

## Discussion

For example, the following characters all represent numbers:

- “7” (U+0037 DIGIT SEVEN)

- “⅚” (U+215A VULGAR FRACTION FIVE SIXTHS)

- “㊈” (U+3288 CIRCLED IDEOGRAPH NINE)

- “𝟠” (U+1D7E0 MATHEMATICAL DOUBLE-STRUCK DIGIT EIGHT)

- “๒” (U+0E52 THAI DIGIT TWO)

## See Also

### Checking a Character’s Numeric Properties

var isWholeNumber: Bool

A Boolean value indicating whether this character represents a whole number.

var wholeNumberValue: Int?

The numeric value this character represents, if it represents a whole number.

var isHexDigit: Bool

A Boolean value indicating whether this character represents a hexadecimal digit.

var hexDigitValue: Int?

The numeric value this character represents, if it is a hexadecimal digit.

