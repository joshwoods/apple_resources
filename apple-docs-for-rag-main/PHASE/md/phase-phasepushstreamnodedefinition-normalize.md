

- PHASE
- PHASEPushStreamNodeDefinition
-  normalize 

Instance Property

# normalize

An option that resizes loudness of the audio stream for consistency.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 17.0+visionOS 1.0+

``` source
var normalize: Bool { get set }
```

## Discussion

The default value is `false`. When `true`, the engine *normalizes* the audio stream — that is, it dynamically resizes loudness within a given range for a consistent listening experience. Normalization serves the benefit of assisting output level calibration. Apps that leave the value `false` need to normalize stream data manually before passing it into the framework (see pushStreamNodes).

