

- Foundation
- NSDecimalNumber
-  rounding(accordingToBehavior:) 

Instance Method

# rounding(accordingToBehavior:)

Returns a rounded version of the decimal number using the specified rounding behavior.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func rounding(accordingToBehavior behavior: (any NSDecimalNumberBehaviors)?) -> NSDecimalNumber
```

## Discussion

For a description of the different ways of rounding, see the roundingMode method in the NSDecimalNumberBehaviors protocol specification.

