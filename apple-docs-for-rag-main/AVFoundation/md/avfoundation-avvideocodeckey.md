

- AVFoundation
-  AVVideoCodecKey 

Global Variable

# AVVideoCodecKey

A key to access the name of the codec for compressing video.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
let AVVideoCodecKey: String
```

## Mentioned in 

Recording movies in alternative formats

## Discussion

The value for this key is an instance of NSString, equivalent to CMVideoCodecType. Use this key to set the video compression format to H.264, HEVC, or JPEG, depending on the video codec types available in AVCaptureMovieFileOutput. Check available video codec types by consulting availableVideoCodecTypes.

## See Also

### Video codecs

struct AVVideoCodecType

A set of constants that describe the codecs the system supports for video capture.

