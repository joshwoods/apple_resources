

- RealityKit
- VideoPlayerComponent
-  avPlayer 

Instance Property

# avPlayer

The AV player that the component plays.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var avPlayer: AVPlayer? { get }
```

## Discussion

Pass this player to the component as a parameter in the initializer; you can’t replace it afterward.

## See Also

### Accessing video player properties

var playerScreenSize: SIMD2&lt;Float>

The screen entity size of the current video player in meters.

var screenVideoDimension: SIMD2&lt;Float>

The video resolution size.

var videoRenderer: AVSampleBufferVideoRenderer?

The component’s video renderer.

var viewingMode: VideoPlaybackController.ViewingMode?

The current content-viewing mode for video playback.

