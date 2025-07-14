

- HealthKit
- HKLensSpecification
-  sphere 

Instance Property

# sphere

The correction for farsightedness.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
@NSCopying
var sphere: HKQuantity { get }
```

## Discussion

This quantity uses diopter() units. The range is -10.5 to +6.5.

## See Also

### Accessing lens specification data

var cylinder: HKQuantity?

Part of the correction for astigmatism that measures the strength of the correction.

var axis: HKQuantity?

Part of the correction for astigmatism that measures the orientation fo the correction.

var addPower: HKQuantity?

The correction for nearsightedness.

