

- AVFoundation
-  AVCaptureAudioDataOutput 

Class

# AVCaptureAudioDataOutput

A capture output that records audio and provides access to audio sample buffers as they are recorded.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
class AVCaptureAudioDataOutput
```

## Topics

### Creating an Audio Capture Output

init()

Creates an instance of audio data output.

### Configuring Audio Capture

var audioSettings: [String : Any]!

The settings used to decode or re-encode audio before it’s output.

func recommendedAudioSettingsForAssetWriter(writingTo: AVFileType) -> [String : Any]?

Specifies the recommended settings for use with an `AVAssetWriterInput`.

### Receiving Captured Audio Data

func setSampleBufferDelegate((any AVCaptureAudioDataOutputSampleBufferDelegate)?, queue: dispatch_queue_t?)

Sets the delegate that will accept captured buffers and the dispatch queue on which the delegate will be called.

var sampleBufferDelegate: (any AVCaptureAudioDataOutputSampleBufferDelegate)?

The capture object’s delegate.

var sampleBufferCallbackQueue: dispatch_queue_t?

The queue on which delegate callbacks are invoked

protocol AVCaptureAudioDataOutputSampleBufferDelegate

Methods for receiving audio sample data from an audio capture.

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

class AVCaptureVideoDataOutput

A capture output that records video and provides access to video frames for processing.

