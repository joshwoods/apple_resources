

- RealityKit
- VideoPlayerComponent
-  videoRenderer 

Instance Property

# videoRenderer

The component’s video renderer.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var videoRenderer: AVSampleBufferVideoRenderer? { get }
```

## Discussion

Pass this renderer to the component as a parameter in the initializer; you can’t replace it afterward. You can’t use the same `AVSampleBufferVideoRenderer` object with more than one `VideoPlayerComponent`.

## See Also

### Accessing video player properties

var avPlayer: AVPlayer?

The AV player that the component plays.

var playerScreenSize: SIMD2&lt;Float>

The screen entity size of the current video player in meters.

var screenVideoDimension: SIMD2&lt;Float>

The video resolution size.

var viewingMode: VideoPlaybackController.ViewingMode?

The current content-viewing mode for video playback.

