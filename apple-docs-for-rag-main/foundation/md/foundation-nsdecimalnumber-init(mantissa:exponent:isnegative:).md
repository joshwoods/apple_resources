

- Foundation
- NSDecimalNumber
-  init(mantissa:exponent:isNegative:) 

Initializer

# init(mantissa:exponent:isNegative:)

Initializes a decimal number using the given mantissa, exponent, and sign.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(
    mantissa: UInt64,
    exponent: Int16,
    isNegative flag: Bool
)
```

## Parameters 

`mantissa`  

The mantissa for the new decimal number object.

`exponent`  

The exponent for the new decimal number object.

`flag`  

A Boolean value that specifies whether the sign of the number is negative.

## Return Value

An `NSDecimalNumber` object initialized using the given mantissa, exponent, and sign.

## Discussion

The arguments express a number in a type of scientific notation that requires the mantissa to be an integer. So, for example, if the number to be represented is 1.23, it is expressed as 123x10^–2—`mantissa` is 123; `exponent` is –2; and `isNegative`, which refers to the sign of the mantissa, is false.

## See Also

### Initializing a Decimal Number

init(decimal: Decimal)

Initializes a decimal number to represent a given decimal.

convenience init(string: String?)

Initializes a decimal number so that its value is equivalent to that in a given numeric string.

convenience init(string: String?, locale: Any?)

Initializes a decimal number so that its value is equivalent to that in a given numeric string, interpreted using a given locale.

