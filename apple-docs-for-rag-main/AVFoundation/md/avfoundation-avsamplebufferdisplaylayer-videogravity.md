

- AVFoundation
- AVSampleBufferDisplayLayer
-  videoGravity 

Instance Property

# videoGravity

A value that indicates how the layer displays video within its bounds.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
var videoGravity: AVLayerVideoGravity { get set }
```

## Discussion

AVLayerVideoGravity defines the supported video gravities. The default value is resizeAspect.

## See Also

### Configuring the layer

var isReadyForDisplay: Bool

A Boolean value that indicates whether the first video frame is ready for display.

var controlTimebase: CMTimebase?

A timebase that determines how the layer interprets timestamps.

struct AVLayerVideoGravity

A structure that defines how a layer displays a player’s visual content within the layer’s bounds.

