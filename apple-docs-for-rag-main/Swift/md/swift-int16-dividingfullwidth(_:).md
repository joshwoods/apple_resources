

- Swift
- Int16
-  dividingFullWidth(\_:) 

Instance Method

# dividingFullWidth(\_:)

Returns a tuple containing the quotient and remainder of dividing the given value by this value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dividingFullWidth(_ dividend: (high: Int16, low: Int16.Magnitude)) -> (quotient: Int16, remainder: Int16)
```

## Parameters 

`dividend`  

A tuple containing the high and low parts of a double-width integer. The `high` component of the value carries the sign, if the type is signed.

## Return Value

A tuple containing the quotient and remainder of `dividend` divided by this value.

## Discussion

The resulting quotient must be representable within the bounds of the type. If the quotient of dividing `dividend` by this value is too large to represent in the type, a runtime error will occur.

