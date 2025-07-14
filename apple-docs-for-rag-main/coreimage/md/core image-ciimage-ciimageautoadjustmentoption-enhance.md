

- Core Image
- CIImage
- CIImageAutoAdjustmentOption
-  enhance 

Type Property

# enhance

A key used to specify whether to return enhancement filters.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
static let enhance: CIImageAutoAdjustmentOption
```

## Discussion

The value associated with this key is a `CFBoolean` value. Supply `false` to indicate not to return enhancement filters. If you don’t specify this option, Core Image assumes its value is `true`.

