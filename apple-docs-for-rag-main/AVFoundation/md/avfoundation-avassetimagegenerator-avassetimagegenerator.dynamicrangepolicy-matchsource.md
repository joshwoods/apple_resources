

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.DynamicRangePolicy
-  matchSource 

Type Property

# matchSource

A policy that preserves the color parameters of the source media.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
static let matchSource: AVAssetImageGenerator.DynamicRangePolicy
```

## Discussion

By default, an image generator converts images to standard dynamic range. When working with HDR video, use this policy to preserve HDR color in the resulting images.

## See Also

### Policies

static let forceSDR: AVAssetImageGenerator.DynamicRangePolicy

A policy that forces conversion to standard dynamic range.

