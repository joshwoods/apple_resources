

- AVFoundation
- AVSampleBufferDisplayLayer
-  isReadyForDisplay 

Instance Property

# isReadyForDisplay

A Boolean value that indicates whether the first video frame is ready for display.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+

``` source
var isReadyForDisplay: Bool { get }
```

## See Also

### Configuring the layer

var controlTimebase: CMTimebase?

A timebase that determines how the layer interprets timestamps.

var videoGravity: AVLayerVideoGravity

A value that indicates how the layer displays video within its bounds.

struct AVLayerVideoGravity

A structure that defines how a layer displays a player’s visual content within the layer’s bounds.

