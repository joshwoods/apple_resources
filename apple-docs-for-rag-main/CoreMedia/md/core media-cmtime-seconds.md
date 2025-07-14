

- Core Media
- CMTime
-  seconds 

Instance Property

# seconds

A representation of the time in seconds.

iOS 4.0+iPadOS 4.0+Mac CatalystmacOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
var seconds: Double { get }
```

## Discussion

If the time is invalid or indefinite, the value equals nan.

## See Also

### Inspecting a Time

var hasBeenRounded: Bool

A Boolean value that indicates whether the system rounded the time.

var isValid: Bool

A Boolean value that indicates whether a time is valid.

var isNumeric: Bool

A Boolean value that indicates whether a time is numeric.

var isIndefinite: Bool

A Boolean value that indicates whether a time is indefinite.

var isPositiveInfinity: Bool

A Boolean value that indicates whether a time represents positive infinity.

var isNegativeInfinity: Bool

A Boolean value that indicates whether a time represents negative infinity.

