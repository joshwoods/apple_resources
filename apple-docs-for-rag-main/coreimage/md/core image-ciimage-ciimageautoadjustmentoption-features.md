

- Core Image
- CIImage
- CIImageAutoAdjustmentOption
-  features 

Type Property

# features

A key used to specify an array of features that you want to apply enhancement and red eye filters to.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
static let features: CIImageAutoAdjustmentOption
```

## Discussion

The associated value is an array of `CIFeature` objects. If you don’t supply an array, the Core Image searches for features using the `CIDetector` class.

