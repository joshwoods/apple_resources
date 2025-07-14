

- ScreenCaptureKit
- SCStreamConfiguration
-  minimumFrameInterval 

Instance Property

# minimumFrameInterval

The desired minimum time between frame updates, in seconds.

Mac Catalyst 18.2+macOS 12.3+

``` source
var minimumFrameInterval: CMTime { get set }
```

## Discussion

Use this value to throttle the rate at which you receive updates. The default value is `0`, which indicates that the system uses the maximum supported frame rate.

You specify the minimum frame interval as the reciprocal of the maximum frame rate. For example, to configure the stream to capture at 60 fps, specify a minimum frame interval equal to `1/60`.

```
let config = SCStreamConfiguration()
config.minimumFrameInterval = CMTime(value: 1, timescale: CMTimeScale(60))
```

## See Also

### Configuring captured frames

var queueDepth: Int

The maximum number of frames for the queue to store.

var captureResolution: SCCaptureResolutionType

The resolution at which to capture source content.

enum SCCaptureResolutionType

Available resolutions for content capture.

