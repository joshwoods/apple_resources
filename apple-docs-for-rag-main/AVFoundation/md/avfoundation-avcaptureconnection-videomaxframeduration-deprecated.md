

- AVFoundation
- AVCaptureConnection
-  videoMaxFrameDuration Deprecated

Instance Property

# videoMaxFrameDuration

The largest time interval the connection can apply between consecutive video frames.

Mac Catalyst 14.0–14.0DeprecatedmacOS 10.9+

``` source
var videoMaxFrameDuration: CMTime { get set }
```

Deprecated

Use AVCaptureDevice's activeVideoMaxFrameDuration instead.

## Discussion

When isVideoMaxFrameDurationSupported is true, the value of the property configures the upper bound for the amount of time a video connection separates consecutive frames. The value is equivalent to the reciprocal of the minimum frame rate.

You can set an unlimited frame rate with zero or invalid (which is the default).

## See Also

### Configuring a video’s frame rate

var isVideoMinFrameDurationSupported: Bool

A Boolean value that indicates whether the connection supports a minimum frame duration.

Deprecated

var videoMinFrameDuration: CMTime

The smallest time interval the connection can apply between consecutive video frames.

Deprecated

var isVideoMaxFrameDurationSupported: Bool

A Boolean value that indicates whether the connection supports a maximum frame duration.

Deprecated

