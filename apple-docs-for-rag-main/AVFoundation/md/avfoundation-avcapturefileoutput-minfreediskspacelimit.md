

- AVFoundation
- AVCaptureFileOutput
-  minFreeDiskSpaceLimit 

Instance Property

# minFreeDiskSpaceLimit

The minimum amount of free space, in bytes, required for recording to continue on a given volume.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var minFreeDiskSpaceLimit: Int64 { get set }
```

## Discussion

This property specifies a hard lower limit on the amount of free space that must remain on a target volume for recording to continue. Recording is stopped when the limit is reached and the fileOutput(_:didFinishRecordingTo:from:error:) delegate method is invoked with an appropriate error.

## See Also

### Setting File Output Properties

var delegate: (any AVCaptureFileOutputDelegate)?

The delegate object for the capture file output.

var maxRecordedDuration: CMTime

The longest duration allowed for the recording.

var maxRecordedFileSize: Int64

The maximum size, in bytes, of the data that should be recorded by the receiver.

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

