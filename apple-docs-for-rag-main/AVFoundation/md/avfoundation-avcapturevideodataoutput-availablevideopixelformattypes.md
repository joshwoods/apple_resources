

- AVFoundation
- AVCaptureVideoDataOutput
-  availableVideoPixelFormatTypes 

Instance Property

# availableVideoPixelFormatTypes

The video pixel formats the output supports.

iOS 5.0+iPadOS 5.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
@nonobjc
var availableVideoPixelFormatTypes: [OSType] { get }
```

## Discussion

This value contains an array of video formats, in unspecified order, that the output supports. You can set the format by specifying it as the kCVPixelBufferPixelFormatTypeKey entry in the output’s videoSettings dictionary.

Note

The contents of this list may change if the video capture device’s activeFormat value changes.

## See Also

### Retrieving Supported Video Types

var availableVideoCodecTypes: [AVVideoCodecType]

The video codecs that the output supports.

func availableVideoCodecTypesForAssetWriter(writingTo: AVFileType) -> [AVVideoCodecType]

The video codecs that the output supports for writing video to the output file.

struct AVVideoCodecType

A set of constants that describe the codecs the system supports for video capture.

