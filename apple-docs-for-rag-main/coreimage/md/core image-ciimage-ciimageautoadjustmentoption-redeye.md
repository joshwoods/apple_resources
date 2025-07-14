

- Core Image
- CIImage
- CIImageAutoAdjustmentOption
-  redEye 

Type Property

# redEye

A key used to specify whether to return a red eye filter.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
static let redEye: CIImageAutoAdjustmentOption
```

## Discussion

The value associated with this key is a `CFBoolean` value. Supply `false` to indicate not to return a red eye filter. If you don’t specify this option, Core Image assumes its value is `true`.

