

- Foundation
- NumberFormatter
-  zeroSymbol 

Instance Property

# zeroSymbol

The string used to represent a zero value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var zeroSymbol: String? { get set }
```

## Discussion

If not specified, zero values are formatted normally.

You might, for example, set this property to “```  ``-``  ```” in a spreadsheet used for accounting.

## See Also

### Configuring Numeric Symbols

var percentSymbol: String!

The string used to represent a percent symbol.

var perMillSymbol: String!

The string used to represent a per-mill (per-thousand) symbol.

var minusSign: String!

The string used to represent a minus sign.

var plusSign: String!

The string used to represent a plus sign.

var exponentSymbol: String!

The string used to represent an exponent symbol.

var nilSymbol: String

The string used to represent a `nil` value.

var notANumberSymbol: String!

The string used to represent a NaN (“not a number”) value.

var negativeInfinitySymbol: String

The string used to represent a negative infinity symbol.

var positiveInfinitySymbol: String

The string used to represent a positive infinity symbol.

