

- AVFoundation
- AVCaptureConnection
-  isVideoMinFrameDurationSupported Deprecated

Instance Property

# isVideoMinFrameDurationSupported

A Boolean value that indicates whether the connection supports a minimum frame duration.

Mac Catalyst 14.0–14.0DeprecatedmacOS 10.7+

``` source
var isVideoMinFrameDurationSupported: Bool { get }
```

Deprecated

Use AVCaptureDevice's activeFormat.videoSupportedFrameRateRanges instead.

## Discussion

The property indicates whether the connection honors the videoMinFrameDuration property for a video connection.

## See Also

### Configuring a video’s frame rate

var videoMinFrameDuration: CMTime

The smallest time interval the connection can apply between consecutive video frames.

Deprecated

var isVideoMaxFrameDurationSupported: Bool

A Boolean value that indicates whether the connection supports a maximum frame duration.

Deprecated

var videoMaxFrameDuration: CMTime

The largest time interval the connection can apply between consecutive video frames.

Deprecated

