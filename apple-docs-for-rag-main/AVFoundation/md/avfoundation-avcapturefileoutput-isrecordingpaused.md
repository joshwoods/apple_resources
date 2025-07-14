

- AVFoundation
- AVCaptureFileOutput
-  isRecordingPaused 

Instance Property

# isRecordingPaused

Indicates whether recording to the current output file is paused.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 10.7+tvOS 18.0+

``` source
var isRecordingPaused: Bool { get }
```

## Discussion

This property indicates recording to the file returned by outputFileURL has been previously paused using the pauseRecording() method. When a recording is paused, captured samples are not written to the output file, but new samples can be written to the same file in the future by calling resumeRecording().

## See Also

### Related Documentation

func pauseRecording()

Pauses recording to the current output file.

func stopRecording()

Tells the receiver to stop recording to the current file.

### Setting File Output Properties

var delegate: (any AVCaptureFileOutputDelegate)?

The delegate object for the capture file output.

var maxRecordedDuration: CMTime

The longest duration allowed for the recording.

var maxRecordedFileSize: Int64

The maximum size, in bytes, of the data that should be recorded by the receiver.

var minFreeDiskSpaceLimit: Int64

The minimum amount of free space, in bytes, required for recording to continue on a given volume.

var outputFileURL: URL?

The URL to which output is directed.

var recordedDuration: CMTime

Indicates the duration of the media recorded to the current output file.

var recordedFileSize: Int64

Indicates the size, in bytes, of the data recorded to the current output file.

var isRecording: Bool

Indicates whether recording is in progress.

