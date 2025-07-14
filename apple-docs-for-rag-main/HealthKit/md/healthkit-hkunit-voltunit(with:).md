

- HealthKit
- HKUnit
-  voltUnit(with:) 

Type Method

# voltUnit(with:)

Returns a HealthKit unit for measuring the electrical potential difference in volts with the provided prefix.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
class func voltUnit(with prefix: HKMetricPrefix) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

## See Also

### Electrical potential difference

class func volt() -> Self

Returns a HealthKit unit for measuring the difference in electrical potential using volts.

