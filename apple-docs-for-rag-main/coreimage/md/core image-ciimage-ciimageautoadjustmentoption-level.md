

- Core Image
- CIImage
- CIImageAutoAdjustmentOption
-  level 

Type Property

# level

A key used to specify whether to return a filter that rotates the image to keep a level perspective.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
static let level: CIImageAutoAdjustmentOption
```

## Discussion

The value associated with this key is a `CFBoolean` value. If `true`, Core Image analyzes the image to determine whether it would benefit from rotation—for example, a landscape photo in which the horizon is not horizontal—and returns a filter to perform that rotation. Supply `false` to indicate not to return a rotation filter. If you don’t specify this option, Core Image assumes its value is `false`.

