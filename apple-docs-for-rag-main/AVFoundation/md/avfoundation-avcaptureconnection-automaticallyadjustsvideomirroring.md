

- AVFoundation
- AVCaptureConnection
-  automaticallyAdjustsVideoMirroring 

Instance Property

# automaticallyAdjustsVideoMirroring

A Boolean value that indicates whether you can enable mirroring based on a session’s configuration.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var automaticallyAdjustsVideoMirroring: Bool { get set }
```

## Discussion

For some session configurations, the connection mirrors the video data by default. When the value of this property is true, the value of isVideoMirrored may change, depending on the configuration of the session. For example, the value may change after switching to a different capture device input.

The default value is true.

## See Also

### Mirroring a video

var isVideoMirroringSupported: Bool

A Boolean value that indicates whether the connection supports video mirroring.

var isVideoMirrored: Bool

A Boolean value that indicates whether the connection horizontally flips the video flowing through it.

