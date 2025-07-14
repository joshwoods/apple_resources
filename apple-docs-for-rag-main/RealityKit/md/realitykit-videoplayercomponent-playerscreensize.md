

- RealityKit
- VideoPlayerComponent
-  playerScreenSize 

Instance Property

# playerScreenSize

The screen entity size of the current video player in meters.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var playerScreenSize: SIMD2 { get }
```

## Discussion

This property has the format `[width, height]`.

## See Also

### Accessing video player properties

var avPlayer: AVPlayer?

The AV player that the component plays.

var screenVideoDimension: SIMD2&lt;Float>

The video resolution size.

var videoRenderer: AVSampleBufferVideoRenderer?

The component’s video renderer.

var viewingMode: VideoPlaybackController.ViewingMode?

The current content-viewing mode for video playback.

