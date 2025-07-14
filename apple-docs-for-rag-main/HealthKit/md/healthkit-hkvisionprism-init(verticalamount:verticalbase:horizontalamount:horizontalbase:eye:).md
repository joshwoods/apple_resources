

- HealthKit
- HKVisionPrism
-  init(verticalAmount:verticalBase:horizontalAmount:horizontalBase:eye:) 

Initializer

# init(verticalAmount:verticalBase:horizontalAmount:horizontalBase:eye:)

Creates a new vision prism object that separates the correction strength into horizontal and vertical components.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    verticalAmount: HKQuantity,
    verticalBase: HKPrismBase,
    horizontalAmount: HKQuantity,
    horizontalBase: HKPrismBase,
    eye: HKVisionEye
)
```

## Parameters 

`verticalAmount`  

The vertical strength of the correction, measured in prismDiopter() units.

`verticalBase`  

The orientation of the vertical correction. This value can be either HKPrismBase.up or HKPrismBase.down.

`horizontalAmount`  

The horizontal strength of the correction, measured in prismDiopter() units.

`horizontalBase`  

The orientation of the horizontal correction. This value can be either HKPrismBase.in or HKPrismBase.out.

`eye`  

A value indicating which eye the correction applies to: HKVisionEye.left or HKVisionEye.right.

## See Also

### Creating vision prism objects

init(amount: HKQuantity, angle: HKQuantity, eye: HKVisionEye)

Creates a new vision prism object, using a single quantity and an alignment angle.

