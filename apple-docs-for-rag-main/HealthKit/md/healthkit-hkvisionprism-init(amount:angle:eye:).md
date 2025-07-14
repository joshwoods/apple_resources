

- HealthKit
- HKVisionPrism
-  init(amount:angle:eye:) 

Initializer

# init(amount:angle:eye:)

Creates a new vision prism object, using a single quantity and an alignment angle.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    amount: HKQuantity,
    angle: HKQuantity,
    eye: HKVisionEye
)
```

## Parameters 

`amount`  

The strength of the correction, measured in prismDiopter() units.

`angle`  

The orientation of the adjustment, measured in degreeAngle() units.

`eye`  

A value indicating which eye the correction applies to: HKVisionEye.left or HKVisionEye.right.

## See Also

### Creating vision prism objects

init(verticalAmount: HKQuantity, verticalBase: HKPrismBase, horizontalAmount: HKQuantity, horizontalBase: HKPrismBase, eye: HKVisionEye)

Creates a new vision prism object that separates the correction strength into horizontal and vertical components.

