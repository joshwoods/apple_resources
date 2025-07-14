

- Core Image
- CIImage
- CIImageAutoAdjustmentOption
-  crop 

Type Property

# crop

A key used to specify whether to return a filter that crops the image to focus on detected features.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
static let crop: CIImageAutoAdjustmentOption
```

## Discussion

The value associated with this key is a `CFBoolean` value. If `true`, the returned filters include an operation that crops the image around the features specified with the `features` option (or any features detected in the image, if that option is not present). Supply `false` to indicate not to return a crop filter. If you don’t specify this option, Core Image assumes its value is `false`.

