

- AVFoundation
- AVCaptureFileOutput
-  outputFileURL 

Instance Property

# outputFileURL

The URL to which output is directed.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var outputFileURL: URL? { get }
```

## See Also

### Setting File Output Properties

var delegate: (any AVCaptureFileOutputDelegate)?

The delegate object for the capture file output.

var maxRecordedDuration: CMTime

The longest duration allowed for the recording.

var maxRecordedFileSize: Int64

The maximum size, in bytes, of the data that should be recorded by the receiver.

var minFreeDiskSpaceLimit: Int64

The minimum amount of free space, in bytes, required for recording to continue on a given volume.

var recordedDuration: CMTime

Indicates the duration of the media recorded to the current output file.

var recordedFileSize: Int64

Indicates the size, in bytes, of the data recorded to the current output file.

var isRecording: Bool

Indicates whether recording is in progress.

var isRecordingPaused: Bool

Indicates whether recording to the current output file is paused.

