

- HealthKit
-  HKPrismBase 

Enumeration

# HKPrismBase

The orientation of the prism correction, represented by the location of the prism’s base (the thickest part of the prism).

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
enum HKPrismBase
```

## Topics

### Prism Base

case none

No prism correction.

case up

The prism’s base is at the top of the lens.

case down

The prism’s base is at the bottom of the lens.

case `in`

The prism base is on the inside edge of the lens.

case out

The prism base is on the outside edge of the lens.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var horizontalAmount: HKQuantity

The strength of the horizontal correction.

var horizontalBase: HKPrismBase

The orientation of the horizontal portion of the correction.

var verticalAmount: HKQuantity

The strength of the vertical correction.

var verticalBase: HKPrismBase

The orientation of the vertical portion of the correction.

