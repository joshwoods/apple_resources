

- Swift
- Character
-  hexDigitValue 

Instance Property

# hexDigitValue

The numeric value this character represents, if it is a hexadecimal digit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var hexDigitValue: Int? { get }
```

## Discussion

Hexadecimal digits include 0-9, Latin letters a-f and A-F, and their fullwidth compatibility forms. If the character does not represent a hexadecimal digit, the value of this property is `nil`.

```
let chars: [Character] = ["1", "a", "Ｆ", "g"]
for ch in chars {
    print(ch, "-->", ch.hexDigitValue)
}
// Prints:
// 1 --> Optional(1)
// a --> Optional(10)
// Ｆ --> Optional(15)
// g --> nil
```

## See Also

### Checking a Character’s Numeric Properties

var isNumber: Bool

A Boolean value indicating whether this character represents a number.

var isWholeNumber: Bool

A Boolean value indicating whether this character represents a whole number.

var wholeNumberValue: Int?

The numeric value this character represents, if it represents a whole number.

var isHexDigit: Bool

A Boolean value indicating whether this character represents a hexadecimal digit.

