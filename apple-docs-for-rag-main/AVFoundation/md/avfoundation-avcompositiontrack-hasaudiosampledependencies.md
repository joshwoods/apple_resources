

- AVFoundation
- AVCompositionTrack
-  hasAudioSampleDependencies 

Instance Property

# hasAudioSampleDependencies

A Boolean value that indicates whether the track has sample dependencies.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var hasAudioSampleDependencies: Bool { get }
```

## Discussion

The value is always false for nonaudible media.

## See Also

### Accessing Audible Characteristics

var preferredVolume: Float

The track’s volume preference for playing its audible media.

