

- AVFoundation
- AVCapturePhotoSettings
-  livePhotoVideoCodecType 

Instance Property

# livePhotoVideoCodecType

The video codec to use for encoding the movie portion of Live Photo output.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var livePhotoVideoCodecType: AVVideoCodecType { get set }
```

## Discussion

This value must be one of the video codec types listed in the photo output’s availableLivePhotoVideoCodecTypes array.

## See Also

### Configuring Live Photo Settings

var livePhotoMovieFileURL: URL?

A URL at which to write Live Photo movie output.

var livePhotoMovieMetadata: [AVMetadataItem]!

A dictionary of metadata to include in the Live Photo movie file.

