

- AVFoundation
- AVCaptureFileOutput
-  maxRecordedFileSize 

Instance Property

# maxRecordedFileSize

The maximum size, in bytes, of the data that should be recorded by the receiver.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var maxRecordedFileSize: Int64 { get set }
```

## Discussion

This property specifies a hard limit on the data size of recorded files. Recording is stopped when the limit is reached and the fileOutput(_:didFinishRecordingTo:from:error:) delegate method is invoked with an appropriate error. The default value of this property is `0`, which indicates no limit.

## See Also

### Setting File Output Properties

var delegate: (any AVCaptureFileOutputDelegate)?

The delegate object for the capture file output.

var maxRecordedDuration: CMTime

The longest duration allowed for the recording.

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

var isRecordingPaused: Bool

Indicates whether recording to the current output file is paused.

