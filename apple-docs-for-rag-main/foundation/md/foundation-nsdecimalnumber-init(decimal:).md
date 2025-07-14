

- Foundation
- NSDecimalNumber
-  init(decimal:) 

Initializer

# init(decimal:)

Initializes a decimal number to represent a given decimal.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(decimal dcm: Decimal)
```

## Parameters 

`dcm`  

The value of the new object.

## Return Value

An `NSDecimalNumber` object initialized to represent `dcm`.

## Discussion

This method is the designated initializer for `NSDecimalNumber`.

## See Also

### Initializing a Decimal Number

convenience init(mantissa: UInt64, exponent: Int16, isNegative: Bool)

Initializes a decimal number using the given mantissa, exponent, and sign.

convenience init(string: String?)

Initializes a decimal number so that its value is equivalent to that in a given numeric string.

convenience init(string: String?, locale: Any?)

Initializes a decimal number so that its value is equivalent to that in a given numeric string, interpreted using a given locale.

