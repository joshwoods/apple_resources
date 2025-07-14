

- AVFoundation
- AVCaptureConnection
-  isVideoMaxFrameDurationSupported Deprecated

Instance Property

# isVideoMaxFrameDurationSupported

A Boolean value that indicates whether the connection supports a maximum frame duration.

Mac Catalyst 14.0–14.0DeprecatedmacOS 10.9+

``` source
var isVideoMaxFrameDurationSupported: Bool { get }
```

Deprecated

Use AVCaptureDevice's activeFormat.videoSupportedFrameRateRanges instead.

## Discussion

The property indicates whether the connection honors the videoMaxFrameDuration property for a video connection.

## See Also

### Configuring a video’s frame rate

var isVideoMinFrameDurationSupported: Bool

A Boolean value that indicates whether the connection supports a minimum frame duration.

Deprecated

var videoMinFrameDuration: CMTime

The smallest time interval the connection can apply between consecutive video frames.

Deprecated

var videoMaxFrameDuration: CMTime

The largest time interval the connection can apply between consecutive video frames.

Deprecated

