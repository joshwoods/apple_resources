

- Foundation
-  NSDecimalCopy(\_:\_:) 

Function

# NSDecimalCopy(\_:\_:)

Copies the value of a decimal number.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func NSDecimalCopy(
    _ destination: UnsafeMutablePointer,
    _ source: UnsafePointer
)
```

## Parameters 

`destination`  

A Decimal reference that receives the copied value.

`source`  

A source Decimal to copy.

## Discussion

Copies the value in `source` to `destination`.

For more information, see Number and Value Programming Topics.

## See Also

### Creating a decimal from another decimal

init(signOf: Decimal, magnitudeOf: Decimal)

Creates and initializes a decimal with the sign and magnitude of the given decimals.

