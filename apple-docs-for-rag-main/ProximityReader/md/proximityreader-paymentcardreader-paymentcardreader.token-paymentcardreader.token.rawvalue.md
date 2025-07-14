

- ProximityReader
- PaymentCardReader
- PaymentCardReader.Token
-  PaymentCardReader.Token.RawValue 

Type Alias

# PaymentCardReader.Token.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
typealias RawValue = String
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

