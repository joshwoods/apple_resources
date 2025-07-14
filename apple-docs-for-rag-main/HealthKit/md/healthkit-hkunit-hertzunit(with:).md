

- HealthKit
- HKUnit
-  hertzUnit(with:) 

Type Method

# hertzUnit(with:)

Returns a HealthKit unit for measuring frequency in hertz with the provided prefix.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class func hertzUnit(with prefix: HKMetricPrefix) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

## Discussion

Hertz represent cycles per second.

## See Also

### Constructing frequency units

class func hertz() -> Self

Returns a HealthKit unit for measuring frequency in hertz.

