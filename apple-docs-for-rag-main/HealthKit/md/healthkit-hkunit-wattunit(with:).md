

- HealthKit
- HKUnit
-  wattUnit(with:) 

Type Method

# wattUnit(with:)

Returns a HealthKit unit for measuring power, using watt units with the provided prefix.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class func wattUnit(with prefix: HKMetricPrefix) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

## See Also

### Constructing power units

class func watt() -> Self

Returns a HealthKit unit for measuring power in watts.

