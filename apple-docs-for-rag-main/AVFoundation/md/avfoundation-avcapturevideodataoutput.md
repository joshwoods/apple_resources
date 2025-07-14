

- AVFoundation
-  AVCaptureVideoDataOutput 

Class

# AVCaptureVideoDataOutput

A capture output that records video and provides access to video frames for processing.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
class AVCaptureVideoDataOutput
```

## Mentioned in 

Setting Up a Capture Session

## Overview

Use this output to process compressed or uncompressed frames from the captured video. You can access the frames with the captureOutput(_:didOutput:from:) delegate method.

This object supports compressed video data output for macOS only. It can output pixel buffers in several pixel formats. Consider the usability and performance characteristics of these formats and choose the best format for your app.

Important

Avoid defaulting to a BGRA format, because BGRA formats aren’t native and require conversion. Additionally, BGRA formats requires significantly more memory than many of the native formats. For more information, see TN3121: Selecting a pixel format for an AVCaptureVideoDataOutput.

## Topics

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

func recommendedVideoSettingsForAssetWriter(writingTo: AVFileType) -> [String : Any]?

Specifies the recommended settings for use with an AVAssetWriterInput.

### Retrieving Supported Video Types

var availableVideoPixelFormatTypes: [OSType]

The video pixel formats the output supports.

var availableVideoCodecTypes: [AVVideoCodecType]

The video codecs that the output supports.

func availableVideoCodecTypesForAssetWriter(writingTo: AVFileType) -> [AVVideoCodecType]

The video codecs that the output supports for writing video to the output file.

struct AVVideoCodecType

A set of constants that describe the codecs the system supports for video capture.

### Receiving Captured Video Data

func setSampleBufferDelegate((any AVCaptureVideoDataOutputSampleBufferDelegate)?, queue: dispatch_queue_t?)

Sets the sample buffer delegate and the queue for invoking callbacks.

var sampleBufferDelegate: (any AVCaptureVideoDataOutputSampleBufferDelegate)?

The capture object’s delegate.

var sampleBufferCallbackQueue: dispatch_queue_t?

The queue on which the system invokes delegate callbacks.

protocol AVCaptureVideoDataOutputSampleBufferDelegate

Methods for receiving sample buffers from, and monitoring the status of, a video data output.

### Creating Video Capture Output

init()

Creates a new video file output.

## Relationships

### Inherits From

- AVCaptureOutput

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Stream capture

class AVCaptureAudioDataOutput

A capture output that records audio and provides access to audio sample buffers as they are recorded.

