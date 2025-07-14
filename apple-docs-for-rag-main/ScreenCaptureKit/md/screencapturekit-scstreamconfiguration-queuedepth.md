

- ScreenCaptureKit
- SCStreamConfiguration
-  queueDepth 

Instance Property

# queueDepth

The maximum number of frames for the queue to store.

Mac Catalyst 18.2+macOS 12.3+

``` source
var queueDepth: Int { get set }
```

## Discussion

By default, the system sets the queue depth to its minimum value of three frames. Specifying more frames uses more memory, but may allow you to process frame data without stalling the display stream.

Important

Don’t exceed a queue depth of eight frames.

## See Also

### Configuring captured frames

var minimumFrameInterval: CMTime

The desired minimum time between frame updates, in seconds.

var captureResolution: SCCaptureResolutionType

The resolution at which to capture source content.

enum SCCaptureResolutionType

Available resolutions for content capture.

