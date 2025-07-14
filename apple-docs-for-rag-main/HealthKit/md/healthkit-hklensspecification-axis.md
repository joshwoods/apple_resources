

- HealthKit
- HKLensSpecification
-  axis 

Instance Property

# axis

Part of the correction for astigmatism that measures the orientation fo the correction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
@NSCopying
var axis: HKQuantity? { get }
```

## Discussion

This quantity measures the orientation of the correction in degreeAngle() units.

## See Also

### Accessing lens specification data

var sphere: HKQuantity

The correction for farsightedness.

var cylinder: HKQuantity?

Part of the correction for astigmatism that measures the strength of the correction.

var addPower: HKQuantity?

The correction for nearsightedness.

