

- AVFoundation
- AVCaptureVideoDataOutput
-  alwaysDiscardsLateVideoFrames 

Instance Property

# alwaysDiscardsLateVideoFrames

Indicates whether to drop video frames if they arrive late.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
var alwaysDiscardsLateVideoFrames: Bool { get set }
```

## Discussion

If this property is true, the output immediately discard frames that captured while the dispatch queue handling existing frames blocks in the captureOutput(_:didOutput:from:) delegate method. When set to false, the output gives delegates more time to process old frames before it discards new frames, but application memory usage may increase significantly as a result.

The default is true.

## See Also

### Configuring Video Capture

var videoSettings: [String : Any]!

A dictionary that contains the compression settings for the output.

Video settings

Configure video processing settings using standard key and value constants.

var automaticallyConfiguresOutputBufferDimensions: Bool

A Boolean value that indicates whether the output automatically configures the size of output buffers.

var deliversPreviewSizedOutputBuffers: Bool

A Boolean value that indicates whether the output is configured to deliver preview-sized buffers.

func recommendedVideoSettings(forVideoCodecType: AVVideoCodecType, assetWriterOutputFileType: AVFileType) -> [String : Any]?

Returns a video settings dictionary appropriate for capturing video to a file with the specified codec and type.

func recommendedVideoSettings(forVideoCodecType: AVVideoCodecType, assetWriterOutputFileType: AVFileType, outputFileURL: URL?) -> [String : Any]?

Returns a dictionary of recommended output settings for writing the specified code, file type, and output URL.

func recommendedVideoSettingsForAssetWriter(writingTo: AVFileType) -> [String : Any]?

Specifies the recommended settings for use with an AVAssetWriterInput.

