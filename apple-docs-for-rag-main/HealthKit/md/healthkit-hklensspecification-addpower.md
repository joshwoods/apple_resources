

- HealthKit
- HKLensSpecification
-  addPower 

Instance Property

# addPower

The correction for nearsightedness.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
@NSCopying
var addPower: HKQuantity? { get }
```

## Discussion

This quantity uses diopter() units. The range is from 0.25 to 2.5. The right and left eyes should have the same value.

## See Also

### Accessing lens specification data

var sphere: HKQuantity

The correction for farsightedness.

var cylinder: HKQuantity?

Part of the correction for astigmatism that measures the strength of the correction.

var axis: HKQuantity?

Part of the correction for astigmatism that measures the orientation fo the correction.

