

- AVFoundation
- AVCaptureVideoDataOutput
-  deliversPreviewSizedOutputBuffers 

Instance Property

# deliversPreviewSizedOutputBuffers

A Boolean value that indicates whether the output is configured to deliver preview-sized buffers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var deliversPreviewSizedOutputBuffers: Bool { get set }
```

## Discussion

AVCaptureVideoDataOutput produces preview-sized buffers, which are approximately the size of the screen, when its automaticallyConfiguresOutputBufferDimensions property is true. If you wish to manually set this property, you must first set automaticallyConfiguresOutputBufferDimensions to false.

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

func recommendedVideoSettings(forVideoCodecType: AVVideoCodecType, assetWriterOutputFileType: AVFileType) -> [String : Any]?

Returns a video settings dictionary appropriate for capturing video to a file with the specified codec and type.

func recommendedVideoSettings(forVideoCodecType: AVVideoCodecType, assetWriterOutputFileType: AVFileType, outputFileURL: URL?) -> [String : Any]?

Returns a dictionary of recommended output settings for writing the specified code, file type, and output URL.

func recommendedVideoSettingsForAssetWriter(writingTo: AVFileType) -> [String : Any]?

Specifies the recommended settings for use with an AVAssetWriterInput.

