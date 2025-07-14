

- AVFoundation
- AVCaptureVideoDataOutput
-  automaticallyConfiguresOutputBufferDimensions 

Instance Property

# automaticallyConfiguresOutputBufferDimensions

A Boolean value that indicates whether the output automatically configures the size of output buffers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var automaticallyConfiguresOutputBufferDimensions: Bool { get set }
```

## Discussion

In most configurations, AVCaptureVideoDataOutput delivers full-resolution buffers that match the video dimensions of the capture device’s activeFormat property. When this property is true, the output is free to scale the buffers delivered to captureOutput(_:didOutput:from:) to a size suitable for preview (approximately the size of the screen).

You can query this property to find out whether the automatic configuration of output buffer dimensions is downscaling buffers to a preview size. You can also query the output’s videoSettings dictionary to find the buffer’s exact dimensions.

The default value of this property is true.

Important

You must set this property to false before you can manually set deliversPreviewSizedOutputBuffers to true.

## See Also

### Configuring Video Capture

var videoSettings: [String : Any]!

A dictionary that contains the compression settings for the output.

Video settings

Configure video processing settings using standard key and value constants.

var alwaysDiscardsLateVideoFrames: Bool

Indicates whether to drop video frames if they arrive late.

var deliversPreviewSizedOutputBuffers: Bool

A Boolean value that indicates whether the output is configured to deliver preview-sized buffers.

func recommendedVideoSettings(forVideoCodecType: AVVideoCodecType, assetWriterOutputFileType: AVFileType) -> [String : Any]?

Returns a video settings dictionary appropriate for capturing video to a file with the specified codec and type.

func recommendedVideoSettings(forVideoCodecType: AVVideoCodecType, assetWriterOutputFileType: AVFileType, outputFileURL: URL?) -> [String : Any]?

Returns a dictionary of recommended output settings for writing the specified code, file type, and output URL.

func recommendedVideoSettingsForAssetWriter(writingTo: AVFileType) -> [String : Any]?

Specifies the recommended settings for use with an AVAssetWriterInput.

