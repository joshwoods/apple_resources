

- AVFoundation
- AVCaptureVideoDataOutput
-  availableVideoCodecTypesForAssetWriter(writingTo:) 

Instance Method

# availableVideoCodecTypesForAssetWriter(writingTo:)

The video codecs that the output supports for writing video to the output file.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func availableVideoCodecTypesForAssetWriter(writingTo outputFileType: AVFileType) -> [AVVideoCodecType]
```

## Parameters 

`outputFileType`  

The UTI of the output file type.

## Return Value

An array of video codecs.

## See Also

### Retrieving Supported Video Types

var availableVideoPixelFormatTypes: [OSType]

The video pixel formats the output supports.

var availableVideoCodecTypes: [AVVideoCodecType]

The video codecs that the output supports.

struct AVVideoCodecType

A set of constants that describe the codecs the system supports for video capture.

