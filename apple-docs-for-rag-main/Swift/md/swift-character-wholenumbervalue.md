

- Swift
- Character
-  wholeNumberValue 

Instance Property

# wholeNumberValue

The numeric value this character represents, if it represents a whole number.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var wholeNumberValue: Int? { get }
```

## Discussion

If this character does not represent a whole number, or the value is too large to represent as an `Int`, the value of this property is `nil`.

```
let chars: [Character] = ["4", "④", "万", "a"]
for ch in chars {
    print(ch, "-->", ch.wholeNumberValue)
}
// Prints:
// 4 --> Optional(4)
// ④ --> Optional(4)
// 万 --> Optional(10000)
// a --> nil
```

## See Also

### Checking a Character’s Numeric Properties

var isNumber: Bool

A Boolean value indicating whether this character represents a number.

var isWholeNumber: Bool

A Boolean value indicating whether this character represents a whole number.

var isHexDigit: Bool

A Boolean value indicating whether this character represents a hexadecimal digit.

var hexDigitValue: Int?

The numeric value this character represents, if it is a hexadecimal digit.

