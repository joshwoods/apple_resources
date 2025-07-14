

- AVFoundation
- AVPartialAsyncProperty
-  hasAudioSampleDependencies 

Type Property

# hasAudioSampleDependencies

A Boolean value that indicates whether the track has sample dependencies.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var hasAudioSampleDependencies: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

The value is always false for nonaudible media.

## See Also

### Loading Audible Characteristics

static var preferredVolume: AVAsyncProperty&lt;Root, Float>

The track’s volume preference for playing its audible media.

