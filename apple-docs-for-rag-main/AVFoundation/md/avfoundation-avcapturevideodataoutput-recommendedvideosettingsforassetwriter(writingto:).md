

- AVFoundation
- AVCaptureVideoDataOutput
-  recommendedVideoSettingsForAssetWriter(writingTo:) 

Instance Method

# recommendedVideoSettingsForAssetWriter(writingTo:)

Specifies the recommended settings for use with an AVAssetWriterInput.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+

``` source
func recommendedVideoSettingsForAssetWriter(writingTo outputFileType: AVFileType) -> [String : Any]?
```

## Parameters 

`outputFileType`  

The Uniform Type Identifier of the file type to write. See `File Format UTIs` for supported types.

## Return Value

A fully populated dictionary of keys and values that are compatible with AVAssetWriter.

## Discussion

This dictionary contains keys and values described in Video settings and is suitable for use when creating an AVAssetWriterInput with the init(mediaType:outputSettings:) initializer. For QuickTime movie and ISO file types, the recommended video settings produce output comparable to that of AVCaptureMovieFileOutput.

Note that the dictionary of settings is dependent on the current configuration of the output’s AVCaptureSession and its inputs. The settings dictionary may change if the session’s configuration changes. As such, configure your session first, then query the recommended video settings.

Note

This method returns appropriate settings based on the device’s default video recording codec, but that default can differ between devices. Use the recommendedVideoSettings(forVideoCodecType:assetWriterOutputFileType:) method to obtain video settings appropriate for a specific codec.

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

func recommendedVideoSettings(forVideoCodecType: AVVideoCodecType, assetWriterOutputFileType: AVFileType, outputFileURL: URL?) -> [String : Any]?

Returns a dictionary of recommended output settings for writing the specified code, file type, and output URL.

