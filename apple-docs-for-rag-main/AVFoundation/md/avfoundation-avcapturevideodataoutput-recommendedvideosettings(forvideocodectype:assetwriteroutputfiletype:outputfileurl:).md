

- AVFoundation
- AVCaptureVideoDataOutput
-  recommendedVideoSettings(forVideoCodecType:assetWriterOutputFileType:outputFileURL:) 

Instance Method

# recommendedVideoSettings(forVideoCodecType:assetWriterOutputFileType:outputFileURL:)

Returns a dictionary of recommended output settings for writing the specified code, file type, and output URL.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
func recommendedVideoSettings(
    forVideoCodecType videoCodecType: AVVideoCodecType,
    assetWriterOutputFileType outputFileType: AVFileType,
    outputFileURL: URL?
) -> [String : Any]?
```

## Parameters 

`videoCodecType`  

The type of video codec to use.

`outputFileType`  

The type of output file to write.

`outputFileURL`  

The URL of the output file to write.

## Return Value

A fully populated output settings dictionary suitable for configuring an asset writer input.

## See Also

### Configuring Video Capture

var videoSettings: [String : Any]!

A dictionary that contains the compression settings for the output.

Video settings

Configure video processing settings using standard key and value constants.

var alwaysDiscardsLateVideoFrames: Bool

Indicates whether to drop video frames if they arrive late.

var automaticallyConfiguresOutputBufferDimensions: Bool

A Boolean value that indicates whether the output automatically configures the size of output buffers.

var deliversPreviewSizedOutputBuffers: Bool

A Boolean value that indicates whether the output is configured to deliver preview-sized buffers.

func recommendedVideoSettings(forVideoCodecType: AVVideoCodecType, assetWriterOutputFileType: AVFileType) -> [String : Any]?

Returns a video settings dictionary appropriate for capturing video to a file with the specified codec and type.

func recommendedVideoSettingsForAssetWriter(writingTo: AVFileType) -> [String : Any]?

Specifies the recommended settings for use with an AVAssetWriterInput.

