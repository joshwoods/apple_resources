

- RealityKit
- VideoPlayerComponent
-  screenVideoDimension 

Instance Property

# screenVideoDimension

The video resolution size.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
var screenVideoDimension: SIMD2 { get }
```

## Discussion

This property has the format `[width, height]`, for example, `[1920, 1080]`.

## See Also

### Accessing video player properties

var avPlayer: AVPlayer?

The AV player that the component plays.

var playerScreenSize: SIMD2&lt;Float>

The screen entity size of the current video player in meters.

var videoRenderer: AVSampleBufferVideoRenderer?

The component’s video renderer.

var viewingMode: VideoPlaybackController.ViewingMode?

The current content-viewing mode for video playback.

