

- Foundation
- Decimal
-  init(signOf:magnitudeOf:) 

Initializer

# init(signOf:magnitudeOf:)

Creates and initializes a decimal with the sign and magnitude of the given decimals.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    signOf: Decimal,
    magnitudeOf magnitude: Decimal
)
```

## Parameters 

`signOf`  

A Decimal to use for the sign of the newly-created Decimal.

`magnitude`  

A Decimal to use for the magnitude of the newly-created Decimal.

## See Also

### Creating a decimal from another decimal

func NSDecimalCopy(UnsafeMutablePointer&lt;Decimal>, UnsafePointer&lt;Decimal>)

Copies the value of a decimal number.

