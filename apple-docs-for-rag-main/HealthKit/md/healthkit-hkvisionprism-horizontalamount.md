

- HealthKit
- HKVisionPrism
-  horizontalAmount 

Instance Property

# horizontalAmount

The strength of the horizontal correction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
@NSCopying
var horizontalAmount: HKQuantity { get }
```

## Discussion

This parameter holds the horizontal component of the prescriptions correction, measured in prismDiopter() units.

## See Also

### Accessing lens specification data

var eye: HKVisionEye

A value indicating which eye the correction applies to.

enum HKVisionEye

A value that specifies the eye for a vision prescription.

var amount: HKQuantity

The strength of the correction.

var angle: HKQuantity

The orientation of the adjustment.

var horizontalBase: HKPrismBase

The orientation of the horizontal portion of the correction.

var verticalAmount: HKQuantity

The strength of the vertical correction.

var verticalBase: HKPrismBase

The orientation of the vertical portion of the correction.

enum HKPrismBase

The orientation of the prism correction, represented by the location of the prism’s base (the thickest part of the prism).

