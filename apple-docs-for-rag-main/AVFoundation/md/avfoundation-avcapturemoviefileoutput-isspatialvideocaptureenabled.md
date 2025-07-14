

- AVFoundation
- AVCaptureMovieFileOutput
-  isSpatialVideoCaptureEnabled 

Instance Property

# isSpatialVideoCaptureEnabled

A Boolean value that indicates whether a movie file output captures spatial videos.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var isSpatialVideoCaptureEnabled: Bool { get set }
```

## Discussion

Spatial capture lets you record your favorite moments in 3D for playback on Apple Vision Pro. This feature isn’t supported on all devices, so you can only enable this property when isSpatialVideoCaptureSupported is true.

The default value is false.

## See Also

### Enabling spatial capture

var isSpatialVideoCaptureSupported: Bool

A Boolean value that indicates whether a movie file output supports capturing spatial videos.

