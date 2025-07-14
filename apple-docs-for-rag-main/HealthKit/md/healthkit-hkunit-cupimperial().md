

- HealthKit
- HKUnit
-  cupImperial() 

Type Method

# cupImperial()

Returns a HealthKit unit for measuring volume in imperial cups.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 2.0+

``` source
class func cupImperial() -> Self
```

## Return Value

A HealthKit unit for measuring volume in imperial cups.

## See Also

### Constructing volume units

class func liter() -> Self

Returns a HealthKit unit for measuring volume in liters.

class func literUnit(with: HKMetricPrefix) -> Self

Returns a HealthKit unit for measuring volume, using liter units with the provided prefix.

class func fluidOunceUS() -> Self

Returns a HealthKit unit for measuring volume in US fluid ounces.

class func fluidOunceImperial() -> Self

Returns a HealthKit unit for measuring volume in imperial fluid ounces.

class func cupUS() -> Self

Returns a HealthKit unit for measuring volume in US cups.

class func pintUS() -> Self

Returns a HealthKit unit for measuring volume in US pints.

class func pintImperial() -> Self

Returns a HealthKit unit for measuring volume in imperial pints.

