

- Swift
- Character
-  isHexDigit 

Instance Property

# isHexDigit

A Boolean value indicating whether this character represents a hexadecimal digit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isHexDigit: Bool { get }
```

## Discussion

Hexadecimal digits include 0-9, Latin letters a-f and A-F, and their fullwidth compatibility forms. To get the character’s value, use the `hexDigitValue` property.

## See Also

### Checking a Character’s Numeric Properties

var isNumber: Bool

A Boolean value indicating whether this character represents a number.

var isWholeNumber: Bool

A Boolean value indicating whether this character represents a whole number.

var wholeNumberValue: Int?

The numeric value this character represents, if it represents a whole number.

var hexDigitValue: Int?

The numeric value this character represents, if it is a hexadecimal digit.

