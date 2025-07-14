

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.DynamicRangePolicy
-  forceSDR 

Type Property

# forceSDR

A policy that forces conversion to standard dynamic range.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
static let forceSDR: AVAssetImageGenerator.DynamicRangePolicy
```

## Discussion

This policy converts PQ or HLG transfer functions to 709, while maintaining color primaries and matrix.

## See Also

### Policies

static let matchSource: AVAssetImageGenerator.DynamicRangePolicy

A policy that preserves the color parameters of the source media.

