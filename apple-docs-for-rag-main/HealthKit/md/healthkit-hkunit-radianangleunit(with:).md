

- HealthKit
- HKUnit
-  radianAngleUnit(with:) 

Type Method

# radianAngleUnit(with:)

Returns a HealthKit unit for measuring angles, using radian units with the provided prefix.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
class func radianAngleUnit(with prefix: HKMetricPrefix) -> Self
```

## Parameters 

`prefix`  

A valid metric prefix value. For the complete list of prefix values, see HKMetricPrefix.

## See Also

### Constructing angle units

class func degreeAngle() -> Self

Returns a HealthKit unit for measuring angles using degrees.

class func radianAngle() -> Self

Returns a HealthKit unit for measuring angles using radians.

