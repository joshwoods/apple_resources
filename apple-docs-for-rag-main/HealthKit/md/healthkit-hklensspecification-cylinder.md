

- HealthKit
- HKLensSpecification
-  cylinder 

Instance Property

# cylinder

Part of the correction for astigmatism that measures the strength of the correction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
@NSCopying
var cylinder: HKQuantity? { get }
```

## Discussion

This quantity measures the strength of the correction in diopter() units. The range is -3.0 to 3.0.

## See Also

### Accessing lens specification data

var sphere: HKQuantity

The correction for farsightedness.

var axis: HKQuantity?

Part of the correction for astigmatism that measures the orientation fo the correction.

var addPower: HKQuantity?

The correction for nearsightedness.

