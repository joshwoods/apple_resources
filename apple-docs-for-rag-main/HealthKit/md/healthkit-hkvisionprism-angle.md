

- HealthKit
- HKVisionPrism
-  angle 

Instance Property

# angle

The orientation of the adjustment.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
@NSCopying
var angle: HKQuantity { get }
```

## Discussion

This is the orientation of the amount correction, measured in degreeAngle() units.

## See Also

### Accessing lens specification data

var eye: HKVisionEye

A value indicating which eye the correction applies to.

enum HKVisionEye

A value that specifies the eye for a vision prescription.

var amount: HKQuantity

The strength of the correction.

var horizontalAmount: HKQuantity

The strength of the horizontal correction.

var horizontalBase: HKPrismBase

The orientation of the horizontal portion of the correction.

var verticalAmount: HKQuantity

The strength of the vertical correction.

var verticalBase: HKPrismBase

The orientation of the vertical portion of the correction.

enum HKPrismBase

The orientation of the prism correction, represented by the location of the prism’s base (the thickest part of the prism).

