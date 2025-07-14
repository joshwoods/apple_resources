

- AVFoundation
- AVPartialAsyncProperty
-  preferredVolume 

Type Property

# preferredVolume

The track’s volume preference for playing its audible media.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var preferredVolume: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

The preferred volume for an audio track is typically, but not always, `1.0`. For nonaudible tracks, the value is `0.0`.

## See Also

### Loading Audible Characteristics

static var hasAudioSampleDependencies: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track has sample dependencies.

